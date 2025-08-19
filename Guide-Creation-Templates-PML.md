<!-- START OF FILE: Guide-Creation-Templates-PML.md -->
# FILENAME: Guide-Creation-Templates-PML.md
# Version: 1.0.0
# Date: 2025-08-19 22:30
# Author: Rolland MELET & Claude Code
# Description: Guide complet pour créer des templates ProcessMetaLanguage V3

# Changelog:
# - v1.0.0: Création du guide complet de création de templates PML V3

# Guide de Création de Templates ProcessMetaLanguage V3

## 📖 Introduction

Ce guide vous accompagne pas à pas dans la création de templates compatibles avec le système ProcessMetaLanguage V3 (PML V3) pour Excalidraw dans Obsidian.

## 🎯 Qu'est-ce qu'un template PML V3 ?

Un template PML V3 est un fichier Markdown qui :
- Contient des **variables substituables** (placeholders)
- Définit **comment** ces variables sont collectées
- Génère un objet Excalidraw personnalisé
- Peut être réutilisé avec différentes valeurs

## 📋 Structure d'un template

### Anatomie complète

```markdown
---
# SECTION 1: Métadonnées PML (OBLIGATOIRE)
processmetalanguage_version: "3.0"
template_type: "type_descriptif"

# SECTION 2: Définitions des propriétés (OBLIGATOIRE)
property_definitions:
  variable1:
    source: "user"
    prompt: "Question pour l'utilisateur"
    required: true
    default_value: "valeur par défaut"
    options: ["choix1", "choix2"]
  
  variable2:
    source: "template"
    default_value: "valeur fixe"

# SECTION 3: Métadonnées Excalidraw (OBLIGATOIRE)
excalidraw-plugin: parsed
tags: [excalidraw]
---

# SECTION 4: Contenu du template avec variables
Titre: ${variable1}
Description: ${variable2}

# SECTION 5: Drawing Excalidraw (OPTIONNEL mais recommandé)
## Drawing
\`\`\`json
{
  "type": "excalidraw",
  "elements": [...]
}
\`\`\`
```

## 🔧 Étape par étape

### Étape 1 : Créer le fichier

1. Créer un nouveau fichier dans le dossier `Templates/`
2. Nommer le fichier de manière descriptive : `Badge-Template-PML.md`

### Étape 2 : Ajouter les métadonnées PML

```yaml
---
processmetalanguage_version: "3.0"
template_type: "badge"  # ou "card", "diagram", etc.
```

### Étape 3 : Définir les propriétés/variables

#### 3.1 Variable demandée à l'utilisateur

```yaml
property_definitions:
  nom:
    source: "user"
    prompt: "Nom de la personne :"
    required: true
    default_value: "John Doe"
    description: "Le nom qui apparaîtra sur le badge"
```

#### 3.2 Variable avec liste de choix

```yaml
  departement:
    source: "user"
    prompt: "Département :"
    required: true
    options: ["IT", "RH", "Production", "Commercial"]
    default_value: "IT"
```

#### 3.3 Variable template (fixe)

```yaml
  entreprise:
    source: "template"
    default_value: "360SmartConnect"
```

#### 3.4 Variable auto-générée

```yaml
  badge_id:
    source: "auto"
    description: "ID unique généré automatiquement"
```

#### 3.5 Variable embedded (optionnelle)

```yaml
  photo:
    source: "embedded"
    prompt: "Lien vers la photo (optionnel) :"
    required: false
```

### Étape 4 : Ajouter les métadonnées Excalidraw

```yaml
excalidraw-plugin: parsed
tags: [excalidraw]
```

### Étape 5 : Créer le contenu avec variables

Utiliser la syntaxe `${nom_variable}` :

```markdown
# Badge ${nom}

**Entreprise :** ${entreprise}
**Département :** ${departement}
**ID :** ${badge_id}

${photo}
```

### Étape 6 : Ajouter le dessin Excalidraw (optionnel)

```markdown
## Drawing
\`\`\`json
{
  "type": "excalidraw",
  "version": 2,
  "elements": [
    {
      "type": "rectangle",
      "x": 0,
      "y": 0,
      "width": 200,
      "height": 100,
      "backgroundColor": "#ffffff",
      "customData": {
        "name": "${nom}",
        "dept": "${departement}"
      }
    }
  ]
}
\`\`\`
```

## 📚 Types de sources détaillés

### `source: "user"`

Variable demandée interactivement à l'utilisateur.

**Options disponibles :**
- `prompt` : Question affichée
- `required` : Si true, doit être remplie
- `default_value` : Valeur pré-remplie
- `options` : Liste de choix (dropdown)
- `description` : Aide contextuelle

**Exemple complet :**
```yaml
fonction:
  source: "user"
  prompt: "Fonction du collaborateur :"
  required: true
  default_value: "Développeur"
  options: ["Développeur", "Chef de projet", "Designer", "Testeur"]
  description: "La fonction sera affichée sur le badge"
```

### `source: "template"`

Variable avec valeur fixe définie dans le template.

**Utilisation :** Constantes, valeurs par défaut, configuration

**Exemple :**
```yaml
version_template:
  source: "template"
  default_value: "v2.0"
logo_url:
  source: "template"
  default_value: "[[Logo-Entreprise.png]]"
```

### `source: "auto"`

Variable générée automatiquement selon son nom.

**Patterns reconnus :**
- Contient `id` → `ID_1755634567890`
- Contient `date` → `2025-01-19`
- Contient `time` → `2025-01-19T15:30:45.123Z`
- Autres → `AUTO_1755634567890`

