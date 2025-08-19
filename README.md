<!-- START OF FILE: README.md -->
# FILENAME: README.md
# Version: 1.0.0
# Date: 2025-08-19 22:30
# Author: Rolland MELET & Claude Code
# Description: Documentation complète du projet ProcessMetaLanguage V3

# Changelog:
# - v1.0.0: Création de la documentation complète du projet PML V3

# ProcessMetaLanguage V3 (PML V3)

## 🎯 Vue d'ensemble

ProcessMetaLanguage V3 est un système de templating avancé pour Excalidraw dans Obsidian, permettant de créer des éléments réutilisables avec des variables dynamiques. Il automatise la création d'objets Excalidraw personnalisés à partir de templates prédéfinis.

### Caractéristiques principales

- ✨ **Templates dynamiques** : Création d'objets Excalidraw avec variables substituables
- 🔄 **Embedding automatique** : Insertion directe dans le canvas actif
- 📝 **Types de variables multiples** : user, template, embedded, auto
- 🎨 **Compatible Excalidraw** : Intégration native avec le plugin Obsidian
- 📊 **Extensible** : Architecture modulaire pour futurs développements

## 📦 Installation

### Prérequis

1. **Obsidian** avec le plugin **Excalidraw** installé et configuré
2. Structure de dossiers suivante dans votre vault :
   ```
   VotreVault/
   ├── Templates/        # Dossier pour les templates PML
   ├── Excalidraw/
   │   └── Scripts/     # Dossier pour les scripts Excalidraw
   ```

### Installation du script

1. Copier le fichier `Scripts/Embedded-Element-PML-From-Template.md` dans votre dossier `Excalidraw/Scripts/`
2. Redémarrer Obsidian ou recharger les scripts Excalidraw
3. Le script apparaîtra dans le menu des scripts Excalidraw

## 🚀 Utilisation rapide

### 1. Créer un template

Créer un fichier dans le dossier `Templates/` avec la structure PML V3 :

```yaml
---
processmetalanguage_version: "3.0"
template_type: "badge"
property_definitions:
  nom:
    source: "user"
    prompt: "Nom de la personne:"
    required: true
  entreprise:
    source: "template"
    default_value: "360SmartConnect"
---

# Badge ${nom}

Entreprise: ${entreprise}
```

### 2. Utiliser le script

1. Ouvrir un canvas Excalidraw
2. Lancer le script `Embedded-Element-PML-From-Template`
3. Sélectionner un template
4. Remplir les variables demandées
5. L'objet est créé et embedded automatiquement

## 📚 Documentation détaillée

### Structure d'un template PML V3

Un template PML V3 contient deux parties principales :

#### 1. Front matter YAML

```yaml
---
processmetalanguage_version: "3.0"  # Version du système PML
template_type: "type_objet"          # Type de template (badge, card, etc.)
property_definitions:                # Définitions des variables
  variable_name:
    source: "user|template|embedded|auto"
    prompt: "Question à poser"
    required: true|false
    default_value: "valeur par défaut"
    options: ["option1", "option2"]  # Pour listes déroulantes
---
```

#### 2. Contenu avec variables

Utiliser la syntaxe `${variable}` pour insérer des variables :

```markdown
# Titre ${titre}

Description: ${description}

## Drawing
\`\`\`json
{
  "elements": [...],
  "customData": {
    "name": "${nom}"
  }
}
\`\`\`
```

### Types de sources de variables

| Source | Description | Comportement |
|--------|-------------|--------------|
| `user` | Demandée à l'utilisateur | Popup de saisie lors de la création |
| `template` | Valeur fixe du template | Utilise `default_value` |
| `embedded` | Optionnelle, pour liens | Popup optionnel |
| `auto` | Générée automatiquement | ID, timestamp, date selon le nom |

### Exemples de variables auto

- `${id}` → `ID_1755634567890`
- `${date}` → `2025-01-19`
- `${time}` → `2025-01-19T15:30:45.123Z`
- `${anything_else}` → `AUTO_1755634567890`

## ⚠️ Limitations connues

### Redimensionnement des embeddings

**Les objets embedded ne peuvent pas être redimensionnés directement dans le canvas hôte.** C'est une limitation du plugin Excalidraw.

**Workaround :**
1. Cmd+Clic sur l'objet pour ouvrir le fichier source
2. Redimensionner dans le fichier source
3. Les changements sont automatiquement reflétés

Voir `LIMITATIONS-EMBEDDING.md` pour plus de détails.

## 🔧 Configuration

### Paramètres du script

Dans le fichier du script, vous pouvez modifier :

```javascript
const TEMPLATES_PATH = "Templates";  // Dossier des templates
const SCRIPT_VERSION = "3.4.0";     // Version actuelle
```

### Structure des fichiers créés

Les objets créés sont sauvegardés dans le même dossier que le canvas actif :
```
Canvas-Folder/
├── Mon-Canvas.md        # Canvas Excalidraw
├── ObjetCree1.md       # Objet embedded créé
├── ObjetCree2.md       # Autre objet créé
└── ...
```

## 📊 Versions

### v3.4.0 (Stable actuelle)
- ✅ Embedding fonctionnel avec éléments visibles
- ✅ Création dans le même dossier que le canvas
- ✅ Support complet des 4 types de variables
- ✅ Logging détaillé avec version

### Historique
- v3.3.0 : Correction du chemin de création
- v3.2.x : Corrections API utils.suggester
- v3.1.0 : Remplacement yesNoPrompt
- v3.0.x : Versions initiales avec corrections syntaxe

## 🛠️ Développement

### Structure du projet

```
ProcessMetaLanguageV3/
├── README.md                        # Ce fichier
├── Scripts/
│   └── Embedded-Element-PML-From-Template.md
├── Templates/                       # Templates d'exemple
├── Documentation/                   # Docs techniques
├── Exemples/                       # Fichiers de test
└── PLAN-DEVELOPPEMENT.md           # Roadmap future
```

### Contribution

Les contributions sont bienvenues ! Voir `PLAN-DEVELOPPEMENT.md` pour la roadmap.

## 📄 Licence

Projet développé par Rolland MELET avec l'assistance de Claude Code.

## 🔗 Liens utiles

- [Plugin Excalidraw](https://github.com/zsviczian/obsidian-excalidraw-plugin)
- [Documentation Obsidian](https://obsidian.md)
- [360SmartConnect](https://360smartconnect.com)

---

*Documentation mise à jour le 2025-01-19*
*Version du script : 3.4.0*
<!-- END OF FILE: README.md -->