# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 🎯 Objectif Principal du Projet

Ce projet ProcessMetaLanguage V3 vise à créer un système de création d'objets Excalidraw embeddés avec templates pour l'intégration avec la plateforme 360SmartConnect. L'objectif est de transformer des workflows visuels en spécifications techniques exploitables via le principe "back of the card" de Zsolt Viczian.

## 🎯 BESOINS PRIORITAIRES À ACCOMPLIR

### 1. Script "Embedded-Element-PML-From-Template"
**Objectif** : Créer un script Excalidraw qui permet d'embedder des éléments à partir de templates avec ajustements utilisateur.

**Conditions de succès** :
- ✅ Fichier embedded créé au même endroit que le fichier principal
- ✅ Nom du fichier = nom de l'objet saisi par l'utilisateur
- ✅ Le dessin du fichier embedded apparaît sur le canvas
- ✅ Position conservée lors du toggle Excalidraw/Markdown

### 2. Guide de création de templates
**Objectif** : Documenter pas-à-pas comment créer des templates compatibles avec le script.

## 📁 Chemins Critiques

### Répertoires Principaux
- **Projet principal** : `/Users/rollandmelet/Library/CloudStorage/GoogleDrive-rm@360sc.io/Mon Drive/OBSIDIAN/CHATTERS/002 - Projets/PERSO/ProcessMetaLanguageV3`
- **Coffre de test** : `/Users/rollandmelet/Développement/Projets/ProcessMetaLanguage/VaultTestObsidian/PML-Beta-Test-v2`

### Répertoires Techniques
- **Scripts Excalidraw** : `/PML-Beta-Test-v2/Excalidraw/Scripts/`
- **Templates** : `/PML-Beta-Test-v2/Templates/`
- **Documentation** : `./Documentation/`

## 🔧 Développement du Script Embedded-Element-PML-From-Template

### Inspiration de Base
Le script doit s'inspirer fortement de `embed-object-from-template.md` v1.3.0 disponible dans `./Documentation/rollandmelet-excalidraw_script_embededdrawingfromtemplate.md`

### Architecture du Script

```javascript
// Structure de base (inspirée du script existant)
const ea = ExcalidrawAutomate;
ea.reset();

// 1. Scanner les templates disponibles
async function getAvailableTemplates() {
    const templates = [];
    const templatesFolder = app.vault.getAbstractFileByPath("Templates");
    
    if (!templatesFolder) return templates;
    
    const allFiles = app.vault.getFiles();
    for (const file of allFiles) {
        if (file.path.startsWith("Templates/") && file.extension === "md") {
            const content = await app.vault.read(file);
            if (content.includes("excalidraw-plugin: parsed")) {
                templates.push({
                    name: file.basename,
                    path: file.path
                });
            }
        }
    }
    return templates;
}

// 2. Sélection interactive du template
async function selectTemplate() {
    const templates = await getAvailableTemplates();
    const options = templates.map(t => t.name);
    
    const selected = await utils.suggester(
        options,
        options,
        false,
        "Sélectionnez un template"
    );
    
    return templates.find(t => t.name === selected);
}

// 3. Création et embedding
async function createEmbeddedObject() {
    const template = await selectTemplate();
    if (!template) return;
    
    const objectName = await utils.inputPrompt("Nom de l'objet:");
    if (!objectName) return;
    
    // Lire le template
    const templateContent = await app.vault.read(
        app.vault.getAbstractFileByPath(template.path)
    );
    
    // Remplacer les variables
    const content = templateContent.replace(/\${objectName}/g, objectName)
                                   .replace(/\${nom}/g, objectName);
    
    // Créer le fichier
    const activeFile = app.workspace.getActiveFile();
    const folder = activeFile.parent;
    const newFilePath = `${folder.path}/${objectName}.md`;
    
    const newFile = await app.vault.create(newFilePath, content);
    
    // Générer fileId unique
    const fileId = generateFileId();
    
    // Ajouter à Embedded Files et JSON (voir section suivante)
}

// Fonction utilitaire pour générer fileId
function generateFileId() {
    const chars = 'abcdef0123456789';
    let result = '';
    for (let i = 0; i < 40; i++) {
        result += chars[Math.floor(Math.random() * chars.length)];
    }
    return result;
}
```

### Mécanisme d'Embedding Excalidraw

Le script doit reproduire la structure d'embedding d'Excalidraw :

1. **Ajouter dans la section `## Embedded Files`** :
   ```
   fileId: [[ObjectName]]
   ```

2. **Ajouter un élément image dans le JSON** :
   ```javascript
   const imageElement = {
       id: generateFileId().substring(0, 16),
       type: "image",
       x: viewCenter.x - 200,
       y: viewCenter.y - 150,
       width: 400,
       height: 300,
       // ... autres propriétés standard
       status: "saved",  // CRITIQUE pour affichage immédiat
       fileId: fileId,
       scale: [1, 1]
   };
   ```

