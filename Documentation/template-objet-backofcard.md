---
excalidraw-plugin: parsed
tags: [excalidraw, template, processmetalanguage, objet]

# Métadonnées du Template
template_type: "objet"
template_version: "1.0.0"
processmetalanguage_version: "2.3"
template_created: "2025-01-18"
template_author: "Rolland MELET & Claude Code"

# Définition des Propriétés de l'Objet
property_definitions:
  # === PROPRIÉTÉS SYSTÈME (générées automatiquement) ===
  id:
    source: "system"
    dynamic: false
    description: "UUID unique généré par 360SmartConnect"
    example: "550e8400-e29b-41d4-a716-446655440000"
    
  uid:
    source: "system"
    dynamic: false
    description: "Identifiant court unique"
    format: "OBJ{YYYYMMDD}{INDEX}"
    example: "OBJ20250118001"
    
  url_propre:
    source: "system"
    dynamic: false
    description: "URL permanente de l'objet"
    format: "/objects/{uid}"
    example: "/objects/OBJ20250118001"
    
  created_at:
    source: "system"
    dynamic: false
    description: "Timestamp de création ISO 8601"
    example: "2025-01-18T10:30:00Z"
    
  created_by:
    source: "system"
    dynamic: false
    description: "Utilisateur créateur"
    
  # === PROPRIÉTÉS UTILISATEUR (saisies à la création) ===
  nom:
    source: "user"
    dynamic: false
    required: true
    prompt: "Nom de l'objet:"
    validation: "Min 3 caractères"
    example: "Bloc Moteur BMW B48"
    
  description:
    source: "user"
    dynamic: true
    required: false
    prompt: "Description de l'objet (optionnelle):"
    multiline: true
    update_triggers: ["update_description", "enrich_metadata"]
    
  type_objet_workflow:
    source: "user"
    dynamic: false
    required: true
    prompt: "Type d'objet dans le workflow:"
    options: ["RESSOURCE", "CONSOMMABLE", "PRODUIT"]
    description: |
      RESSOURCE: Objets réutilisables qui cyclent dans le processus (moule, commande)
      CONSOMMABLE: Éléments consommés par le workflow (armature, étuvage, TIPI)
      PRODUIT: Objet produit par le workflow (voussoir, PAC)
    validation: "Doit être l'un des trois types"
    
  categorie:
    source: "user"
    dynamic: false
    required: false
    prompt: "Catégorie métier de l'objet:"
    options: ["Composant", "Document", "Matériel", "Matière première", "Service", "Autre"]
    
  proprietes_metier:
    source: "user"
    dynamic: true
    required: false
    type: "json"
    prompt: "Propriétés métier spécifiques (format JSON):"
    example: '{"reference": "BMW-B48-001", "poids": 120, "materiau": "aluminium"}'
    update_triggers: ["update_properties", "enrich_metadata"]
    
  tags:
    source: "user"
    dynamic: true
    required: false
    type: "array"
    prompt: "Tags (séparés par des virgules):"
    example: "moteur, bmw, production"
    update_triggers: ["add_tag", "remove_tag"]
    
  # === PROPRIÉTÉS SPÉCIFIQUES SELON TYPE ===
  # Pour RESSOURCE
  cycles_utilisation:
    source: "default"
    dynamic: true
    default_value: 0
    description: "Nombre de cycles d'utilisation (pour RESSOURCE)"
    update_triggers: ["increment_cycle", "reset_cycles"]
    applicable_to: ["RESSOURCE"]
    
  disponibilite:
    source: "default"
    dynamic: true
    default_value: "disponible"
    options: ["disponible", "en_utilisation", "maintenance", "indisponible"]
    description: "État de disponibilité (pour RESSOURCE)"
    update_triggers: ["change_availability"]
    applicable_to: ["RESSOURCE"]
    
  # Pour CONSOMMABLE
  quantite_stock:
    source: "user"
    dynamic: true
    default_value: 0
    type: "number"
    prompt: "Quantité en stock (pour CONSOMMABLE):"
    description: "Quantité disponible en stock"
    update_triggers: ["consume", "restock"]
    applicable_to: ["CONSOMMABLE"]
    
  lot_numero:
    source: "user"
    dynamic: false
    prompt: "Numéro de lot (pour CONSOMMABLE):"
    description: "Référence du lot de fabrication"
    applicable_to: ["CONSOMMABLE"]
    
  date_peremption:
    source: "user"
    dynamic: false
    type: "date"
    prompt: "Date de péremption (pour CONSOMMABLE, optionnel):"
    applicable_to: ["CONSOMMABLE"]
    
  # Pour PRODUIT
  date_production:
    source: "default"
    dynamic: true
    default_value: null
    type: "date"
    description: "Date de production (pour PRODUIT)"
    update_triggers: ["start_production", "complete_production"]
    applicable_to: ["PRODUIT"]
    
  conformite:
    source: "default"
    dynamic: true
    default_value: null
    options: ["conforme", "non_conforme", "en_controle", null]
    description: "Statut de conformité (pour PRODUIT)"
    update_triggers: ["quality_check", "approve", "reject"]
    applicable_to: ["PRODUIT"]
    
  traçabilite_composants:
    source: "default"
    dynamic: true
    default_value: []
    type: "array"
    description: "Liste des composants/consommables utilisés (pour PRODUIT)"
    update_triggers: ["add_component", "link_consumable"]
    applicable_to: ["PRODUIT"]
    
  # === PROPRIÉTÉS PAR DÉFAUT (initialisées à null) ===
  processus_objet_id:
    source: "default"
    dynamic: true
    default_value: null
    description: "ID du processus assigné à l'objet"
    update_triggers: ["assign_to_process", "remove_from_process"]
    validation: "Doit référencer un processus existant"
    
  etat_actuel_id:
    source: "default"
    dynamic: true
    default_value: null
    description: "ID de l'état actuel dans le processus"
    update_triggers: ["state_transition"]
    validation: "Si processus_objet_id existe, etat_actuel_id est OBLIGATOIRE"
    
  etat_actuel_nom:
    source: "default"
    dynamic: true
    default_value: null
    description: "Nom lisible de l'état actuel"
    update_triggers: ["state_transition"]
    
  workflow_parent_id:
    source: "default"
    dynamic: true
    default_value: null
    description: "ID du workflow parent"
    update_triggers: ["attach_to_workflow", "detach_from_workflow"]
    
  priorite:
    source: "default"
    dynamic: true
    default_value: "normale"
    options: ["basse", "normale", "haute", "critique"]
    update_triggers: ["change_priority"]
    
  statut:
    source: "default"
    dynamic: true
    default_value: "actif"
    options: ["actif", "inactif", "archive", "supprime"]
    update_triggers: ["change_status"]
    
  # === PROPRIÉTÉS SYSTÈME DYNAMIQUES ===
  modified_at:
    source: "system"
    dynamic: true
    description: "Dernière modification"
    update_triggers: ["*"]
    
  modified_by:
    source: "system"
    dynamic: true
    description: "Dernier utilisateur modificateur"
    update_triggers: ["*"]
    
  version:
    source: "system"
    dynamic: true
    default_value: 1
    description: "Version de l'objet"
    update_triggers: ["*"]
    
  historique:
    source: "system"
    dynamic: true
    default_value: []
    type: "array"
    description: "Historique complet des modifications"
    update_triggers: ["*"]
    structure:
      - timestamp: "ISO 8601"
      - property: "Propriété modifiée"
      - old_value: "Ancienne valeur"
      - new_value: "Nouvelle valeur"
      - action: "Action déclenchante"
      - user: "Utilisateur"
      
  liens:
    source: "default"
    dynamic: true
    default_value: []
    type: "array"
    description: "Liens vers d'autres objets"
    update_triggers: ["create_link", "remove_link"]
    
  fichiers_attaches:
    source: "default"
    dynamic: true
    default_value: []
    type: "array"
    description: "Fichiers attachés à l'objet"
    update_triggers: ["attach_file", "detach_file"]

