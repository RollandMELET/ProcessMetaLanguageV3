/*
<!-- START OF FILE: Embedded-Element-PML-From-Template.md -->
FILENAME: Embedded-Element-PML-From-Template.md
Version: 3.4.0
Date: 2025-01-19 20:00
Author: Rolland MELET & Claude Code
Description: Script ProcessMetaLanguage V3 pour créer des éléments Excalidraw avec variables.
             Version 3.4.0 - Ajout de l'élément image pour embedding visuel complet

Changelog:
- v3.4.0: Ajout de l'élément image dans le JSON pour embedding visuel complet
- v3.3.0: Création des objets dans le même dossier que le canvas pour embedding correct
- v3.2.2: Correction erreur MarkdownView non défini, suppression rechargement inutile
- v3.2.1: Correction ordre paramètres utils.suggester (labels, values)
- v3.2.0: Correction utils.suggester (fonction, pas constructeur) et suppression test Excalidraw inutile
- v3.1.0: Remplacement yesNoPrompt par inputPrompt avec validation oui/non
- v3.0.9: Format correct sans backticks markdown pour Excalidraw
- v3.0.8: Version minimale debug
- v3.0.7: Version sans contrôle de compression pour debug
- v3.0.6: Solution définitive backticks avec String.fromCharCode(96)
- v3.0.5: Correction définitive regex sans backticks
- v3.0.4: Correction regex backticks, ajout log version console
- v3.0.3: Suppression méthode EA, correction format embed |100%, regex Embedded Files, warning compression
- v3.0.2: Ajout méthode EA pour embedding direct
- v3.0.1: Correction popup collecte variables
- v3.0.0: Version initiale ProcessMetaLanguage V3
*/

// ============================================
// PROCESSMETALANGUAGE V3 - EMBEDDED ELEMENT
// ============================================

const SCRIPT_VERSION = "3.4.0";
const SCRIPT_NAME = "ProcessMetaLanguage V3 - Embedded Element";

// Configuration des chemins
const TEMPLATES_PATH = "Templates";
const OBJECTS_PATH = "Objects";  // Non utilisé dans v3.3.0+
const TEMP_PATH = ".temp";

// ============================================
// FONCTION UTILITAIRE : LOGGING
// ============================================

/**
 * Log un message avec préfixe ProcessMetaLanguage
 * @param {string} message - Message à logger
 * @param {string} level - Niveau de log (info, warning, error)
 */
function log(message, level = "info") {
    const prefix = "[" + SCRIPT_NAME + " v" + SCRIPT_VERSION + "]";
    const timestamp = new Date().toISOString();
    
    switch(level) {
        case "error":
            console.error(prefix + " [ERROR] " + timestamp + ": " + message);
            break;
        case "warning":
            console.warn(prefix + " [WARNING] " + timestamp + ": " + message);
            break;
        default:
            console.log(prefix + " [INFO] " + timestamp + ": " + message);
    }
}

// ============================================
// GESTION DES TEMPLATES
// ============================================

/**
 * Récupère la liste des templates disponibles
 * @returns {Promise<Array>} Liste des templates
 */
async function getTemplatesList() {
    log("Recherche des templates ProcessMetaLanguage V3...");
    
    try {
        const templatesFolder = app.vault.getAbstractFileByPath(TEMPLATES_PATH);
        if (!templatesFolder) {
            log("Dossier " + TEMPLATES_PATH + " non trouvé", "error");
            return [];
        }

        const templates = [];
        const files = templatesFolder.children || [];
        
        for (const file of files) {
            if (file.extension === "md") {
                const content = await app.vault.read(file);
                
                // Vérifier si c'est un template ProcessMetaLanguage V3
                if (content.includes("processmetalanguage_version:") && 
                    content.includes("property_definitions:")) {
                    
                    // Extraire le type de template
                    const typeMatch = content.match(/template_type:\s*"([^"]+)"/);
                    const templateType = typeMatch ? typeMatch[1] : "generic";
                    
                    templates.push({
                        name: file.basename,
                        path: file.path,
                        type: templateType,
                        displayName: file.basename + " (" + templateType + ")"
                    });
                    
                    log("Template trouvé: " + file.basename + " (type: " + templateType + ")");
                }
            }
        }
        
        log(templates.length + " template(s) ProcessMetaLanguage V3 trouvé(s)");
        return templates;
        
    } catch (error) {
        log("Erreur lors de la recherche des templates: " + error.message, "error");
        return [];
    }
}

/**
 * Sélectionner un template via un dialogue
 * @param {Array} templates - Liste des templates
 * @returns {Promise<Object>} Template sélectionné
 */
