# Besoins
J'ai besoin de creer :
## Embedded-Element-PML-From-Template
### description
Ce script doit permettre d'embedded dans le ficher Excalidraw courant, des elements Excalidraw à partir d'un Template.
Le script doit repérer, dans le template, quels sont les composants du fichier qui doivent être ajuster par l'utilisateur au moment de la creation du fichier qui sera embedded. (ex le nom du fichier)
Le script doit être capable de mettre à jour le coté textuel de l'objet et aussi le Drawing.
Le fichier Embedded doit être enregistré au même endroit que le fichier corrant dans lequel il est inséré.
### conditions de succes
le fichier embedded est créé 
il est présent au coté du fichier principal
le nom du fichier est celui de l'objet
C'est bien le dessin du fichier embedded qui apparait sur le canvas du fichier principal.
lors du "toggle entre Excalidraw et Markdown" le fichier Embedded garde sa dernière place, surtout si il a été déplacé apres la creation.

### Inspiration
ce script doit fortement s'inspirer du script decrit dans [[rollandmelet-excalidraw_script_embededdrawingfromtemplate]]

## Methode pour creer des templates

J'ai besoin d'une note descriptive pour savoir comment creer les template qui pourront être utilisé avec le script "Embedded-Element-PML-From-Template"

Cette methode doit prendre la forme d'un fichier Markdown qui decrira pas a pas ce qu'il faut faire pour creer le template.

# Informations générales

les scripts doivent se trouver dans le repertoire prévu pour les scripts dans les paramétres du plugin Excalidraw pour Obsidian.

les templates doivent se trouver dans le repertoire prévu pour les templates dans les paramétres d'Obsidian.

J'ai deux repertoire :
- un de travail ou doit se trouver les fichiers initiaux : c'est le repertoire `ProcessMetaLanguageV3` dans mon coffre principal obsidian dont le chemin complet est `/Users/rollandmelet/Library/CloudStorage/GoogleDrive-rm@360sc.io/Mon Drive/OBSIDIAN/CHATTERS/002 - Projets/PERSO/ProcessMetaLanguageV3`
- un coffre de test qui est dans `/Users/rollandmelet/Développement/Projets/ProcessMetaLanguage/VaultTestObsidian/PML-Beta-Test-v2` ou se trouve un repertoire `/Users/rollandmelet/Développement/Projets/ProcessMetaLanguage/VaultTestObsidian/PML-Beta-Test-v2/Excalidraw/Scripts`pour les scripts et un repertoire `/Users/rollandmelet/Développement/Projets/ProcessMetaLanguage/VaultTestObsidian/PML-Beta-Test-v2/Templates`pour les Templates

Il y a dans le repertoire corant du projet un repertoire `./Documentation`qui contient des documents issues de précédent projet et qui peuvent être pertinent avec des informations mettre en contexte : 
- [[zsviczian-obsidian-excalidraw-plugin]] = > le github du pluginn excalidraw avce tous les code notament des examples de scripts Excalidraw 
- [[002 - Projets/PERSO/ProcessMetaLanguageV3/Documentation/template-objet-backofcard]] : un exemple de template d'element "OBJET" dont je ne suis pas à 100% satisfait mais qui peut servir d'inspiration
- [[Script-Creation-Template-Avatar]] : une description de ce qu'il faut trouver au minimum dans un template pour que le fichier produit par le script soit compatible avec la plateforme 360SmartConnect.
- [[rollandmelet-excalidraw_script_embededdrawingfromtemplate]] : le github de mon précédent script dont il faut s'inspirer.

# REGLES

- Analyse les documents fournis
- Avec tes MCP tools recupére tout le savoir faire dont tu as besoin, notament sur Excalidraw et ses scripts
- ne fait pas trop de choses à la fois dans la production de rendu
- Etablie un plan detaillé dont les grandes devront être validée par l'utilisateur
- Suit le plan
- RESTE SIMPLE
- Lors des précédentes sessions je me suis appercu que certain savoir ou apprentissages ont été perdu. Organise toi pour que cela n'arrive plus en constituant une base de connaisance dans ta memory que tu sera capable de mobiliser pendant cette session et ultérieuerment.