# Configuration d'affichage selon type
display_config:
  RESSOURCE:
    couleur: "#52C41A"  # Vert - objets réutilisables
    icone: "🔄"         # Cycle
    forme: "rectangle"
    description: "Objet réutilisable qui cycle dans le processus"
  CONSOMMABLE:
    couleur: "#FA8C16"  # Orange - consommables
    icone: "📦"         # Paquet
    forme: "rectangle"
    description: "Élément consommé par le workflow"
  PRODUIT:
    couleur: "#1890FF"  # Bleu - produit final
    icone: "🏭"         # Usine/Production
    forme: "rectangle"
    description: "Objet produit par le workflow"
  taille_defaut:
    width: 200
    height: 100

---

==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠==

# ${nom}

> **Type d'objet**: ${type_objet_workflow}  
> **UID**: ${uid}  
> **URL**: ${url_propre}  
> **Créé le**: ${created_at}  
> **Créé par**: ${created_by}  

## 📋 Informations Générales

| Propriété | Valeur |
|-----------|--------|
| **Nom** | ${nom} |
| **Type dans Workflow** | ${type_objet_workflow} |
| **Description** | ${description} |
| **Catégorie** | ${categorie} |
| **Tags** | ${tags} |
| **Priorité** | ${priorite} |
| **Statut** | ${statut} |

## 🎯 Propriétés Spécifiques (${type_objet_workflow})

### Pour RESSOURCE
| Propriété | Valeur |
|-----------|--------|
| **Cycles d'utilisation** | ${cycles_utilisation} |
| **Disponibilité** | ${disponibilite} |

### Pour CONSOMMABLE
| Propriété | Valeur |
|-----------|--------|
| **Quantité en stock** | ${quantite_stock} |
| **Numéro de lot** | ${lot_numero} |
| **Date de péremption** | ${date_peremption} |

### Pour PRODUIT
| Propriété | Valeur |
|-----------|--------|
| **Date de production** | ${date_production} |
| **Conformité** | ${conformite} |
| **Composants tracés** | ${traçabilite_composants} |

## 🔄 État dans le Processus

| Propriété | Valeur |
|-----------|--------|
| **Processus** | ${processus_objet_id} |
| **État Actuel** | ${etat_actuel_nom} (${etat_actuel_id}) |
| **Workflow Parent** | ${workflow_parent_id} |

## 📊 Propriétés Métier

```yaml
${proprietes_metier}
```

## 🔗 Relations

### Liens vers autres objets
${liens}

### Fichiers attachés
${fichiers_attaches}

## 📝 Historique des Modifications

```dataview
TABLE 
  timestamp as "Date/Heure",
  property as "Propriété",
  old_value as "Ancienne Valeur",
  new_value as "Nouvelle Valeur",
  action as "Action",
  user as "Utilisateur"
FROM this.historique
SORT timestamp DESC
```

## 🎨 Zone de Dessin Excalidraw

*L'utilisateur dessine ici la représentation visuelle de l'objet*

# Excalidraw Data

## Text Elements
OBJET
${nom} ^Oq8Ia1VJ

%%
## Drawing
```compressed-json
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
```
%%