async function selectTemplate(templates) {
    if (templates.length === 0) {
        throw new Error("Aucun template ProcessMetaLanguage V3 disponible");
    }
    
    // Utiliser utils.suggester avec le bon ordre de paramètres
    const selected = await utils.suggester(
        templates.map(t => t.displayName),
        templates
    );
    
    if (!selected) {
        throw new Error("Aucun template sélectionné");
    }
    
    log("Template sélectionné: " + selected.name);
    return selected;
}

// ============================================
// PARSING PROCESSMETALANGUAGE V3
// ============================================

/**
 * Parse les property_definitions d'un template
 * @param {string} content - Contenu du template
 * @returns {Object} Définitions des propriétés
 */
function parsePropertyDefinitions(content) {
    log("Parsing des property_definitions...");
    
    const propertyDefs = {};
    
    // Extraire la section property_definitions
    const propsMatch = content.match(/property_definitions:\s*\n([\s\S]*?)(?=\n[^\s]|\n---|\n#|$)/);
    if (!propsMatch) {
        log("Aucune property_definitions trouvée", "warning");
        return propertyDefs;
    }
    
    const propsSection = propsMatch[1];
    
    // Parser chaque propriété
    const propRegex = /^\s{2}(\w+):\s*\n([\s\S]*?)(?=\n\s{2}\w+:|\n[^\s]|$)/gm;
    let match;
    
    while ((match = propRegex.exec(propsSection)) !== null) {
        const propName = match[1];
        const propContent = match[2];
        
        const property = {
            name: propName,
            source: extractValue(propContent, "source") || "user",
            required: extractValue(propContent, "required") === "true",
            prompt: extractValue(propContent, "prompt") || propName + ":",
            description: extractValue(propContent, "description"),
            default_value: extractValue(propContent, "default_value"),
            options: extractOptions(propContent)
        };
        
        propertyDefs[propName] = property;
        log("Propriété parsée: " + propName + " (source: " + property.source + ")");
    }
    
    return propertyDefs;
}

/**
 * Extrait une valeur d'une propriété YAML
 * @param {string} content - Contenu YAML
 * @param {string} key - Clé à extraire
 * @returns {string} Valeur extraite
 */
function extractValue(content, key) {
    const regex = new RegExp(key + ":\\s*\"?([^\"\\n]+)\"?", 'i');
    const match = content.match(regex);
    return match ? match[1].trim() : null;
}

/**
 * Extrait les options d'une propriété
 * @param {string} content - Contenu YAML
 * @returns {Array} Liste des options
 */
function extractOptions(content) {
    const optionsMatch = content.match(/options:\s*\[(.*?)\]/);
    if (!optionsMatch) return [];
    
    return optionsMatch[1]
        .split(',')
        .map(opt => opt.trim().replace(/[\"']/g, ''))
        .filter(opt => opt.length > 0);
}

// ============================================
// COLLECTE DES VALEURS DE VARIABLES
// ============================================

/**
 * Collecte les valeurs pour les variables selon leur source
 * @param {Object} propertyDefs - Définitions des propriétés
 * @param {Array} variables - Liste des variables trouvées
 * @returns {Promise<Object>} Valeurs collectées
 */
async function collectVariableValues(propertyDefs, variables) {
    log("Collecte des valeurs de variables...");
    const values = {};
    
    for (const variable of variables) {
        const propDef = propertyDefs[variable];
        
        if (!propDef) {
            log("Variable " + variable + " non définie dans property_definitions", "warning");
            // Demander à l'utilisateur pour les variables non définies
            try {
                const promptText = variable + ":";
                const value = await utils.inputPrompt(promptText, "");
                values[variable] = value || "";
                log("Variable non définie " + variable + ": \"" + values[variable] + "\"");
            } catch (e) {
                log("Erreur lors de la collecte de " + variable + ": " + e.message, "error");
                values[variable] = "";
            }
            continue;
        }
        
        // Traiter selon la source
        switch (propDef.source) {
            case "user":
                values[variable] = await collectUserValue(propDef);
                break;
                
            case "template":
                values[variable] = propDef.default_value || "";
                log("Variable template " + variable + ": \"" + values[variable] + "\"");
                break;
                
            case "embedded":
                values[variable] = await collectEmbeddedValue(propDef);
                break;
                
            case "auto":
                values[variable] = generateAutoValue(propDef);
                break;
                
            default:
                values[variable] = propDef.default_value || "";
                log("Variable " + variable + " (source: " + propDef.source + "): \"" + values[variable] + "\"");
        }
    }
    
    return values;
}

/**
 * Collecte une valeur depuis l'utilisateur
 * @param {Object} propDef - Définition de la propriété
 * @returns {Promise<string>} Valeur saisie
 */
async function collectUserValue(propDef) {
    try {
        let value;
        
        if (propDef.options && propDef.options.length > 0) {
            // Utiliser utils.suggester avec le bon ordre de paramètres
            value = await utils.suggester(
                propDef.options,
                propDef.options
            );
        } else {
            // Input simple
            const promptText = propDef.prompt || propDef.name + ":";
            const defaultVal = propDef.default_value || "";
            value = await utils.inputPrompt(promptText, defaultVal);
        }
        
        // Vérifier si requis
        if (propDef.required && !value) {
            log("Propriété requise " + propDef.name + " non remplie, utilisation de la valeur par défaut", "warning");
            value = propDef.default_value || "[" + propDef.name + "]";
        }
        
        log("Variable user " + propDef.name + ": \"" + value + "\"");
        return value || propDef.default_value || "";
        
    } catch (error) {
        log("Erreur lors de la collecte de " + propDef.name + ": " + error.message, "error");
        return propDef.default_value || "";
    }
}

/**
 * Collecte une valeur embedded (optionnelle)
 * @param {Object} propDef - Définition de la propriété
 * @returns {Promise<string>} Valeur saisie ou vide
 */
async function collectEmbeddedValue(propDef) {
    try {
        const promptText = propDef.prompt || propDef.name + " (optionnel):";
        const value = await utils.inputPrompt(promptText, "");
        
        log("Variable embedded " + propDef.name + ": \"" + value + "\"");
        return value || "";
        
    } catch (error) {
        log("Erreur lors de la collecte embedded de " + propDef.name + ": " + error.message, "error");
        return "";
    }
}

/**
 * Génère une valeur automatique
 * @param {Object} propDef - Définition de la propriété
 * @returns {string} Valeur générée
 */
function generateAutoValue(propDef) {
    const timestamp = Date.now();
    let value = "";
    
    // Générer selon le nom de la propriété
    if (propDef.name.toLowerCase().includes("id")) {
        value = "ID_" + timestamp;
    } else if (propDef.name.toLowerCase().includes("date")) {
        value = new Date().toISOString().split('T')[0];
    } else if (propDef.name.toLowerCase().includes("time")) {
        value = new Date().toISOString();
    } else {
        value = "AUTO_" + timestamp;
    }
    
    log("Variable auto " + propDef.name + ": \"" + value + "\"");
    return value;
}

// ============================================
// SUBSTITUTION DES VARIABLES
// ============================================

/**
 * Substitue les variables dans le contenu
 * @param {string} content - Contenu avec variables
 * @param {Object} values - Valeurs des variables
 * @returns {string} Contenu avec variables substituées
 */
function substituteVariables(content, values) {
    log("Substitution des variables dans le contenu...");
    
    let result = content;
    let substitutionCount = 0;
    
    for (const [variable, value] of Object.entries(values)) {
        const regex = new RegExp("\\$\\{" + variable + "\\}", 'g');
        const matches = result.match(regex);
        
        if (matches) {
            result = result.replace(regex, value);
            substitutionCount += matches.length;
            log("Variable " + variable + " substituée " + matches.length + " fois");
        }
    }
    
    log("Total: " + substitutionCount + " substitution(s) effectuée(s)");
    return result;
}

/**
 * Extrait les variables d'un contenu
 * @param {string} content - Contenu à analyser
 * @returns {Array} Liste des variables uniques
 */
function extractVariables(content) {
    const regex = /\$\{(\w+)\}/g;
    const variables = new Set();
    let match;
    
    while ((match = regex.exec(content)) !== null) {
        variables.add(match[1]);
    }
    
    const varList = Array.from(variables);
    log(varList.length + " variable(s) trouvée(s): " + varList.join(', '));
    return varList;
}

// ============================================
// GÉNÉRATION DU NOM D'OBJET
// ============================================

/**
 * Génère le nom de l'objet basé sur les valeurs
 * @param {Object} values - Valeurs des variables
 * @param {string} templateName - Nom du template
 * @returns {string} Nom de l'objet
 */
function generateObjectName(values, templateName) {
    // Priorité : nom > objectName > template_timestamp
    if (values.nom) {
        return values.nom;
    } else if (values.objectName) {
        return values.objectName;
    } else {
        const timestamp = new Date().toISOString().replace(/[:.]/g, '-').slice(0, 19);
        return templateName + "_" + timestamp;
    }
}

// ============================================
// CRÉATION DU FICHIER OBJET
// ============================================

/**
 * Crée le fichier objet dans le même dossier que le canvas actif
 * @param {string} content - Contenu du fichier
 * @param {string} objectName - Nom de l'objet
 * @param {Object} activeFile - Fichier actif (canvas)
 * @returns {Promise<Object>} Informations sur le fichier créé
 */
async function createObjectFile(content, objectName, activeFile) {
    log("Création du fichier objet: " + objectName + ".md");
    
    try {
        // Obtenir le dossier du fichier actif
        const activeFolder = activeFile.parent ? activeFile.parent.path : "";
        const filePath = activeFolder ? activeFolder + "/" + objectName + ".md" : objectName + ".md";
        
        // Vérifier si le fichier existe déjà
        const existingFile = app.vault.getAbstractFileByPath(filePath);
        if (existingFile) {
            // Ajouter un suffixe unique
            const timestamp = Date.now();
            const uniqueName = objectName + "_" + timestamp;
            const uniquePath = activeFolder ? activeFolder + "/" + uniqueName + ".md" : uniqueName + ".md";
            
            await app.vault.create(uniquePath, content);
            log("Fichier créé avec nom unique: " + uniqueName + ".md dans " + (activeFolder || "racine"));
            
            return {
                path: uniquePath,
                name: uniqueName,
                file: app.vault.getAbstractFileByPath(uniquePath)
            };
        } else {
            await app.vault.create(filePath, content);
            log("Fichier créé: " + objectName + ".md dans " + (activeFolder || "racine"));
            
            return {
                path: filePath,
                name: objectName,
                file: app.vault.getAbstractFileByPath(filePath)
            };
        }
        
    } catch (error) {
        log("Erreur lors de la création du fichier: " + error.message, "error");
        throw error;
    }
}

// ============================================
// EMBEDDING DANS EXCALIDRAW (MÉTHODE MANUELLE)
// ============================================

/**
 * Génère un fileId unique pour l'embedding
 * @returns {string} FileId unique
 */
function generateFileId() {
    const chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    let result = '';
    for (let i = 0; i < 8; i++) {
        result += chars.charAt(Math.floor(Math.random() * chars.length));
    }
    return result;
}

/**
 * Génère un ID unique pour un élément
 * @returns {string} ID unique
 */
function generateElementId() {
    const chars = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
    let result = '';
    for (let i = 0; i < 10; i++) {
        result += chars.charAt(Math.floor(Math.random() * chars.length));
    }
    return result;
}

/**
 * Ajoute l'embedding manuellement dans le fichier Excalidraw
 * @param {Object} activeFile - Fichier actif
 * @param {Object} newFile - Nouveau fichier créé
 * @returns {Promise<void>}
 */
async function addManualEmbedding(activeFile, newFile) {
    log("Ajout manuel de l'embedding dans le fichier Excalidraw...");
    
    try {
        // Lire le contenu actuel
        let content = await app.vault.read(activeFile);
        
        // Générer un fileId unique
        const fileId = generateFileId();
        log("FileId généré: " + fileId);
        
        // Format correct avec |100%
        const embedEntry = fileId + ": [[" + newFile.name + "|100%]]";
        
        // 1. Ajouter l'entrée dans ## Embedded files
        const embeddedFilesRegex = /## Embedded [Ff]iles\n([\s\S]*?)(?=\n%%|$)/i;
        const embeddedMatch = content.match(embeddedFilesRegex);
        
        if (embeddedMatch) {
            // Ajouter à la section existante
            const updatedSection = embeddedMatch[0] + "\n" + embedEntry;
            content = content.replace(embeddedFilesRegex, updatedSection);
            log("Entrée ajoutée à la section 'Embedded files' existante");
        } else {
            // Créer la section si elle n'existe pas
            const drawingStart = content.indexOf("## Drawing");
            if (drawingStart !== -1) {
                const insertPosition = drawingStart;
                const embeddedSection = "## Embedded Files\n" + embedEntry + "\n\n";
                content = content.slice(0, insertPosition) + embeddedSection + content.slice(insertPosition);
                log("Section 'Embedded Files' créée avec l'entrée");
            } else {
                log("Impossible de trouver la section Drawing", "error");
                throw new Error("Structure Excalidraw invalide");
            }
        }
        
        // 2. Ajouter l'élément image dans le JSON
        const jsonMatch = content.match(/```json\n([\s\S]*?)\n```/);
        if (jsonMatch) {
            try {
                const excalidrawData = JSON.parse(jsonMatch[1]);
                
                // Créer l'élément image
                const imageElement = {
                    "id": generateElementId(),
                    "type": "image",
                    "x": 0,  // Position centrale
                    "y": 0,
                    "width": 300,
                    "height": 200,
                    "angle": 0,
                    "strokeColor": "transparent",
                    "backgroundColor": "transparent",
                    "fillStyle": "solid",
                    "strokeWidth": 2,
                    "strokeStyle": "solid",
                    "roughness": 1,
                    "opacity": 100,
                    "groupIds": [],
                    "frameId": null,
                    "index": "a" + (excalidrawData.elements.length + 1),
                    "roundness": null,
                    "seed": Math.floor(Math.random() * 2000000000),
                    "version": 1,
                    "versionNonce": Math.floor(Math.random() * 2000000000),
                    "isDeleted": false,
                    "boundElements": [],
                    "updated": Date.now(),
                    "link": null,
                    "locked": false,
                    "status": "pending",
                    "fileId": fileId,
                    "scale": [1, 1]
                };
                
                // Ajouter l'élément au tableau
                excalidrawData.elements.push(imageElement);
                
                // Remplacer le JSON dans le contenu
                const newJson = JSON.stringify(excalidrawData, null, "\t");
                content = content.replace(jsonMatch[1], newJson);
                
                log("Élément image ajouté au JSON Excalidraw");
            } catch (jsonError) {
                log("Erreur lors du parsing/modification du JSON: " + jsonError.message, "error");
                // Continuer sans l'élément image si erreur
            }
        }
        
        // Sauvegarder les modifications
        await app.vault.modify(activeFile, content);
        log("Fichier Excalidraw modifié avec succès");
        
        // Note: Le rechargement de la vue n'est pas nécessaire
        // Excalidraw détectera automatiquement les changements
        
    } catch (error) {
        log("Erreur lors de l'embedding manuel: " + error.message, "error");
        throw error;
    }
}

// ============================================
// FONCTION PRINCIPALE
// ============================================

/**
 * Fonction principale du script
 */
async function main() {
    console.log("=".repeat(50));
    console.log("Version: " + SCRIPT_VERSION);  // Log de version
    log("Script " + SCRIPT_NAME + " - Démarrage");
    console.log("=".repeat(50));
    
    try {
        // Vérifier qu'on est dans un fichier actif
        const activeFile = app.workspace.getActiveFile();
        if (!activeFile) {
            throw new Error("Aucun fichier actif");
        }
        
        log("Fichier actif: " + activeFile.path);
        
        // Obtenir la liste des templates
        const templates = await getTemplatesList();
        if (templates.length === 0) {
            throw new Error("Aucun template ProcessMetaLanguage V3 trouvé dans " + TEMPLATES_PATH);
        }
        
        // Sélectionner un template
        const selectedTemplate = await selectTemplate(templates);
        
        // Lire et parser le template
        const templateContent = await app.vault.read(
            app.vault.getAbstractFileByPath(selectedTemplate.path)
        );
        
        // Parser les property_definitions
        const propertyDefs = parsePropertyDefinitions(templateContent);
        
        // Extraire les variables du template
        const variables = extractVariables(templateContent);
        
        // Collecter les valeurs
        const values = await collectVariableValues(propertyDefs, variables);
        
        // Substituer les variables
        const processedContent = substituteVariables(templateContent, values);
        
        // Générer le nom de l'objet
        const objectName = generateObjectName(values, selectedTemplate.name);
        log("Nom de l'objet généré: " + objectName);
        
        // Créer le fichier objet dans le même dossier que le canvas
        const createdFile = await createObjectFile(processedContent, objectName, activeFile);
        
        // Embedding dans Excalidraw (méthode manuelle)
        await addManualEmbedding(activeFile, createdFile);
        
        // Message de succès
        const successMsg = "✅ ProcessMetaLanguage V3\n\n" +
                          "Objet créé: " + createdFile.name + "\n" +
                          "Template: " + selectedTemplate.name + "\n" +
                          "Embedding: Ajouté au canvas\n\n" +
                          "Note: Basculez en vue Excalidraw pour voir l'objet";
        
        new Notice(successMsg, 5000);
        log("Script terminé avec succès");
        
    } catch (error) {
        log("Erreur: " + error.message, "error");
        new Notice("❌ Erreur ProcessMetaLanguage V3:\n" + error.message, 5000);
    }
    
    console.log("=".repeat(50));
    log("Fin du script");
    console.log("=".repeat(50));
}

// Lancer le script
await main();

// <!-- END OF FILE: Embedded-Element-PML-From-Template.md -->