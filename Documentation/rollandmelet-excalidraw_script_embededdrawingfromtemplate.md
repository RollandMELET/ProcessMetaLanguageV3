Directory structure:
└── rollandmelet-excalidraw_script_embededdrawingfromtemplate/
    ├── README.md
    ├── Brouillon de Workflow.md
    ├── embed-object-from-template.md
    ├── plan.md
    ├── README-FR.md
    ├── template-example.md
    └── docs/
        ├── PRD-EN.md
        └── PRD-FR.md


Files Content:

================================================
FILE: README.md
================================================
# Excalidraw Embed from Template Script

## The "Back of the Card" Problem - Solved

This script solves a specific workflow challenge in Obsidian's Excalidraw plugin, inspired by Zsolt's Visual Zettelkasten methodology demonstrated in his videos on [Visual Zettelkasten](https://www.youtube.com/watch?v=o49C8jQIsvs), [Block References](https://www.youtube.com/watch?v=yDZ6v7_OqZE), and [Hybrid Notes](https://www.youtube.com/watch?v=DbeLGGxvKZQ).

### The Problem
In Zsolt's Visual PKM approach, every visual element should have a "back of the card" - a markdown file containing the element's metadata, detailed information, and connections. Previously, creating these embedded objects required:

1. **Exit Excalidraw** - Break your visual flow
2. **Create a new markdown file** - Navigate file explorer  
3. **Apply a template** - Find and copy the right template
4. **Return to Excalidraw** - Context switch back
5. **Manually embed the file** - Drag or use `![[filename]]` syntax

**Result:** 5+ steps, multiple context switches, disrupted creative flow.

### The Solution
With this script: **One keyboard shortcut** creates everything instantly, without leaving Excalidraw.

Press `Cmd+Shift+O` → Select template → Name your object → Done! The embedded object appears immediately in your drawing with its backing markdown file already created.

## Current Version: v1.3.0 (Bilingual)
Released: August 15, 2025

## 🎯 Key Features

### ✨ True Visual PKM Workflow
- Create embedded objects **directly from Excalidraw** - no context switching
- Automatic "back of the card" markdown file generation
- Instant visual feedback - embeds appear immediately
- Perfect for Visual Zettelkasten methodology

### 🌍 Bilingual Support (v1.3.0)
- **Automatic language detection** (EN/FR)
- Uses Obsidian's locale settings
- Seamless experience for international users
- All messages and prompts in your language

### 🎨 Dynamic Template System
- **Interactive template selection** from your `Templates/` folder
- **Category support** via subfolders
- **Recently used templates** (last 5) for quick access
- **Favorite templates** marked with ⭐
- **Built-in fallback template** when no templates available

### 🔄 Smart Duplicate Handling
- Automatic detection of existing filenames
- **Intelligent suggestions**: name(1), name(2), name_v2, name_copy
- Clean interface using `utils.suggester()`
- Custom naming option available

## 📋 Prerequisites

- **Obsidian** v1.5.0 or higher
- **Excalidraw Plugin** v2.14.0 or higher (by Zsolt Viczian)
- `Templates/` folder in your vault (optional but recommended)

## 🚀 Installation

### Via Excalidraw Scripts Menu (Recommended)

1. Open any Excalidraw file in Obsidian
2. Click the **tools icon** in Excalidraw toolbar
3. Navigate to **Scripts** → **Downloaded** → **Install new**
4. Copy the entire content of `embed-object-from-template.md`
5. The script will appear in the "Downloaded" section with a custom cube icon

### Manual Installation

1. Copy `embed-object-from-template.md` to:
   ```
   YourVault/Excalidraw/Scripts/Downloaded/
   ```
2. Restart Obsidian or refresh scripts

## 🎮 Usage

### Basic Workflow

1. **Open** an Excalidraw drawing
2. **Launch** the script:
   - Via Scripts menu → Downloaded → embed-object-from-template
   - Or use your configured keyboard shortcut
3. **Select** a template from the list (or use default)
4. **Name** your workflow object
5. **Done!** Object is created and embedded instantly

### Keyboard Shortcut Setup

1. Settings → Hotkeys
2. Search for "Excalidraw: embed-object-from-template"
3. Assign shortcut (e.g., `Cmd+Shift+O` or `Ctrl+Shift+O`)

### Template Organization

Structure your templates in the `Templates/` folder:

```
Templates/
├── BasicCard.md
├── ProcessStep.md
├── Workflows/
│   ├── SimpleWorkflow.md
│   └── ComplexWorkflow.md
├── Concepts/
│   ├── Definition.md
│   └── Reference.md
└── DataStructure.md
```

Templates are automatically:
- Discovered and listed by category
- Sorted alphabetically
- Remembered after use (recent templates)

## ⚙️ Advanced Configuration

### Template Structure

Templates must be valid Excalidraw files containing:
- YAML header with `excalidraw-plugin: parsed`
- Standard Excalidraw sections
- `${objectName}` variable for dynamic content

### Minimal Template Example

```markdown
---
excalidraw-plugin: parsed
tags: [excalidraw]
---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==

# Text Elements
${objectName}

# Embedded files

# Drawing
```json
{
    "type": "excalidraw",
    "version": 2,
    "source": "https://github.com/zsviczian/obsidian-excalidraw-plugin",
    "elements": [],
    "appState": {
        "theme": "light",
        "viewBackgroundColor": "#ffffff"
    }
}
```
%%
```

## 🎯 Use Cases (Visual PKM)

### Visual Zettelkasten
Create atomic notes with visual representations. Each embedded object becomes a permanent note in your Zettelkasten with both visual and textual dimensions.

### Process Documentation
Build complex workflows visually while maintaining detailed documentation in the backing files. Perfect for standard operating procedures.

### Knowledge Graphs
Construct visual knowledge graphs where each node has rich metadata and connections stored in its markdown file.

### Project Planning
Design project structures visually with each component having detailed specifications in its "back of the card."

## 🔧 Troubleshooting

| Issue | Solution |
|-------|----------|
| Embed doesn't appear | ✅ Fixed in v1.3.0 with automatic toggle |
| "No active file" error | Open an Excalidraw drawing first |
| Templates not found | Check `Templates/` folder exists and contains valid files |
| Duplicate filename | Script automatically suggests alternatives |
| Creation error | Check folder permissions |

## 📊 Technical Architecture

### How It Works

1. **Template Selection**: Interactive menu with memory
2. **Name Input**: User prompt with duplicate detection
3. **File Creation**: Generate from template with variable substitution
4. **Excalidraw Integration**:
   - Generate unique fileId
   - Add to `## Embedded Files` section
   - Insert image element in JSON
   - Set status "saved" for immediate display
5. **Programmatic Toggle**: Force Excalidraw to refresh
6. **Success Notification**: Confirm creation

### The Innovation (v1.3.0)

The script implements multiple refresh strategies to ensure immediate display:
1. Toggle source/preview for Markdown views
2. setState() to force reload
3. File close/reopen via temporary file
4. Obsidian event triggering

This multi-strategy approach ensures compatibility across different Excalidraw states and view modes.

## 📈 Version History

### v1.3.0 (August 15, 2025) - **Current Stable**
- ✅ Bilingual support (EN/FR) with auto-detection
- ✅ Custom SVG icon for script menu
- ✅ Programmatic toggle for immediate display
- ✅ Final resolution of display bug
- ✅ International release ready

### v1.2.0 - v1.2.9
- Dynamic template selection system
- Advanced duplicate handling
- Multiple interface improvements
- Filename/embed synchronization

### v1.0.0
- Initial stable release
- Basic creation with fixed template

## 🌟 Why This Matters

This script bridges the gap between visual thinking and structured note-taking. It enables the Visual PKM methodology promoted by Zsolt without the friction of constant context switching. You can now build complex visual systems while maintaining the detailed metadata and connections that make Obsidian powerful.

## 🤝 Contributing

Contributions are welcome! 

- **Report bugs**: Via [GitHub issues](https://github.com/RollandMELET/EXCALIDRAW_Script_EmbededDrawingFromTemplate/issues)
- **Suggest improvements**: Pull requests accepted
- **Share templates**: Add examples to the Templates folder
- **Join the discussion**: [Obsidian Discord](https://discord.gg/obsidianmd) #excalidraw channel

## 📝 License

MIT License - See LICENSE file for details

## 👥 Credits

- **Rolland MELET** - Script Development & Visual PKM Implementation
- **Claude (Anthropic)** - Development assistance
- **Zsolt Viczian** - Excalidraw Plugin creator & Visual PKM inspiration
- **Obsidian Community** - Feedback and ideas

## 💬 Support

For questions or issues:
- Open an issue on [GitHub](https://github.com/RollandMELET/EXCALIDRAW_Script_EmbededDrawingFromTemplate)
- Contact: rm@360sc.io
- Discord: Find me in the Obsidian Discord #excalidraw channel

---

*Empowering Visual PKM in Obsidian - Create once, think visually, document thoroughly.*

**Version 1.3.0** - Bilingual Edition


================================================
FILE: Brouillon de Workflow.md
================================================
---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠== You can decompress Drawing data with the command palette: 'Decompress current Excalidraw file'. For more info check in plugin settings under 'Saving'


# Excalidraw Data

## Text Elements
## Embedded Files
d6413039388e1fc6acc3ea0a0d2d29637798000f: [[O1]]

f4fe1dc8199c29c3a4b09f5d5ade5111003327f7: [[O2]]

%%
dfaa55707d76668344c8e08686f068b76cc3227b: [[Projets/Projet_Alpha/O4.md]]
## Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.14.0",
	"elements": [
		{
			"id": "48ycW4NZYL13fSdbpTd-3",
			"type": "diamond",
			"x": -526.40234375,
			"y": -450.96484375,
			"width": 200.20703125,
			"height": 224.2265625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"index": "a0",
			"roundness": {
				"type": 2
			},
			"seed": 1365343573,
			"version": 20,
			"versionNonce": 2078515480,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755180884080,
			"link": null,
			"locked": false
		},
		{
			"id": "2gYdsm68ewwOaWDReM1JG",
			"type": "rectangle",
			"x": 4.6796875,
			"y": -394.5625,
			"width": 231.45703125,
			"height": 141.35546875,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"index": "a1",
			"roundness": {
				"type": 3
			},
			"seed": 35111547,
			"version": 20,
			"versionNonce": 1584700520,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755180884080,
			"link": null,
			"locked": false
		},
		{
			"id": "btfsqq21k_MB3RxT3i1Rk",
			"type": "ellipse",
			"x": -206.17578125,
			"y": -278.171875,
			"width": 154.34375,
			"height": 134.6015625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"index": "a2",
			"roundness": {
				"type": 2
			},
			"seed": 987735387,
			"version": 21,
			"versionNonce": 1711259160,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755180884080,
			"link": null,
			"locked": false
		},
		{
			"id": "ca19416030d9e75c",
			"type": "image",
			"x": -712.1411627634117,
			"y": -1301.3937479301394,
			"width": 565.685424949238,
			"height": 212.13203435596427,
			"angle": 0,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 543180903,
			"versionNonce": 1573495271,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755204282436,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "d6413039388e1fc6acc3ea0a0d2d29637798000f",
			"scale": [
				1,
				1
			],
			"version": 48,
			"index": "a3",
			"crop": null
		},
		{
			"id": "047bdd08b2c1cae7",
			"type": "image",
			"x": 781.2716299628713,
			"y": -998.99593887777,
			"width": 565.685424949238,
			"height": 212.13203435596427,
			"angle": 0,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 1741758308,
			"versionNonce": 904803945,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755204222625,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "f4fe1dc8199c29c3a4b09f5d5ade5111003327f7",
			"scale": [
				1,
				1
			],
			"version": 2,
			"index": "a4",
			"crop": null
		},
		{
			"id": "a67f2c2fdd992ebf",
			"type": "image",
			"x": 1314.1143424374904,
			"y": -1042.9299216997879,
			"width": 400,
			"height": 300,
			"angle": 0,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 609038272,
			"versionNonce": 268796071,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755204222625,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "14f4fa53356a77315f5f1bf42a26f57d305baecb",
			"scale": [
				1,
				1
			],
			"version": 2,
			"index": "a5",
			"crop": null
		},
		{
			"id": "cdf20795fc925f30",
			"type": "image",
			"x": 1764.1143424374904,
			"y": -1042.9299216997879,
			"width": 400,
			"height": 300,
			"angle": 0,
			"strokeColor": "transparent",
			"backgroundColor": "transparent",
			"fillStyle": "hachure",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"seed": 445589286,
			"versionNonce": 1242389121,
			"isDeleted": false,
			"boundElements": null,
			"updated": 1755204403619,
			"link": null,
			"locked": false,
			"status": "pending",
			"fileId": "dfaa55707d76668344c8e08686f068b76cc3227b",
			"scale": [
				1,
				1
			]
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 2,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 5,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"currentItemArrowType": "round",
		"scrollX": 1169.8616150434518,
		"scrollY": 2973.9465213348194,
		"zoom": {
			"value": 0.175922
		},
		"currentItemRoundness": "round",
		"gridSize": 20,
		"gridStep": 5,
		"gridModeEnabled": false,
		"gridColor": {
			"Bold": "rgba(217, 217, 217, 0.5)",
			"Regular": "rgba(230, 230, 230, 0.5)"
		},
		"currentStrokeOptions": null,
		"frameRendering": {
			"enabled": true,
			"clip": true,
			"name": true,
			"outline": true
		},
		"objectsSnapModeEnabled": false,
		"activeTool": {
			"type": "selection",
			"customType": null,
			"locked": false,
			"fromSelection": false,
			"lastActiveTool": null
		}
	},
	"files": {}
}
```
%%


================================================
FILE: embed-object-from-template.md
================================================
/*
excalidraw-script-icon: <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M23 18C23 18.75 22.79 19.46 22.42 20.06C22.21 20.42 21.94 20.74 21.63 21C20.93 21.63 20.01 22 19 22C17.78 22 16.69 21.45 15.97 20.59C15.95 20.56 15.92 20.54 15.9 20.51C15.78 20.37 15.67 20.22 15.58 20.06C15.21 19.46 15 18.75 15 18C15 16.74 15.58 15.61 16.5 14.88C17.19 14.33 18.06 14 19 14C20 14 20.9 14.36 21.6 14.97C21.72 15.06 21.83 15.17 21.93 15.28C22.59 16 23 16.95 23 18Z" stroke="#292D32" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path> <path d="M20.4898 17.98H17.5098" stroke="#292D32" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path> <path d="M19 16.52V19.51" stroke="#292D32" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path> <g opacity="0.4"> <path d="M3.16992 7.43994L11.9999 12.5499L20.7699 7.46991" stroke="#292D32" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path> <path d="M12 21.61V12.54" stroke="#292D32" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path> <path d="M21.6106 9.17V14.83C21.6106 14.88 21.6106 14.92 21.6006 14.97C20.9006 14.36 20.0006 14 19.0006 14C18.0606 14 17.1906 14.33 16.5006 14.88C15.5806 15.61 15.0006 16.74 15.0006 18C15.0006 18.75 15.2106 19.46 15.5806 20.06C15.6706 20.22 15.7806 20.37 15.9006 20.51L14.0706 21.52C12.9306 22.16 11.0706 22.16 9.93062 21.52L4.59062 18.56C3.38062 17.89 2.39062 16.21 2.39062 14.83V9.17C2.39062 7.79 3.38062 6.11002 4.59062 5.44002L9.93062 2.48C11.0706 1.84 12.9306 1.84 14.0706 2.48L19.4106 5.44002C20.6206 6.11002 21.6106 7.79 21.6106 9.17Z" stroke="#292D32" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path> </g> </g></svg>
Script Excalidraw pour créer et intégrer des objets depuis un template
Excalidraw Script for creating and embedding objects from templates
Version 1.3.0 - Bilingual Edition
Author: Rolland MELET & Claude Code
Date: 2025-08-15
Changelog:
- v1.3.0: Bilingual support (EN/FR) + Custom icon + Programmatic toggle for instant display
- v1.2.9: Fix critical - Sync filename/embed entry  
- v1.2.8: Fix immediate display (status "saved" + operation order)
- v1.2.7: Simplified two-step approach for duplicates
- v1.2.6: Fix "false" title and allow direct name input
- v1.2.5: Use utils.suggester() for elegant selection menu
- v1.2.4: Fix - Enter now correctly accepts default suggestion
- v1.2.3: Message correction (Tab doesn't work with inputPrompt)
- v1.2.2: Tab attempt (non-functional - API limitation)
- v1.2.1: Add duplicate handling with automatic name suggestion
- v1.2.0: Add dynamic template selection
- v1.0.0: Initial stable version
*/

// === CONFIGURATION ===
const TEMPLATES_FOLDER = "Templates";
const DEFAULT_TEMPLATE_NAME = "Embedded-Object-Template";
const STORAGE_KEY = "excalidraw-embed-preferences";

// === INTERNATIONALIZATION ===
// Detect user language
const getUserLanguage = () => {
    const lang = moment?.locale() || 
                 navigator.language || 
                 app.locale || 
                 'en';
    return lang.startsWith('fr') ? 'fr' : 'en';
};

const lang = getUserLanguage();

// Translation dictionary
const i18n = {
    en: {
        selectTemplate: "Select a template",
        objectName: "Workflow object name:",
        defaultTemplate: "📦 Default template (built-in)",
        fileExists: "already exists. Choose an option:",
        enterCustomName: "💡 Enter another name...",
        suggestionsAvailable: "Available suggestions:",
        enterNewName: "Enter a new name:",
        cancelled: "Creation cancelled",
        noActiveFile: "No active file",
        noTemplateFound: "No template found in Templates/. Using default template.",
        templateSelected: "Template selected:",
        defaultSelected: "Default template selected",
        fileCreatedAs: "File created as",
        objectCreated: "✅ Object",
        createdWith: "created with",
        error: "Error",
        errorCreatingFile: "Unable to create file",
        errorReadingTemplate: "Error reading template. Using default.",
        invalidTemplate: "Selected template is not a valid Excalidraw file.",
        scriptStarting: "Excalidraw Embed Script v1.3.0 - Starting",
        scanningTemplates: "Scanning templates folder",
        templatesFolder: "Templates folder",
        notFound: "not found",
        fileEmbed: "File embed created:",
        errorFileStructure: "Error: File structure not recognized",
        attemptingToggle: "Attempting programmatic toggle...",
        viewDetected: "Excalidraw/Markdown view detected, toggling...",
        toSourceMode: "Switching to source mode",
        toPreviewMode: "Back to preview mode",
        usingSetState: "Using setState to refresh",
        toggleViaReopen: "Toggle via close/reopen file",
        triggeringEvent: "Triggering file-open event",
        toggleComplete: "Programmatic toggle complete",
        toggleError: "Error during programmatic toggle:",
        refreshError: "Error during fallback refresh:",
        suggesterUnavailable: "utils.suggester unavailable, using fallback",
        nameAlreadyExists: "(name already exists)"
    },
    fr: {
        selectTemplate: "Sélectionnez un template",
        objectName: "Nom de l'objet de workflow:",
        defaultTemplate: "📦 Template par défaut (intégré)",
        fileExists: "existe déjà. Choisissez une option :",
        enterCustomName: "💡 Saisir un autre nom...",
        suggestionsAvailable: "Suggestions disponibles :",
        enterNewName: "Entrez un nouveau nom :",
        cancelled: "Création annulée",
        noActiveFile: "Aucun fichier actif",
        noTemplateFound: "Aucun template trouvé dans le dossier Templates/. Utilisation du template par défaut.",
        templateSelected: "Template sélectionné :",
        defaultSelected: "Template par défaut sélectionné",
        fileCreatedAs: "Fichier créé sous le nom",
        objectCreated: "✅ Objet",
        createdWith: "créé avec",
        error: "Erreur",
        errorCreatingFile: "Impossible de créer le fichier",
        errorReadingTemplate: "Erreur lors de la lecture du template. Utilisation du template par défaut.",
        invalidTemplate: "Le template sélectionné n'est pas un fichier Excalidraw valide.",
        scriptStarting: "Script Excalidraw Embed v1.3.0 - Démarrage",
        scanningTemplates: "Scan du dossier Templates",
        templatesFolder: "Dossier Templates",
        notFound: "non trouvé",
        fileEmbed: "Fichier embed créé :",
        errorFileStructure: "Erreur: Structure du fichier non reconnue",
        attemptingToggle: "Tentative de toggle programmatique...",
        viewDetected: "Vue Excalidraw/Markdown détectée, toggle en cours...",
        toSourceMode: "Passage en mode source",
        toPreviewMode: "Retour en mode preview",
        usingSetState: "Utilisation de setState pour rafraîchir",
        toggleViaReopen: "Toggle via fermeture/réouverture du fichier",
        triggeringEvent: "Déclenchement d'un événement file-open",
        toggleComplete: "Toggle programmatique terminé",
        toggleError: "Erreur lors du toggle programmatique:",
        refreshError: "Erreur lors du rafraîchissement fallback:",
        suggesterUnavailable: "utils.suggester non disponible, utilisation du fallback",
        nameAlreadyExists: "(nom déjà existant)"
    }
};

// Helper function to get translation
const t = (key) => i18n[lang][key] || i18n['en'][key];

// Default template (fallback)
const TEMPLATE_DEFAULT = `---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==


# Text Elements

# Embedded files

# Drawing
\`\`\`json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin",
	"elements": [],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#000000",
		"currentItemBackgroundColor": "transparent",
		"currentItemFillStyle": "hachure",
		"currentItemStrokeWidth": 1,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 1,
		"currentItemFontSize": 20,
		"currentItemTextAlign": "left",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"scrollX": 0,
		"scrollY": 0,
		"zoom": {
			"value": 1
		},
		"gridSize": null,
		"gridColor": {
			"Bold": "#C9C9C9FF",
			"Regular": "#EDEDEDFF"
		}
	},
	"files": {}
}
\`\`\`
%%`;

// Generate unique file ID
function generateFileId() {
    const chars = 'abcdef0123456789';
    let result = '';
    for (let i = 0; i < 40; i++) {
        result += chars[Math.floor(Math.random() * chars.length)];
    }
    return result;
}

// Load saved preferences
function loadPreferences() {
    try {
        const stored = localStorage.getItem(STORAGE_KEY);
        if (stored) {
            return JSON.parse(stored);
        }
    } catch (e) {
        console.error("Error loading preferences:", e);
    }
    return {
        lastUsedTemplate: null,
        recentTemplates: []
    };
}

// Save preferences
function savePreferences(prefs) {
    try {
        localStorage.setItem(STORAGE_KEY, JSON.stringify(prefs));
    } catch (e) {
        console.error("Error saving preferences:", e);
    }
}

// Update recent templates
function updateRecentTemplates(templatePath, prefs) {
    prefs.recentTemplates = prefs.recentTemplates.filter(t => t !== templatePath);
    prefs.recentTemplates.unshift(templatePath);
    prefs.recentTemplates = prefs.recentTemplates.slice(0, 5);
    prefs.lastUsedTemplate = templatePath;
    savePreferences(prefs);
}

// Scan Templates folder for available files
async function getAvailableTemplates() {
    const templates = [];
    
    try {
        const templatesFolder = app.vault.getAbstractFileByPath(TEMPLATES_FOLDER);
        
        if (!templatesFolder) {
            console.log(`${t('templatesFolder')} ${t('notFound')}`);
            return templates;
        }
        
        const allFiles = app.vault.getFiles();
        
        for (const file of allFiles) {
            if (file.path.startsWith(TEMPLATES_FOLDER + "/")) {
                if (file.extension === "md" || file.extension === "excalidraw") {
                    const content = await app.vault.read(file);
                    if (content.includes("excalidraw-plugin: parsed") || file.extension === "excalidraw") {
                        const relativePath = file.path.substring(TEMPLATES_FOLDER.length + 1);
                        const category = relativePath.includes("/") ? 
                            relativePath.substring(0, relativePath.lastIndexOf("/")) : "";
                        
                        templates.push({
                            name: file.basename,
                            path: file.path,
                            category: category,
                            displayName: category ? `${category}/${file.basename}` : file.basename
                        });
                    }
                }
            }
        }
        
        templates.sort((a, b) => {
            if (a.category !== b.category) {
                return a.category.localeCompare(b.category);
            }
            return a.name.localeCompare(b.name);
        });
        
    } catch (e) {
        console.error(`${t('error')} ${t('scanningTemplates')}:`, e);
    }
    
    return templates;
}

// Show template selection menu
async function selectTemplate() {
    const prefs = loadPreferences();
    const templates = await getAvailableTemplates();
    
    const options = [];
    const templateMap = {};
    
    // Add recent templates first
    if (prefs.recentTemplates.length > 0) {
        const recentTemplates = [];
        for (const recentPath of prefs.recentTemplates) {
            const template = templates.find(t => t.path === recentPath);
            if (template) {
                const recentOption = `⭐ ${template.displayName}`;
                recentTemplates.push(recentOption);
                templateMap[recentOption] = template;
            }
        }
        
        if (recentTemplates.length > 0) {
            options.push(...recentTemplates);
            options.push("───────────────");
        }
    }
    
    // Add all templates
    for (const template of templates) {
        const option = template.displayName;
        options.push(option);
        templateMap[option] = template;
    }
    
    // Add default template option
    if (options.length > 0) {
        options.push("───────────────");
    }
    options.push(t('defaultTemplate'));
    
    // If no templates available, use default directly
    if (templates.length === 0 && prefs.recentTemplates.length === 0) {
        new Notice(t('noTemplateFound'));
        return null;
    }
    
    // Show selection menu
    let selectedOption;
    try {
        if (typeof utils !== 'undefined' && utils.suggester) {
            selectedOption = await utils.suggester(
                options,
                options,
                false,
                t('selectTemplate')
            );
        } else {
            const numberedOptions = options.map((opt, idx) => 
                opt.startsWith("───") ? opt : `${idx + 1}. ${opt}`
            ).join("\n");
            
            const choice = await utils.inputPrompt(
                `${t('selectTemplate')}:\n\n${numberedOptions}\n\n:`
            );
            
            if (choice && !isNaN(choice)) {
                const index = parseInt(choice) - 1;
                if (index >= 0 && index < options.length && !options[index].startsWith("───")) {
                    selectedOption = options[index];
                }
            }
        }
    } catch (e) {
        console.error(`${t('error')}:`, e);
        return null;
    }
    
    if (!selectedOption) {
        return null;
    }
    
    if (selectedOption === t('defaultTemplate')) {
        return { isDefault: true };
    }
    
    if (selectedOption.startsWith("───")) {
        return null;
    }
    
    const cleanOption = selectedOption.startsWith("⭐ ") ? 
        selectedOption.substring(2) : selectedOption;
    
    const selectedTemplate = templateMap[selectedOption] || templateMap[cleanOption];
    
    if (selectedTemplate) {
        updateRecentTemplates(selectedTemplate.path, prefs);
        return selectedTemplate;
    }
    
    return null;
}

// Get template content
async function getTemplateContent(templateInfo) {
    if (templateInfo.isDefault) {
        return TEMPLATE_DEFAULT;
    }
    
    try {
        const templateFile = app.vault.getAbstractFileByPath(templateInfo.path);
        if (templateFile) {
            const content = await app.vault.read(templateFile);
            if (!content.includes("excalidraw-plugin: parsed")) {
                new Notice(t('invalidTemplate'));
                return TEMPLATE_DEFAULT;
            }
            return content;
        }
    } catch (e) {
        console.error(`${t('errorReadingTemplate')}:`, e);
        new Notice(t('errorReadingTemplate'));
    }
    
    return TEMPLATE_DEFAULT;
}

// Get current view center
function getViewCenter(excalidrawContent) {
    try {
        const appStateMatch = excalidrawContent.match(/"appState":\s*{([^}]*)}/);
        if (appStateMatch) {
            const appStateStr = `{${appStateMatch[1]}}`;
            const scrollXMatch = appStateStr.match(/"scrollX":\s*([-\d.]+)/);
            const scrollYMatch = appStateStr.match(/"scrollY":\s*([-\d.]+)/);
            const zoomMatch = appStateStr.match(/"zoom":\s*{[^}]*"value":\s*([\d.]+)/);
            
            if (scrollXMatch && scrollYMatch) {
                const scrollX = parseFloat(scrollXMatch[1]);
                const scrollY = parseFloat(scrollYMatch[1]);
                const zoom = zoomMatch ? parseFloat(zoomMatch[1]) : 1;
                
                const viewportWidth = 800;
                const viewportHeight = 600;
                
                const centerX = -scrollX + (viewportWidth / 2) / zoom;
                const centerY = -scrollY + (viewportHeight / 2) / zoom;
                
                return { x: centerX, y: centerY };
            }
        }
    } catch (e) {
        // Return default values on error
    }
    
    return { x: 0, y: 0 };
}

// Main script
(async () => {
    console.log(t('scriptStarting'));
    
    // Step 1: Select template
    const templateInfo = await selectTemplate();
    
    if (!templateInfo) {
        new Notice(t('cancelled'));
        return;
    }
    
    // Display selected template
    if (templateInfo.isDefault) {
        console.log(t('defaultSelected'));
    } else {
        console.log(`${t('templateSelected')} ${templateInfo.displayName}`);
    }
    
    // Step 2: Get object name
    let objectName = await utils.inputPrompt(t('objectName'));
    if (!objectName) {
        new Notice(t('cancelled'));
        return;
    }
    
    // Get active file
    const activeFile = app.workspace.getActiveFile();
    if (!activeFile) {
        new Notice(t('noActiveFile'));
        return;
    }
    
    // Function to generate unique filename
    async function getUniqueFileName(baseName, folder) {
        let fileName = `${baseName}.md`;
        let filePath = folder ? `${folder.path}/${fileName}` : fileName;
        
        if (!app.vault.getAbstractFileByPath(filePath)) {
            return { name: baseName, fileName: fileName, filePath: filePath };
        }
        
        const choices = [];
        
        // Generate suggestions - Windows style: name(1), name(2)
        for (let i = 1; i <= 3; i++) {
            const suggestion = `${baseName}(${i})`;
            const suggestionPath = folder ? 
                `${folder.path}/${suggestion}.md` : 
                `${suggestion}.md`;
            
            if (!app.vault.getAbstractFileByPath(suggestionPath)) {
                choices.push(suggestion);
                if (choices.length >= 2) break;
            }
        }
        
        // Version style: name_v2
        const versionName = `${baseName}_v2`;
        const versionPath = folder ? 
            `${folder.path}/${versionName}.md` : 
            `${versionName}.md`;
        if (!app.vault.getAbstractFileByPath(versionPath)) {
            choices.push(versionName);
        }
        
        // Copy style: name_copy
        const copyName = `${baseName}_copy`;
        const copyPath = folder ? 
            `${folder.path}/${copyName}.md` : 
            `${copyName}.md`;
        if (!app.vault.getAbstractFileByPath(copyPath)) {
            choices.push(copyName);
        }
        
        choices.push(t('enterCustomName'));
        
        // Simplified approach: Selection menu without free input
        let selected;
        try {
            if (typeof utils !== 'undefined' && utils.suggester) {
                const displayLabels = choices.map(choice => {
                    if (choice === t('enterCustomName')) {
                        return choice;
                    }
                    return `✓ ${choice}`;
                });
                
                selected = await utils.suggester(
                    displayLabels,
                    choices,
                    false,
                    `"${baseName}.md" ${t('fileExists')}`
                );
            } else {
                console.log(t('suggesterUnavailable'));
                selected = choices[0];
                new Notice(`${t('fileCreatedAs')} "${selected}.md" ${t('nameAlreadyExists')}`);
            }
        } catch (e) {
            console.error(`${t('error')} suggester:`, e);
            selected = choices[0];
        }
        
        if (!selected) {
            return null;
        }
        
        if (selected === t('enterCustomName')) {
            let customName = await utils.inputPrompt(
                `"${baseName}.md" ${t('fileExists')}\n\n` +
                `${t('suggestionsAvailable')} ${choices.slice(0, -1).join(", ")}\n\n` +
                `${t('enterNewName')}`,
                baseName + "_new"
            );
            
            if (!customName) {
                return null;
            }
            
            return await getUniqueFileName(customName, folder);
        }
        
        const selectedFileName = `${selected}.md`;
        const selectedFilePath = folder ? 
            `${folder.path}/${selectedFileName}` : 
            selectedFileName;
        
        return { 
            name: selected, 
            fileName: selectedFileName, 
            filePath: selectedFilePath 
        };
    }
    
    // Get parent folder and unique filename
    const folder = activeFile.parent;
    const fileInfo = await getUniqueFileName(objectName, folder);
    
    if (!fileInfo) {
        new Notice(t('cancelled'));
        return;
    }
    
    const finalObjectName = fileInfo.name;
    const newFileName = fileInfo.fileName;
    const newFilePath = fileInfo.filePath;
    
    try {
        // Create embed file FIRST
        const templateContent = await getTemplateContent(templateInfo);
        const content = templateContent.replace(/\${objectName}/g, finalObjectName);
        
        let newFile;
        try {
            newFile = await app.vault.create(newFilePath, content);
            console.log(`${t('fileEmbed')} ${newFilePath}`);
        } catch (createError) {
            console.error(`${t('errorCreatingFile')}:`, createError);
            new Notice(`${t('error')}: ${t('errorCreatingFile')} "${newFileName}". ${createError.message}`);
            return;
        }
        
        // Wait for file indexing
        await new Promise(resolve => setTimeout(resolve, 200));
        
        // Generate unique ID for embed
        const fileId = generateFileId();
        
        // Read current Excalidraw file content
        let excalidrawContent = await app.vault.read(activeFile);
        
        // Parse drawing JSON
        const drawingMatch = excalidrawContent.match(/## Drawing\n```json\n([\s\S]*?)\n```/);
        if (!drawingMatch) {
            new Notice(t('errorFileStructure'));
            return;
        }
        
        const drawingData = JSON.parse(drawingMatch[1]);
        
        // Calculate position - centered in current view
        const viewCenter = getViewCenter(excalidrawContent);
        let x = viewCenter.x - 200;
        let y = viewCenter.y - 150;
        
        // Cascade offset if embeds already exist
        if (drawingData.elements && drawingData.elements.length > 0) {
            const embedElements = drawingData.elements.filter(el => el.type === "image" && el.fileId);
            if (embedElements.length > 0) {
                const offset = (embedElements.length % 5) * 30;
                x += offset;
                y += offset;
            }
        }
        
        // Create image element for embed with status "saved"
        const imageElement = {
            id: generateFileId().substring(0, 16),
            type: "image",
            x: x,
            y: y,
            width: 400,
            height: 300,
            angle: 0,
            strokeColor: "transparent",
            backgroundColor: "transparent",
            fillStyle: "hachure",
            strokeWidth: 1,
            strokeStyle: "solid",
            roughness: 1,
            opacity: 100,
            groupIds: [],
            frameId: null,
            roundness: null,
            seed: Math.floor(Math.random() * 2000000000),
            versionNonce: Math.floor(Math.random() * 2000000000),
            isDeleted: false,
            boundElements: null,
            updated: Date.now(),
            link: null,
            locked: false,
            status: "saved",
            fileId: fileId,
            scale: [1, 1]
        };
        
        // Add element to drawing
        drawingData.elements = drawingData.elements || [];
        drawingData.elements.push(imageElement);
        
        // Manage Embedded Files section
        const embedEntry = `${fileId}: [[${finalObjectName}|100%]]`;
        
        const embeddedFilesRegex = /## Embedded Files\n([\s\S]*?)(?=\n%%|$)/;
        const embeddedFilesMatch = excalidrawContent.match(embeddedFilesRegex);
        
        if (embeddedFilesMatch) {
            let existingContent = embeddedFilesMatch[1].trim();
            
            const newContent = existingContent ? 
                `${existingContent}\n${embedEntry}` : 
                embedEntry;
            
            excalidrawContent = excalidrawContent.replace(
                embeddedFilesRegex, 
                `## Embedded Files\n${newContent}\n`
            );
        } else {
            const textElementsIndex = excalidrawContent.indexOf("## Text Elements");
            const drawingIndex = excalidrawContent.indexOf("## Drawing");
            const percentIndex = excalidrawContent.indexOf("%%");
            
            let insertPosition;
            
            if (percentIndex > -1 && percentIndex < drawingIndex) {
                insertPosition = percentIndex;
            } else if (drawingIndex > -1) {
                insertPosition = drawingIndex;
            } else {
                return;
            }
            
            excalidrawContent = 
                excalidrawContent.slice(0, insertPosition) + 
                `## Embedded Files\n${embedEntry}\n\n` +
                excalidrawContent.slice(insertPosition);
        }
        
        // Replace drawing JSON
        const newDrawingJson = JSON.stringify(drawingData, null, "\t");
        excalidrawContent = excalidrawContent.replace(
            /## Drawing\n```json\n[\s\S]*?\n```/,
            `## Drawing\n\`\`\`json\n${newDrawingJson}\n\`\`\``
        );
        
        // Save modifications
        await app.vault.modify(activeFile, excalidrawContent);
        
        // Force save to disk
        await app.vault.adapter.write(activeFile.path, excalidrawContent);
        
        // Wait for save to complete
        await new Promise(resolve => setTimeout(resolve, 1000));
        
        // PROGRAMMATIC TOGGLE to force Excalidraw to reload embeds
        try {
            console.log(t('attemptingToggle'));
            
            const activeLeaf = app.workspace.activeLeaf;
            if (activeLeaf && activeLeaf.view) {
                const view = activeLeaf.view;
                
                // Method 1: If it's a Markdown/Excalidraw view
                if (view.getViewType && (view.getViewType() === "markdown" || view.getViewType() === "excalidraw")) {
                    console.log(t('viewDetected'));
                    
                    const currentState = view.getState ? view.getState() : null;
                    
                    // Switch to source mode
                    if (view.setMode) {
                        await view.setMode('source');
                        console.log(t('toSourceMode'));
                        await new Promise(resolve => setTimeout(resolve, 200));
                        
                        // Back to preview mode
                        await view.setMode('preview');
                        console.log(t('toPreviewMode'));
                    } else if (view.setState && currentState) {
                        console.log(t('usingSetState'));
                        await view.setState(currentState, { history: false });
                    }
                }
                // Method 2: Close and reopen file
                else {
                    console.log(t('toggleViaReopen'));
                    
                    const tempNote = await app.vault.create(`temp-${Date.now()}.md`, "");
                    
                    await activeLeaf.openFile(tempNote);
                    await new Promise(resolve => setTimeout(resolve, 100));
                    
                    await activeLeaf.openFile(activeFile);
                    await new Promise(resolve => setTimeout(resolve, 100));
                    
                    await app.vault.delete(tempNote);
                }
                
                // Method 3: Trigger modification event
                if (app.workspace.trigger) {
                    console.log(t('triggeringEvent'));
                    app.workspace.trigger('file-open', activeFile);
                }
                
                console.log(t('toggleComplete'));
            }
        } catch (e) {
            console.error(t('toggleError'), e);
            
            // Fallback: simple refresh
            try {
                const activeLeaf = app.workspace.activeLeaf;
                if (activeLeaf) {
                    await activeLeaf.openFile(activeFile);
                }
            } catch (e2) {
                console.error(t('refreshError'), e2);
            }
        }
        
        // Success message
        const templateName = templateInfo.isDefault ? 
            t('defaultTemplate') : 
            templateInfo.displayName;
        new Notice(`${t('objectCreated')} "${finalObjectName}" ${t('createdWith')} ${templateName}!`);
        
        console.log(`${t('objectCreated')} ${finalObjectName} (Template: ${templateName})`);
        
    } catch (error) {
        console.error(`${t('error')}:`, error);
        new Notice(`${t('error')}: ${error.message}`);
    }
})();


================================================
FILE: plan.md
================================================
# Plan d'implémentation : Sélection de Template Dynamique

## 🎯 Objectif
Permettre à l'utilisateur de choisir parmi plusieurs templates disponibles lors de la création d'un objet, avec un système de mémorisation et de catégorisation.

## 📋 Étapes d'implémentation

### 1. **Détection et listage des templates**
- Scanner le dossier `Templates/` pour trouver tous les fichiers `.md` et `.excalidraw`
- Créer une fonction `getAvailableTemplates()` qui retourne la liste des templates
- Gérer le cas où le dossier Templates n'existe pas

### 2. **Interface de sélection améliorée**
- Remplacer le template fixe par un système de sélection
- Options d'implémentation :
  - **Option A**: Menu suggérer avec `app.workspace.getSuggestions()` (plus natif Obsidian)
  - **Option B**: Double prompt (1: choisir template, 2: nommer l'objet)
  - **Option C**: Syntaxe spéciale dans le nom (ex: `MonObjet@template1`)

### 3. **Système de template par défaut intelligent**
- Mémoriser le dernier template utilisé dans les settings
- Template "Embedded-Object-Template" comme fallback ultime
- Ordre de priorité :
  1. Template sélectionné par l'utilisateur
  2. Dernier template utilisé (si option activée)
  3. Template par défaut configuré
  4. Template intégré dans le script

### 4. **Catégorisation des templates (optionnel)**
- Support des sous-dossiers dans `Templates/`
- Ex: `Templates/Process/`, `Templates/Data/`, `Templates/UI/`
- Affichage hiérarchique dans le menu de sélection

### 5. **Validation et feedback**
- Vérifier que le template sélectionné est valide (format Excalidraw)
- Message d'erreur clair si template invalide
- Prévisualisation rapide du template (nom + description)

## 🔧 Modifications du code

### Fichiers à modifier :
1. **embed-object-from-template.md** (script principal)
   - Ajouter `getAvailableTemplates()`
   - Modifier le workflow de sélection
   - Implémenter la mémorisation du dernier choix

### Nouvelles fonctions :
```javascript
// Lister les templates disponibles
async function getAvailableTemplates() {
    // Scanner le dossier Templates/
    // Retourner un array d'objets {name, path, category}
}

// Afficher le menu de sélection
async function selectTemplate(templates) {
    // Utiliser utils.suggester() ou utils.inputPrompt()
    // Retourner le template sélectionné
}

// Sauvegarder le dernier template utilisé
function saveLastUsedTemplate(templatePath) {
    // Stocker dans localStorage ou settings
}

// Charger le dernier template utilisé
function getLastUsedTemplate() {
    // Récupérer depuis localStorage ou settings
}
```

## ⚡ Workflow utilisateur final

1. **Raccourci clavier** → Script activé
2. **Menu de sélection** apparaît avec :
   - Templates récents (3-5 derniers)
   - Séparateur
   - Tous les templates disponibles
   - Option "Template par défaut"
3. **Sélection du template**
4. **Saisie du nom** de l'objet
5. **Création et intégration** instantanée

## 🎨 Options d'amélioration future

- **Aperçu du template** : Miniature ou description
- **Templates favoris** : Marquer certains templates comme favoris
- **Raccourcis directs** : Assigner des raccourcis à des templates spécifiques
- **Import de templates** : Depuis GitHub ou URL externe
- **Création de template** : À partir d'un objet existant

## ✅ Tests à prévoir

1. Dossier Templates vide
2. Dossier Templates inexistant
3. Templates invalides (non-Excalidraw)
4. Sélection rapide (mémorisation)
5. Annulation de la sélection
6. Performance avec beaucoup de templates (50+)

## 📊 Priorités d'implémentation

### Phase 1 - MVP (Version 1.1.0)
- [x] Listage basique des templates
- [x] Menu de sélection simple
- [x] Template par défaut comme fallback

### Phase 2 - Améliorations (Version 1.2.0)
- [ ] Mémorisation du dernier template
- [ ] Templates récents
- [ ] Validation des templates

### Phase 3 - Avancé (Version 1.3.0)
- [ ] Catégorisation
- [ ] Templates favoris
- [ ] Aperçu des templates

## 🔐 Considérations techniques

### Stockage des préférences
- **Option 1**: LocalStorage d'Obsidian
  ```javascript
  localStorage.setItem('excalidraw-last-template', templatePath);
  ```
- **Option 2**: Plugin settings (nécessite modification du plugin)
- **Option 3**: Fichier de configuration `.excalidraw-script-config.json`

### Performance
- Cache de la liste des templates (rafraîchi toutes les 5 minutes)
- Chargement asynchrone des templates
- Limite de 100 templates affichés simultanément

### Compatibilité
- Maintenir la rétrocompatibilité avec l'ancienne méthode
- Support des anciens formats de templates
- Migration automatique des anciens settings


================================================
FILE: README-FR.md
================================================
[Binary file]


================================================
FILE: template-example.md
================================================
// <!-- START OF FILE: template-example.md -->
// FILENAME: template-example.md
// Version: 1.0.0
// Date: 2025-08-14 15:40
// Author: Rolland MELET & Claude Code
// Description: Exemple de template pour les objets de workflow

# ${objectName}

## 📋 Description
[Décrire brièvement la fonction de cet objet dans le workflow]

## ⚙️ Paramètres

### Entrées
- **Input 1** : [Type] - [Description]
- **Input 2** : [Type] - [Description]

### Sorties
- **Output 1** : [Type] - [Description]
- **Output 2** : [Type] - [Description]

## 🔧 Configuration
```yaml
# Configuration spécifique à l'objet
param1: value1
param2: value2
```

## 🔗 Connexions
- **Prérequis** : [Liste des objets qui doivent être exécutés avant]
- **Déclenche** : [Liste des objets déclenchés après cet objet]

## 📊 Métriques
- **Temps d'exécution moyen** : 
- **Taux de succès** : 
- **Volume traité** : 

## 🚨 Gestion des erreurs
- **Erreur 1** : [Description] → [Action]
- **Erreur 2** : [Description] → [Action]

## 📝 Notes d'implémentation
[Notes techniques, considérations particulières, limitations connues]

## 🏷️ Tags
#workflow #${objectName} #processus

---
*Dernière mise à jour : {{date}} par {{author}}*

// <!-- END OF FILE: template-example.md -->


================================================
FILE: docs/PRD-EN.md
================================================
# Product Requirements Document
## Excalidraw Embed from Template Script

**Version:** 1.3.0  
**Date:** August 15, 2025  
**Author:** Rolland MELET & Claude (Anthropic)  
**Status:** Production Ready - Bilingual Edition

## 1. Executive Summary

This script enables seamless creation of embedded Excalidraw objects with backing markdown files ("back of the card") directly from within Excalidraw, following Zsolt Viczian's Visual PKM methodology.

### Core Problem
Visual PKM requires every visual element to have detailed metadata in a backing file. Previously, this required 5+ manual steps and constant context switching between Excalidraw and Obsidian's file explorer.

### Solution
One keyboard shortcut creates both the visual embed and its backing markdown file instantly, without leaving Excalidraw.

## 2. User Stories

### Primary User Story
**As a** Visual PKM practitioner using Obsidian and Excalidraw,  
**I want to** create embedded objects with backing files using a single keyboard shortcut,  
**So that** I can maintain my visual flow while building comprehensive knowledge systems.

### Secondary User Stories

**Template Selection**  
**As a** user with different object types,  
**I want to** choose from multiple templates when creating objects,  
**So that** I can quickly create structured objects for different purposes.

**Language Support**  
**As an** international user,  
**I want** the script to detect and use my language automatically,  
**So that** I can work in my native language without configuration.

## 3. Functional Requirements

### 3.1 Core Functionality
- **Single-action creation**: One keyboard shortcut triggers the entire workflow
- **In-context execution**: All operations happen within Excalidraw view
- **Immediate visual feedback**: Embedded object appears instantly
- **Automatic file generation**: Backing markdown file created with template content

### 3.2 Template System
- **Dynamic discovery**: Scan `Templates/` folder for available templates
- **Category support**: Organize templates in subfolders
- **Recent templates**: Remember last 5 used templates
- **Fallback template**: Built-in default when no templates available
- **Variable substitution**: Replace `${objectName}` in templates

### 3.3 User Interface
- **Interactive selection**: Clean menu for template choice
- **Smart suggestions**: Propose alternatives for duplicate names
- **Bilingual support**: Auto-detect language (EN/FR)
- **Custom icon**: Distinctive cube icon in scripts menu

### 3.4 File Management
- **Smart positioning**: Center embed in current viewport
- **Cascade offset**: Offset multiple embeds for visibility
- **Duplicate handling**: Automatic name suggestions (name(1), name_v2, etc.)
- **Same folder creation**: Files created in active drawing's folder

## 4. Technical Specifications

### 4.1 Excalidraw Integration
```javascript
// Required modifications to Excalidraw file:
1. Add entry to "## Embedded Files" section
   Format: fileId: [[ObjectName|100%]]

2. Insert image element in JSON with:
   - type: "image"
   - fileId: unique 40-character hash
   - status: "saved"
   - Centered position based on viewport

3. Force refresh via programmatic toggle
```

### 4.2 Language Detection
```javascript
const getUserLanguage = () => {
    const lang = moment?.locale() || 
                 navigator.language || 
                 app.locale || 
                 'en';
    return lang.startsWith('fr') ? 'fr' : 'en';
};
```

### 4.3 Refresh Strategy
Multiple fallback methods ensure immediate display:
1. Toggle source/preview mode
2. setState() for view refresh
3. File close/reopen sequence
4. Obsidian event triggering

## 5. Non-Functional Requirements

### Performance
- **Creation time**: < 2 seconds from trigger to visible embed
- **Template scanning**: Cached for repeated use
- **Memory usage**: Minimal footprint, cleanup after execution

### Compatibility
- **Obsidian**: v1.5.0+
- **Excalidraw Plugin**: v2.14.0+
- **Platform**: Cross-platform (Windows, Mac, Linux)

### Usability
- **Zero configuration**: Works out of the box
- **Intuitive workflow**: Follows Obsidian conventions
- **Error recovery**: Graceful handling with user feedback

## 6. Success Metrics

### Adoption Metrics
- Script installations via Excalidraw menu
- GitHub stars and forks
- Community feedback and contributions

### Usage Metrics
- Objects created per session
- Template variety usage
- Error rate < 1%

### Quality Metrics
- Immediate display success rate > 99%
- User-reported bugs resolved within 48 hours
- Community template contributions

## 7. Implementation Phases

### Phase 1: Core Functionality ✅
- Basic object creation
- Fixed template support
- Manual refresh required

### Phase 2: Template System ✅
- Dynamic template selection
- Category organization
- Recent templates memory

### Phase 3: Polish & International ✅
- Bilingual support (EN/FR)
- Custom icon
- Programmatic refresh
- Production stability

### Phase 4: Future Vision
- Multi-language support (ES, DE, etc.)
- Template sharing marketplace
- AI-suggested templates
- Batch object creation

## 8. Technical Debt & Known Limitations

### Current Limitations
- Language support limited to EN/FR
- Template variables limited to `${objectName}`
- Maximum 5 recent templates remembered

### Technical Debt
- Refresh mechanism uses multiple fallbacks (could be simplified when Excalidraw API improves)
- Template validation is basic (checks for header only)

## 9. Security Considerations

- No external API calls
- All operations local to vault
- No sensitive data handling
- Template content sandboxed

## 10. Documentation Requirements

### User Documentation
- README.md in English and French
- Installation guide with screenshots
- Template creation guide
- Troubleshooting section

### Developer Documentation
- Code comments in English
- JSDoc for all functions
- Architecture diagram
- Contribution guidelines

## 11. Release Criteria

### v1.3.0 Release Checklist
- ✅ Bilingual support functional
- ✅ Custom icon displayed
- ✅ Programmatic refresh working
- ✅ Documentation in both languages
- ✅ GitHub repository prepared
- ✅ Community announcement drafted

## 12. Support & Maintenance

### Support Channels
- GitHub Issues for bug reports
- Discord #excalidraw channel for discussions
- Direct email for critical issues

### Maintenance Plan
- Monthly review of issues
- Quarterly compatibility testing
- Annual major version consideration

---

*This PRD represents the current state of the Excalidraw Embed from Template Script, focusing on solving the "back of the card" workflow challenge in Visual PKM.*


================================================
FILE: docs/PRD-FR.md
================================================

## **PRD : Création et Intégration Dynamique d'Objets de Workflow dans Excalidraw pour Obsidian**

**Version :** 1.3
**Date :** 2025-08-15
**Auteur :** SuperAssistant (sur la base des besoins et de l'analyse technique de l'utilisateur)
**Mise à jour :** Version stable avec affichage immédiat des embeds
**Sources d'Information :**
*   **Dépôt GitHub du Plugin Excalidraw :** [https://github.com/zsviczian/obsidian-excalidraw-plugin](https://github.com/zsviczian/obsidian-excalidraw-plugin)
*   **Documentation de l'API Excalidraw Automate :** [https://zsviczian.github.io/obsidian-excalidraw-plugin/](https://zsviczian.github.io/obsidian-excalidraw-plugin/)
* **Dépôt GitHub de Templater Obsidian Plugin**  https://github.com/SilentVoid13/Templater

### 1. Descriptif Précis du Rendu de l'Opération (Le "Quoi")

L'utilisateur se trouve dans une vue Excalidraw active dans Obsidian.

#### Version 1.0 (Actuelle)
1.  En utilisant un raccourci clavier unique et dédié (ex: `Cmd+Option+O`), une boîte de dialogue apparaît, lui demandant de nommer un nouvel "objet de workflow".
2.  L'utilisateur saisit un nom (ex: "Étape 1 - Authentification") et valide.
3.  **Immédiatement et sans aucune autre action manuelle**, les événements suivants se produisent de manière atomique :
    *   Un nouvel élément visuel apparaît sur le canevas Excalidraw. Cet élément est l'intégration ("embed") d'un nouveau fichier. **Il doit être positionné au centre de la vue visible de l'utilisateur à l'instant de la création.**
    *   Dans l'explorateur de fichiers d'Obsidian, un nouveau fichier Markdown (ex: `Étape 1 - Authentification.md`) est créé.
    *   Ce nouveau fichier est impérativement localisé dans le **même dossier** que le dessin Excalidraw actif.
    *   Le contenu de ce nouveau fichier est pré-rempli à partir d'un template spécifié (ex: `Templates/MonTemplateObjet.md`).

#### Version 1.2 (Nouvelle - Sélection de Template)
1.  En utilisant un raccourci clavier unique et dédié (ex: `Cmd+Option+O`), **un menu de sélection de templates apparaît**.
2.  **L'utilisateur choisit parmi les templates disponibles** :
    *   Liste des templates du dossier `Templates/` (fichiers `.md` et `.excalidraw`)
    *   Templates récemment utilisés (3-5 derniers)
    *   Option "Template par défaut" (Embedded-Object-Template)
    *   Support des catégories si sous-dossiers présents
3.  Une fois le template sélectionné, l'utilisateur saisit le nom de l'objet.
4.  Le reste du processus reste identique à la version 1.0.

Le processus doit être fluide, rapide (moins de 2 secondes) et ne doit laisser aucun artefact. L'utilisateur doit pouvoir enchaîner cette opération plusieurs fois pour construire rapidement son diagramme.

### 2. Contexte et Objectif Stratégique (Le "Pourquoi")

Cette fonctionnalité est la pierre angulaire d'un système de **"Visual Product Management"** dont l'objectif final est de transformer des workflows visuels en spécifications techniques (PRD) exploitables par une IA (projet 360SmartConnect).

Chaque "objet" sur le canevas doit être une entité "intelligente" possédant deux facettes :
*   **Une facette visuelle :** Un pictogramme ou une forme simple sur le canevas Excalidraw.
*   **Une facette "données" :** Un fichier Markdown structuré contenant tous les paramètres de l'objet, suivant le principe de la "fiche" (back of the card).

L'objectif est de réduire la friction entre l'idéation (le dessin) et la spécification (le texte), pour ensuite automatiser la génération de documentation via des outils comme le script "Excalidraw Writing Machine".

### 3. User Stories

#### User Story 1 (Version de base)
**En tant que** Product/Process Designer,
**Je veux** utiliser un raccourci clavier pour créer instantanément un nouvel objet de workflow à partir d'un template et l'intégrer au centre de ma vue sur le canevas Excalidraw actif,
**Afin de** construire visuellement mes processus de manière fluide, tout en générant automatiquement la structure de données sous-jacente nécessaire pour une documentation et une automatisation futures.

#### User Story 2 (Sélection de template)
**En tant que** Product/Process Designer,
**Je veux** pouvoir choisir parmi différents templates disponibles lors de la création d'un objet,
**Afin de** créer rapidement des objets de différents types (Process, Data, Interface, etc.) avec la structure appropriée.

#### User Story 3 (Mémorisation)
**En tant que** utilisateur régulier,
**Je veux** que le système mémorise mes templates récemment utilisés,
**Afin de** gagner du temps en accédant rapidement à mes templates favoris sans parcourir toute la liste.

### 4. Analyse Technique de l'Intégration Manuelle

L'observation d'une intégration manuelle réussie révèle la mécanique interne précise d'Excalidraw :

1.  Une nouvelle section **`## Embedded Files`** est créée dans le fichier Markdown du dessin, positionnée entre `## Text Elements` et `## Drawing`.
2.  Cette section contient un manifeste liant un **token de signature (hash)** au chemin du fichier intégré.
    *   Exemple : `de59b03237d1e12e71b4fdb15566266f919fe31c: [[Chemin/Vers/Objet.md]]`
3.  Dans la section `## Drawing`, le JSON de la scène est modifié pour inclure un nouvel élément de type **`image`**.
4.  Cet élément `image` contient une clé **`"fileId"`** dont la valeur est le **token de signature** correspondant, assurant ainsi la liaison entre l'objet visuel et sa source.

Toute solution automatisée devra impérativement reproduire cette structure en trois parties (ajout à la section `Embedded Files`, ajout de l'élément `image` au JSON, et synchronisation du `fileId`).

### 5. Brief sur les Tentatives et Échecs

Les multiples tentatives ont révélé des instabilités et des conflits de contexte entre Templater et l'API Excalidraw Automate (`ea`).

*   **Tentative 1 : API Excalidraw directe (`addEmbeddable`)**
    *   **Échec :** Les fonctions se sont révélées inexistantes ou ont échoué en raison d'un contexte non défini (`targetView not set`). L'API, appelée depuis Templater, est instable et n'arrive pas à effectuer la triple modification (section `Embedded Files`, JSON, `fileId`) requise.

*   **Tentative 2 : Contournement par `app.vault.append()`**
    *   **Succès partiel :** Le fichier a été créé au bon endroit et le dessin modifié pour y ajouter `![[...]]`.
    *   **Échec :** Le rafraîchissement de la vue pour qu'Excalidraw interprète le lien `![[...]]` et génère la structure complète (section `Embedded Files`, `fileId`) a échoué. Les fonctions de l'API pour forcer ce rafraîchissement se sont révélées tout aussi instables.

### 6. Apprentissages Clés

1.  **L'API Excalidraw Automate (`ea`) est une boîte noire instable** lorsqu'elle est pilotée par un script Templater externe. Ses fonctions ne sont pas fiables pour des opérations complexes comme l'intégration.
2.  **La manipulation directe du fichier est plus robuste**, mais incomplète si elle ne reproduit pas la structure précise d'Excalidraw (JSON + section `Embedded Files`).
3.  **Les fonctions de base d'Obsidian (`app.workspace`, `app.vault`) sont la seule source de vérité fiable** pour manipuler les fichiers et connaître le contexte.

### 7. Nouvelles Fonctionnalités (Version 1.2)

#### 7.1 Sélection Dynamique de Templates

**Exigences fonctionnelles :**
1. **Découverte automatique** : Scanner le dossier `Templates/` pour lister tous les fichiers compatibles
2. **Interface de sélection** : Menu déroulant ou suggérer pour choisir le template
3. **Templates récents** : Afficher les 3-5 derniers templates utilisés en haut de la liste
4. **Catégorisation** : Support des sous-dossiers (ex: `Templates/Process/`, `Templates/Data/`)
5. **Template par défaut** : Fallback sur "Embedded-Object-Template" si aucun template sélectionné

**Exigences techniques :**
- Utiliser `app.vault.getFiles()` ou `app.vault.getMarkdownFiles()` pour lister les templates
- Stocker les préférences dans `localStorage` ou un fichier de configuration
- Validation du format Excalidraw avant utilisation
- Cache de la liste des templates pour optimiser les performances

#### 7.2 Mémorisation et Personnalisation

**Fonctionnalités :**
1. **Dernier template utilisé** : Option pour réutiliser automatiquement le dernier template
2. **Templates favoris** : Marquer certains templates comme favoris
3. **Raccourcis personnalisés** : Assigner des raccourcis à des templates spécifiques

**Stockage des préférences :**
```javascript
{
  "lastUsedTemplate": "Templates/Process/Step.md",
  "recentTemplates": ["Template1.md", "Template2.md"],
  "favoriteTemplates": ["MainTemplate.md"],
  "templateShortcuts": {
    "Cmd+Shift+1": "Templates/Process.md",
    "Cmd+Shift+2": "Templates/Data.md"
  }
}
```

### 8. Orientations Techniques Possibles (Historique)

1.  **Option A (La plus Robuste) : Script Excalidraw Pur**
    *   **Concept :** Abandonner Templater comme "pilote". Le script doit être un **script du moteur Excalidraw natif**, placé dans le dossier des scripts d'Excalidraw (voir `ea-scripts/` sur le GitHub).
    *   **Avantages :** Le script s'exécutera dans un contexte 100% Excalidraw. L'objet `ea` sera stable et correctement initialisé. Il n'y aura plus de conflit. L'API `ea` devrait alors être capable d'effectuer correctement la triple modification requise.
    *   **Défis :** Il faudra ré-implémenter la création de fichier depuis un template en utilisant l'API de base d'Obsidian, mais c'est la garantie d'une solution stable et propre.

2.  **Option B (L'Ingénierie Inverse) : Script Templater de Haute Précision**
    *   **Concept :** Créer un script Templater qui **simule manuellement et parfaitement** ce que fait Excalidraw en interne.
    *   **Séquence :**
        1.  Créer le nouveau fichier `Objet.md` (partie maîtrisée).
        2.  Lire le contenu du fichier `Brouillon.md` actif.
        3.  Générer un token de signature (hash) unique.
        4.  Créer un nouvel objet `image` en JSON avec ce `fileId`.
        5.  Insérer cet objet `image` dans le JSON de la section `## Drawing`.
        6.  Insérer la ligne `hash: [[Chemin/Objet.md]]` dans la section `## Embedded Files` (en la créant si elle n'existe pas).
        7.  Ré-écrire la totalité du fichier `Brouillon.md` avec ces modifications.
        8.  Forcer le rafraîchissement de la vue avec `leaf.openFile()`.
    *   **Avantages :** Reste dans l'écosystème Templater.
    *   **Défis :** Extrêmement complexe, fragile aux mises à jour du plugin Excalidraw, et risque de corruption de fichiers. **Non recommandé.**

### 9. Roadmap de Développement

#### Phase 1 - Version 1.0.0 ✅ (Complétée)
- Création d'objets avec template fixe
- Positionnement intelligent au centre
- Format `|100%` pour affichage correct
- Sauvegarde forcée et rafraîchissement

#### Phase 2 - Version 1.2.0 ✅ (Complétée)
- Sélection dynamique de templates
- Interface de sélection intuitive
- Templates récents et mémorisation
- Support des catégories
- Gestion intelligente des doublons

#### Phase 3 - Version 1.3.0 ✅ (Complétée - Version Stable)
- Toggle programmatique pour affichage immédiat
- Résolution définitive du bug d'affichage
- Multiples méthodes de rafraîchissement
- Optimisation des performances
- Version de production stable

#### Phase 4 - Version 2.0.0 (Vision long terme)
- Création de templates depuis objets existants
- Synchronisation des templates entre vaults
- Templates partagés (GitHub, communauté)
- IA pour suggestion de templates contextuels


