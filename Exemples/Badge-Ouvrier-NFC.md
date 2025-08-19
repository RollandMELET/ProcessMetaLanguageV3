---
excalidraw-plugin: parsed
tags:
  - workflow-objet
  - processmetalanguage
  - objet
  - avatar-360sc
---
# Name

Badge Ouvrier NFC
# Type

OBJET

## 📋 Description
Badge NFC permettant l'identification et la traçabilité des ouvriers sur chantier. Gère l'accès aux zones sécurisées et le pointage des heures de travail.

## ⚙️ Paramètres Avatar 360SmartConnect

### Propriétés Obligatoires
- **name** : "Badge Ouvrier NFC" (nom descriptif)
- **avatarType** : "/api/avatar_types/badge-ouvrier" (type badge ouvrier)

### Propriétés Configurées
- **serialNumber** : Mode Embedded (numéro unique par badge)
- **company** : "/api/companies/chantier-a" (société du chantier)
- **status** : 1 (actif par défaut)

## 🔧 Configuration
```yaml
# Configuration Avatar 360SmartConnect
avatar_config:
  type: "badge-ouvrier"
  company: "chantier-a"
  auto_status: true
  tracking_enabled: true
  
# Propriétés métier
properties:
  zone_access: ["zone-a", "zone-b"]
  shift_tracking: true
  emergency_contact: true
```

## 🚨 Gestion des erreurs
- **Badge non reconnu** : Vérifier numéro série → Réenregistrer dans 360SC
- **Accès refusé zone** : Contrôler permissions utilisateur → Mettre à jour droits
- **Lecture NFC échouée** : Badge défectueux → Remplacer badge

## 📝 Notes d'implémentation
- Badge compatible NFC Type 2 (ISO14443A)
- Portée lecture : 2-4cm maximum
- Durée de vie batterie : 2 ans en usage normal
- Résistant projections d'eau (IP54)

## 🏷️ Tags
#badge-nfc #ouvrier #tracabilite #acces #pointage

# Excalidraw Data

## Text Elements
Badge Ouvrier NFC ^JwlF0Ue7

%%
## Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.14.0",
	"elements": [
		{
			"id": "shape-1",
			"type": "rectangle",
			"x": -150,
			"y": -50,
			"width": 300,
			"height": 100,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1e90ff",
			"fillStyle": "hachure",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"seed": 12345,
			"version": 3,
			"versionNonce": 1846050995,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "JwlF0Ue7"
				}
			],
			"updated": 1755269391089,
			"link": null,
			"locked": false,
			"index": "a0",
			"groupIds": [],
			"frameId": null,
			"roundness": null,
			"customData": {
				"avatar360sc_template": {
					"type": "Avatar360SC_Template",
					"data": {
						"templateType": "Avatar360SC",
						"version": "1.0",
						"created": "2025-08-19T10:30:00.000Z",
						"properties": {
							"name": {
								"mode": "template",
								"value": "Badge Ouvrier NFC",
								"required": true
							},
							"avatarType": {
								"mode": "template",
								"value": "/api/avatar_types/badge-ouvrier",
								"required": true
							},
							"serialNumber": {
								"mode": "embedded",
								"defaultValue": "BDG-",
								"required": false
							},
							"company": {
								"mode": "template",
								"value": "/api/companies/chantier-a",
								"required": false
							},
							"status": {
								"mode": "template",
								"value": 1,
								"required": false
							}
						}
					},
					"timestamp": 1724058600000
				}
			}
		},
		{
			"id": "JwlF0Ue7",
			"type": "text",
			"x": -73.7679443359375,
			"y": -10,
			"width": 147.535888671875,
			"height": 20,
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
			"roundness": null,
			"seed": 379966365,
			"version": 6,
			"versionNonce": 885973645,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755612577723,
			"link": null,
			"locked": false,
			"text": "Badge Ouvrier NFC",
			"rawText": "Badge Ouvrier NFC",
			"fontSize": 16,
			"fontFamily": 5,
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "shape-1",
			"originalText": "Badge Ouvrier NFC",
			"autoResize": true,
			"lineHeight": 1.25
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
		"scrollX": 232.625,
		"scrollY": 216.6640625,
		"zoom": {
			"value": 2
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