3. **Toggle programmatique pour affichage immédiat** :
   ```javascript
   // Stratégie multi-niveaux pour forcer l'affichage
   try {
       const activeLeaf = app.workspace.activeLeaf;
       if (activeLeaf?.view) {
           // Méthode 1: Toggle source/preview
           await activeLeaf.view.setMode('source');
           await new Promise(resolve => setTimeout(resolve, 200));
           await activeLeaf.view.setMode('preview');
       }
   } catch (e) {
       // Fallback: Réouverture du fichier
       await activeLeaf.openFile(activeFile);
   }
   ```

## 📋 Guide de Création de Templates

### Structure Obligatoire d'un Template

Chaque template doit respecter cette structure :

```markdown
---
excalidraw-plugin: parsed
tags: [processmetalanguage, template, avatar-360sc]

# Métadonnées du Template (pour BackOfCard)
template_type: "avatar"
template_version: "1.0.0"
processmetalanguage_version: "3.0"

# Propriétés Avatar 360SmartConnect
property_definitions:
  nom:
    source: "user"
    required: true
    prompt: "Nom de l'avatar:"
    
  avatarType:
    source: "template"
    required: true
    value: "/api/avatar_types/badge-ouvrier"
    
  serialNumber:
    source: "embedded"
    required: false
    prompt: "Numéro de série:"
    
  company:
    source: "template"
    value: "/api/companies/360smartconnect"
    
  status:
    source: "default"
    default_value: 1
---

==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==

# ${nom}

> **Type d'objet**: Avatar 360SmartConnect  
> **Template**: ${template_type}  

## 📋 Propriétés Avatar

| Propriété | Valeur |
|-----------|--------|
| **Nom** | ${nom} |
| **Type** | ${avatarType} |
| **Numéro de série** | ${serialNumber} |
| **Société** | ${company} |
| **Statut** | ${status} |

# Excalidraw Data

## Text Elements
${nom} ^uniqueTextId

## Embedded files

## Drawing
```json
{
    "type": "excalidraw",
    "version": 2,
    "source": "https://github.com/zsviczian/obsidian-excalidraw-plugin",
    "elements": [
        // Éléments visuels du template
    ],
    "appState": {
        // Configuration de l'état de l'application
    },
    "files": {}
}
```
%%
```

### Variables Supportées dans les Templates

| Variable | Description | Exemple |
|----------|-------------|---------|
| `${nom}` | Nom de l'objet saisi par l'utilisateur | "Badge Ouvrier NFC" |
| `${objectName}` | Alias de `${nom}` | "Badge Ouvrier NFC" |
| `${template_type}` | Type du template | "avatar" |
| `${avatarType}` | Type d'avatar 360SC | "/api/avatar_types/123" |
| `${serialNumber}` | Numéro de série | "BDG-2025-001" |
| `${company}` | Société propriétaire | "/api/companies/456" |
| `${status}` | Statut de l'avatar | 1 |

### Modes de Configuration des Propriétés

- **`"user"`** : Valeur saisie par l'utilisateur lors de la création
- **`"template"`** : Valeur fixe définie dans le template
- **`"embedded"`** : Valeur saisie pour chaque instance
- **`"auto"`** : Valeur générée automatiquement par 360SmartConnect
- **`"default"`** : Valeur par défaut

## 🔗 API 360SmartConnect V2

### Objet Avatar (Structure Principale)

L'objet `Avatar` est l'entité centrale de l'API 360SmartConnect :

```json
{
    "id": "integer (readOnly)",
    "name": "string (requis)",
    "serialNumber": "string",
    "avatarType": "IRI string (obligatoire)",
    "company": "IRI string",
    "status": "integer",
    "parent": "IRI string",
    "children": ["array of IRI (readOnly)"],
    "properties": ["array of IRI (readOnly)"],
    "groups": ["array of IRI"],
    "users": ["array of IRI"]
}
```

### Format IRI (Internationalized Resource Identifier)

Les relations dans l'API utilisent des IRI au format :
- `"/api/avatar_types/{id}"` - Référence vers un AvatarType
- `"/api/companies/{id}"` - Référence vers une Company
- `"/api/avatars/{id}"` - Référence vers un Avatar parent

### Propriétés Obligatoires pour Avatar

1. **`name`** (string) - Nom descriptif de l'avatar
2. **`avatarType`** (IRI) - OBLIGATOIRE - Lien vers le type d'avatar

### Structure BackOfCard pour 360SmartConnect

Dans le template, inclure dans le frontmatter YAML :

```yaml
# Configuration Avatar 360SmartConnect
avatar_360sc:
  properties:
    name:
      mode: "embedded"
      required: true
    avatarType:
      mode: "template"
      value: "/api/avatar_types/badge-ouvrier"
      required: true
    serialNumber:
      mode: "embedded"
      required: false
    company:
      mode: "template"
      value: "/api/companies/chantier-a"
    status:
      mode: "template"
      value: 1
```

