---
excalidraw-plugin: parsed
tags: [processmetalanguage, template, badge, test]

# Métadonnées ProcessMetaLanguage V3
template_type: "badge"
template_version: "3.0.0"
processmetalanguage_version: "3.0"
template_created: "2025-01-19"
template_author: "ProcessMetaLanguage V3 - Test"

# Configuration des Propriétés
property_definitions:
  nom:
    source: "user"
    required: true
    prompt: "Nom du badge:"
    description: "Nom descriptif du badge"
  
  type_badge:
    source: "user"
    required: true
    prompt: "Type de badge:"
    options: ["NFC", "QR Code", "RFID", "Magnétique"]
    default_value: "NFC"
    
  numero_serie:
    source: "embedded"
    required: false
    prompt: "Numéro de série (optionnel):"
    
  couleur:
    source: "user"
    required: false
    prompt: "Couleur du badge:"
    options: ["Bleu", "Vert", "Rouge", "Jaune", "Blanc"]
    default_value: "Bleu"

# Configuration 360SmartConnect
avatar_360sc:
  enabled: true
  properties:
    name:
      mode: "embedded"
      required: true
    avatarType:
      mode: "template"
      value: "/api/avatar_types/badge-test"
    serialNumber:
      mode: "embedded"
      required: false
    status:
      mode: "template"
      value: 1
---

==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==

# ${nom}

> **Type de badge**: ${type_badge}  
> **Couleur**: ${couleur}  
> **Numéro de série**: ${numero_serie}  
> **Template**: Badge Test PML V3  

## 📋 Description

Badge de test pour ProcessMetaLanguage V3 avec support 360SmartConnect.

## 📊 Propriétés

| Propriété | Valeur |
|-----------|--------|
| **Nom** | ${nom} |
| **Type** | ${type_badge} |
| **Couleur** | ${couleur} |
| **Numéro de série** | ${numero_serie} |

## 🔗 360SmartConnect

- **Avatar Type**: Badge Test
- **Status**: Actif
- **Mode**: Test ProcessMetaLanguage V3

# Excalidraw Data

## Text Elements
${nom} ^veW9b56L

${type_badge} ^lvpIUavq

%%
## Drawing
```json
{
	"type": "excalidraw",
	"version": 2,
	"source": "https://github.com/zsviczian/obsidian-excalidraw-plugin/releases/tag/2.15.0",
	"elements": [
		{
			"id": "badge-rect-001",
			"type": "rectangle",
			"x": -151.787109375,
			"y": -74.935546875,
			"width": 301.720703125,
			"height": 150.009765625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1890ff",
			"fillStyle": "solid",
			"strokeWidth": 3,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"seed": 12345,
			"version": 83,
			"versionNonce": 47117909,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "veW9b56L"
				}
			],
			"updated": 1755633753240,
			"link": null,
			"locked": false,
			"index": "a0",
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3,
				"value": 15
			},
			"customData": {
				"legacyTextWrap": true
			}
		},
		{
			"id": "veW9b56L",
			"type": "text",
			"x": -32.94873046875,
			"y": -11.1806640625,
			"width": 64.0439453125,
			"height": 22.5,
			"angle": 0,
			"strokeColor": "#ffffff",
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
			"seed": 54321,
			"version": 84,
			"versionNonce": 380068789,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755633753240,
			"link": null,
			"locked": false,
			"text": "${nom}",
			"rawText": "${nom}",
			"fontSize": 18,
			"fontFamily": 5,
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "badge-rect-001",
			"originalText": "${nom}",
			"autoResize": true,
			"lineHeight": 1.25
		},
		{
			"id": "type-rect-002",
			"type": "rectangle",
			"x": -100,
			"y": 25,
			"width": 200,
			"height": 35,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#f0f0f0",
			"fillStyle": "solid",
			"strokeWidth": 2,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"seed": 67890,
			"version": 1,
			"versionNonce": 456789123,
			"isDeleted": false,
			"boundElements": [
				{
					"type": "text",
					"id": "lvpIUavq"
				}
			],
			"updated": 1705680000000,
			"link": null,
			"locked": false,
			"index": "a2",
			"groupIds": [],
			"frameId": null,
			"roundness": {
				"type": 3,
				"value": 8
			},
			"customData": {
				"legacyTextWrap": true
			}
		},
		{
			"id": "lvpIUavq",
			"type": "text",
			"x": -44.54393005371094,
			"y": 35,
			"width": 89.08786010742188,
			"height": 15,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "transparent",
			"fillStyle": "solid",
			"strokeWidth": 1,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"index": "a3",
			"roundness": null,
			"seed": 98765,
			"version": 1,
			"versionNonce": 789123456,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1705680000000,
			"link": null,
			"locked": false,
			"text": "${type_badge}",
			"rawText": "${type_badge}",
			"fontSize": 12,
			"fontFamily": 5,
			"textAlign": "center",
			"verticalAlign": "middle",
			"containerId": "type-rect-002",
			"originalText": "${type_badge}",
			"autoResize": true,
			"lineHeight": 1.25
		},
		{
			"id": "BxT_wiEKBTdY1sxpGNr0D",
			"type": "ellipse",
			"x": -50.630859375,
			"y": -115.400390625,
			"width": 99.451171875,
			"height": 63.181640625,
			"angle": 0,
			"strokeColor": "#1e1e1e",
			"backgroundColor": "#1890ff",
			"fillStyle": "solid",
			"strokeWidth": 3,
			"strokeStyle": "solid",
			"roughness": 1,
			"opacity": 100,
			"groupIds": [],
			"frameId": null,
			"index": "a4",
			"roundness": {
				"type": 2
			},
			"seed": 1839692661,
			"version": 118,
			"versionNonce": 793596053,
			"isDeleted": false,
			"boundElements": [],
			"updated": 1755618658574,
			"link": null,
			"locked": false
		}
	],
	"appState": {
		"theme": "light",
		"viewBackgroundColor": "#ffffff",
		"currentItemStrokeColor": "#1e1e1e",
		"currentItemBackgroundColor": "#1890ff",
		"currentItemFillStyle": "solid",
		"currentItemStrokeWidth": 3,
		"currentItemStrokeStyle": "solid",
		"currentItemRoughness": 1,
		"currentItemOpacity": 100,
		"currentItemFontFamily": 5,
		"currentItemFontSize": 18,
		"currentItemTextAlign": "center",
		"currentItemStartArrowhead": null,
		"currentItemEndArrowhead": "arrow",
		"currentItemArrowType": "round",
		"currentItemFrameRole": null,
		"scrollX": 186.375,
		"scrollY": 236.8642578125,
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
			"outline": true,
			"markerName": true,
			"markerEnabled": true
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