**Exemple :**
```yaml
creation_date:
  source: "auto"
unique_id:
  source: "auto"
timestamp:
  source: "auto"
```

### `source: "embedded"`

Variable optionnelle pour liens ou références.

**Utilisation :** Photos, documents liés, références externes

**Exemple :**
```yaml
document_link:
  source: "embedded"
  prompt: "Lien vers le document (optionnel) :"
  required: false
```

## 🎨 Exemples complets

### Exemple 1 : Badge simple

```markdown
---
processmetalanguage_version: "3.0"
template_type: "badge"
property_definitions:
  nom:
    source: "user"
    prompt: "Nom complet :"
    required: true
  fonction:
    source: "user"
    prompt: "Fonction :"
    required: true
    options: ["Directeur", "Manager", "Employé", "Stagiaire"]
  entreprise:
    source: "template"
    default_value: "360SmartConnect"
  badge_id:
    source: "auto"

excalidraw-plugin: parsed
tags: [excalidraw]
---

# Badge Employé

**Nom :** ${nom}
**Fonction :** ${fonction}
**Entreprise :** ${entreprise}

Badge ID: ${badge_id}
```

### Exemple 2 : Card avec dessin

```markdown
---
processmetalanguage_version: "3.0"
template_type: "card"
property_definitions:
  titre:
    source: "user"
    prompt: "Titre de la carte :"
    required: true
  couleur:
    source: "user"
    prompt: "Couleur de fond :"
    options: ["#ff0000", "#00ff00", "#0000ff", "#ffff00"]
    default_value: "#0000ff"
  contenu:
    source: "user"
    prompt: "Contenu de la carte :"
    required: false
  creation_date:
    source: "auto"

excalidraw-plugin: parsed
tags: [excalidraw]
---

# ${titre}

${contenu}

*Créé le ${creation_date}*

## Drawing
\`\`\`json
{
  "type": "excalidraw",
  "version": 2,
  "elements": [
    {
      "type": "rectangle",
      "x": 0,
      "y": 0,
      "width": 300,
      "height": 200,
      "backgroundColor": "${couleur}",
      "strokeColor": "#000000"
    },
    {
      "type": "text",
      "x": 150,
      "y": 100,
      "text": "${titre}",
      "fontSize": 20,
      "textAlign": "center"
    }
  ]
}
\`\`\`
```

## ✅ Checklist de validation

Avant d'utiliser votre template, vérifiez :

- [ ] Le fichier est dans le dossier `Templates/`
- [ ] `processmetalanguage_version: "3.0"` est présent
- [ ] `template_type` est défini
- [ ] `property_definitions` contient au moins une variable
- [ ] Chaque variable a un `source` valide
- [ ] Les variables `user` ont un `prompt`
- [ ] Les variables sont utilisées avec `${variable}`
- [ ] `excalidraw-plugin: parsed` est présent
- [ ] Le JSON Excalidraw est valide (si présent)

## 🔍 Dépannage

### Le template n'apparaît pas dans la liste

**Vérifier :**
1. Le fichier est bien dans `Templates/`
2. L'extension est `.md`
3. Le front matter contient `processmetalanguage_version`
4. Le front matter contient `property_definitions`

### Les variables ne sont pas substituées

**Vérifier :**
1. Syntaxe exacte : `${nom_variable}`
2. Le nom correspond exactement à celui dans `property_definitions`
3. Pas d'espaces dans `${variable}`

### L'objet n'apparaît pas dans le canvas

**Vérifier :**
1. Le JSON Excalidraw est valide
2. Les éléments ont des coordonnées `x`, `y`
3. Les éléments ont `width`, `height` > 0

## 📊 Bonnes pratiques

### Nommage
- Templates : `Type-Description-PML.md`
- Variables : `snake_case` ou `camelCase`
- Types : descriptifs (`badge`, `card`, `diagram`)

### Organisation
```
Templates/
├── Badges/
│   ├── Badge-Employe-PML.md
│   └── Badge-Visiteur-PML.md
├── Cards/
│   ├── Card-Projet-PML.md
│   └── Card-Tache-PML.md
└── Diagrammes/
    └── Diagram-Process-PML.md
```

### Documentation
- Ajouter des `description` aux variables complexes
- Commenter le JSON Excalidraw si nécessaire
- Inclure des exemples de valeurs dans les `default_value`

## 🚀 Pour aller plus loin

### Intégration avec 360SmartConnect

Pour que vos templates soient compatibles avec 360SmartConnect, incluez :

```yaml
property_definitions:
  api_compatible:
    source: "template"
    default_value: "true"
  object_type:
    source: "template"
    default_value: "360SC_Badge"
  sync_enabled:
    source: "user"
    prompt: "Activer la synchronisation ?"
    options: ["true", "false"]
    default_value: "true"
```

### Variables calculées (future feature)

Dans les versions futures, support prévu pour :
```yaml
full_name:
  source: "computed"
  formula: "${prenom} ${nom}"
```

## 📚 Ressources

- [README.md](README.md) - Documentation générale
- [PLAN-DEVELOPPEMENT.md](PLAN-DEVELOPPEMENT.md) - Roadmap
- [Scripts/Embedded-Element-PML-From-Template.md](Scripts/Embedded-Element-PML-From-Template.md) - Le script

---

*Guide créé le 2025-01-19*
*Version ProcessMetaLanguage : 3.0*
<!-- END OF FILE: Guide-Creation-Templates-PML.md -->