## ⚙️ Commandes de Développement

### Installation et Test du Script

1. **Copier le script** dans le répertoire Scripts :
   ```
   cp script.md /Users/rollandmelet/Développement/Projets/ProcessMetaLanguage/VaultTestObsidian/PML-Beta-Test-v2/Excalidraw/Scripts/
   ```

2. **Assigner un raccourci clavier** dans Obsidian :
   - Settings → Hotkeys
   - Chercher "Excalidraw: nom-du-script"
   - Assigner `Cmd+Shift+O` (ou autre)

3. **Tester le script** :
   - Ouvrir un fichier Excalidraw dans le coffre de test
   - Utiliser le raccourci clavier
   - Vérifier la création du fichier embedded
   - Contrôler l'affichage sur le canvas

### Validation des Templates

Pour vérifier qu'un template est valide :

1. **Frontmatter obligatoire** :
   ```yaml
   ---
   excalidraw-plugin: parsed
   ---
   ```

2. **Structure Excalidraw Data** :
   - Section `## Text Elements`
   - Section `## Embedded files`
   - Section `## Drawing` avec JSON valide

3. **Variables définies** :
   - Utiliser `${nom}` ou `${objectName}` dans le texte
   - Définir les propriétés dans `property_definitions`

### Debug et Troubleshooting

1. **Console JavaScript** : Utiliser `console.log()` dans le script
2. **Vérification Embedded Files** : Contrôler la section après création
3. **Status "saved"** : S'assurer que les images ont `status: "saved"`
4. **FileId unique** : Vérifier que chaque embed a un ID de 40 caractères

## 🧠 Gestion de la Mémoire et Base de Connaissances

### Stratégie de Préservation des Apprentissages

**CRITIQUE** : Pour éviter la perte de connaissances entre sessions :

1. **Utiliser Memory Bank MCP** pour sauvegarder :
   - Solutions aux problèmes techniques rencontrés
   - Améliorations apportées aux scripts
   - Nouvelles découvertes sur l'API 360SmartConnect

2. **Format REX (Retour d'Expérience)** :
   ```markdown
   # REX : [Titre du Problème]
   - **Problème** : Description concise
   - **Impact** : Effet sur le workflow
   - **Solution** : Étapes de résolution
   - **Leçon** : Point clé à retenir
   ```

3. **Mise à jour de CLAUDE.md** : Enrichir ce fichier avec les nouvelles découvertes

## 📚 Références et Fichiers Importants

### Scripts de Référence
- `./Documentation/rollandmelet-excalidraw_script_embededdrawingfromtemplate.md` - Script v1.3.0 complet
- Script existant : système bilingue, gestion des doublons, toggle programmatique

### Templates d'Exemple
- `./Documentation/template-objet-backofcard.md` - Template complet pour objets 360SC
- `./Exemples/Badge-Ouvrier-NFC.md` - Exemple d'objet Avatar fonctionnel

### Documentation API
- `./Documentation/API 360SmartConnect V2.md` - Spécifications complètes de l'API
- `./Documentation/Script-Creation-Template-Avatar.md` - Guide pour templates Avatar

### Ressources Excalidraw
- GitHub : https://github.com/zsviczian/obsidian-excalidraw-plugin
- API : https://zsviczian.github.io/obsidian-excalidraw-plugin/API/introduction.html

## ⚠️ Règles Critiques

### Développement du Script

1. **TOUJOURS s'inspirer** du script `embed-object-from-template.md` existant
2. **Générer des fileId uniques** : 40 caractères hexadécimaux
3. **Status "saved"** : Obligatoire pour affichage immédiat des embeds
4. **Toggle programmatique** : Implémenter 4 stratégies de fallback
5. **Gestion des doublons** : Proposer des noms alternatifs automatiques

### Format des Templates

1. **Frontmatter YAML** : `excalidraw-plugin: parsed` obligatoire
2. **Variables** : Utiliser `${nom}` et `${objectName}` de façon interchangeable
3. **Structure JSON** : Respecter le format Excalidraw standard
4. **IRI 360SC** : Format `/api/resource_type/id` pour les relations

### Intégration 360SmartConnect

1. **Propriétés obligatoires** : `name` et `avatarType` minimum
2. **Format IRI** : Toujours utiliser des chemins absolus `/api/...`
3. **BackOfCard** : Inclure métadonnées dans le frontmatter YAML
4. **Modes de configuration** : Respecter auto/template/embedded/user/default

### Règle d'Or : RESTER SIMPLE

- Ne pas sur-complexifier l'implémentation
- Utiliser les patterns éprouvés du script existant
- Tester fréquemment dans le coffre de test
- Documenter chaque modification dans Memory Bank

---

**Note importante** : Ce fichier CLAUDE.md est conçu pour permettre aux futures instances de Claude Code de reprendre efficacement le travail sur ce projet. Il doit être mis à jour à chaque découverte ou amélioration significative.