Directory structure:
└── zsviczian-obsidian-excalidraw-plugin/
    ├── README.md
    ├── AutomateHowTo.md
    ├── esbuild.config.json
    ├── manifest-beta.json
    ├── manifest.json
    ├── package.json
    ├── rollup.config.js
    ├── styles.css
    ├── tsconfig-lib.json
    ├── tsconfig.dev.json
    ├── tsconfig.json
    ├── versions.json
    ├── .babelrc
    ├── .eslintignore
    ├── .eslintrc.json
    ├── .nvmrc
    ├── .replit
    ├── docs/
    │   ├── readme.md
    │   ├── _config.yml
    │   ├── ExcalidrawScriptsEngine.md
    │   ├── API/
    │   │   ├── attributes_functions_overview.md
    │   │   ├── canvas_style.md
    │   │   ├── element_style.md
    │   │   ├── introduction.md
    │   │   ├── objects.md
    │   │   └── utility.md
    │   ├── Examples/
    │   │   ├── apply_template.md
    │   │   ├── connect_objects.md
    │   │   ├── dataviewjs_familytree.md
    │   │   ├── dataviewjs_mindmap.md
    │   │   ├── insert_new_drawing.md
    │   │   └── templater_mindmap.md
    │   └── zh-cn/
    │       ├── README.md
    │       ├── AutomateHowTo.md
    │       ├── docs/
    │       │   ├── readme.md
    │       │   ├── ExcalidrawScriptsEngine.md
    │       │   ├── API/
    │       │   │   ├── attributes_functions_overview.md
    │       │   │   ├── canvas_style.md
    │       │   │   ├── element_style.md
    │       │   │   ├── introduction.md
    │       │   │   ├── objects.md
    │       │   │   └── utility.md
    │       │   └── Examples/
    │       │       ├── apply_template.md
    │       │       ├── connect_objects.md
    │       │       ├── dataviewjs_familytree.md
    │       │       ├── dataviewjs_mindmap.md
    │       │       ├── insert_new_drawing.md
    │       │       └── templater_mindmap.md
    │       └── ea-scripts/
    │           └── README.md
    ├── ea-scripts/
    │   ├── README.md
    │   ├── Add Connector Point.md
    │   ├── Add Link to Existing File and Open.md
    │   ├── Add Link to New Page and Open.md
    │   ├── Add Next Step in Process.md
    │   ├── Auto Layout.md
    │   ├── Boolean Operations.md
    │   ├── Box Each Selected Groups.md
    │   ├── Box Selected Elements.md
    │   ├── Change shape of selected elements.md
    │   ├── Concatenate lines.md
    │   ├── Connect elements.md
    │   ├── Convert freedraw to line.md
    │   ├── Convert selected text elements to sticky notes.md
    │   ├── Convert text to link with folder and alias.md
    │   ├── Copy Selected Element Styles to Global.md
    │   ├── Create DrawIO file.md
    │   ├── Create new markdown file and embed into active drawing.md
    │   ├── Crop Vintage Mask.md
    │   ├── Custom Zoom.md
    │   ├── Darken background color.md
    │   ├── Deconstruct selected elements into new drawing.md
    │   ├── directory-info.json
    │   ├── Elbow connectors.md
    │   ├── Ellipse Selected Elements.md
    │   ├── ExcaliAI.md
    │   ├── Excalidraw Collaboration Frame.md
    │   ├── Excalidraw Writing Machine.md
    │   ├── Expand rectangles horizontally keep text centered.md
    │   ├── Expand rectangles horizontally.md
    │   ├── Expand rectangles vertically keep text centered.md
    │   ├── Expand rectangles vertically.md
    │   ├── Fixed horizontal distance between centers.md
    │   ├── Fixed inner distance.md
    │   ├── Fixed spacing.md
    │   ├── Fixed vertical distance between centers.md
    │   ├── Fixed vertical distance.md
    │   ├── Folder Note Core - Make Current Drawing a Folder.md
    │   ├── Full-Year Calendar Generator.md
    │   ├── Golden Ratio.md
    │   ├── GPT-Draw-a-UI.md
    │   ├── Grid Selected Images.md
    │   ├── Image Occlusion.md
    │   ├── Invert colors.md
    │   ├── Lighten background color.md
    │   ├── Mindmap connector.md
    │   ├── Mindmap format.md
    │   ├── Modify background color opacity.md
    │   ├── Normalize Selected Arrows.md
    │   ├── Organic Line Legacy.md
    │   ├── Organic Line.md
    │   ├── Palette loader.md
    │   ├── Palm Guard.md
    │   ├── PDF Page Text to Clipboard.md
    │   ├── Printable Layout Wizard.md
    │   ├── Relative Font Size Cycle.md
    │   ├── Rename Image.md
    │   ├── Repeat Elements.md
    │   ├── Repeat Texts.md
    │   ├── Reset LaTeX Size.md
    │   ├── Reverse arrows.md
    │   ├── Scribble Helper.md
    │   ├── Select Elements of Type.md
    │   ├── Select Similar Elements.md
    │   ├── Set background color of unclosed line object by adding a shadow clone.md
    │   ├── Set Dimensions.md
    │   ├── Set Font Family.md
    │   ├── Set Grid.md
    │   ├── Set Link Alias.md
    │   ├── Set Stroke Width of Selected Elements.md
    │   ├── Set Text Alignment.md
    │   ├── Shade Master.md
    │   ├── Slideshow.md
    │   ├── Split Ellipse.md
    │   ├── Split text by lines.md
    │   ├── Text Aura.md
    │   ├── Text to Path.md
    │   ├── Text to Sticky Notes.md
    │   ├── To Line.md
    │   ├── Toggle Grid.md
    │   ├── Uniform size.md
    │   ├── Zoom to Fit Selected Elements.md
    │   ├── Archive/
    │   │   ├── Alternative Pens.md
    │   │   ├── index.md
    │   │   ├── OCR - Optical Character Recognition.md
    │   │   ├── TheBrain-navigation.md
    │   │   ├── Toggle Fullscreen on Mobile.md
    │   │   └── Transfer TextElements to Excalidraw markdown metadata.md
    │   └── pens/
    │       ├── Fine tipped pen - fixed pressure.md
    │       ├── Fountain pen.md
    │       ├── Mindmap - thick-thin-thick.md
    │       ├── Mindmap - thick-thin.md
    │       ├── Thick marker - dynamic pressure.md
    │       └── Thick marker - fixed pressure.md
    ├── MathjaxToSVG/
    │   ├── index.ts
    │   ├── package.json
    │   ├── rollup.config.js
    │   └── tsconfig.json
    ├── scripts/
    │   ├── ea-scripts-with-modified-dates.md
    │   └── generate-script-library.js
    ├── src/
    │   ├── constants/
    │   │   ├── constants.ts
    │   │   ├── constSettingsTags.ts
    │   │   ├── starutpscript.ts
    │   │   └── assets/
    │   │       └── startupScript.md
    │   ├── core/
    │   │   ├── index.ts
    │   │   ├── editor/
    │   │   │   ├── EditorHandler.ts
    │   │   │   └── Fadeout.ts
    │   │   └── managers/
    │   │       ├── EventManager.ts
    │   │       ├── FileManager.ts
    │   │       ├── MarkdownPostProcessor.ts
    │   │       ├── ObserverManager.ts
    │   │       ├── PackageManager.ts
    │   │       └── StylesManager.ts
    │   ├── lang/
    │   │   ├── helpers.ts
    │   │   ├── langDiffWithEn.js
    │   │   └── locale/
    │   │       ├── ar.ts
    │   │       ├── cz.ts
    │   │       ├── da.ts
    │   │       ├── de.ts
    │   │       ├── en-gb.ts
    │   │       ├── fr.ts
    │   │       ├── hi.ts
    │   │       ├── hu.ts
    │   │       ├── id.ts
    │   │       ├── it.ts
    │   │       ├── ja.ts
    │   │       ├── ko.ts
    │   │       ├── nl.ts
    │   │       ├── no.ts
    │   │       ├── pl.ts
    │   │       ├── pt-br.ts
    │   │       ├── pt.ts
    │   │       ├── ro.ts
    │   │       └── tr.ts
    │   ├── shared/
    │   │   ├── CropImage.ts
    │   │   ├── EmbeddedFileLoader.ts
    │   │   ├── ExcalidrawConfig.ts
    │   │   ├── Frontmatter.ts
    │   │   ├── ImageCache.ts
    │   │   ├── LaTeX.ts
    │   │   ├── Scripts.ts
    │   │   ├── WeakArray.ts
    │   │   ├── components/
    │   │   │   └── ContentSearcher.ts
    │   │   ├── Dialogs/
    │   │   │   ├── EmbeddableMDFileCustomDataSettingsComponent.ts
    │   │   │   ├── EmbeddableSettings.ts
    │   │   │   ├── ExportDialog.ts
    │   │   │   ├── FloatingModal.ts
    │   │   │   ├── FrameSettings.ts
    │   │   │   ├── HotkeyEditor.ts
    │   │   │   ├── ImportSVGDialog.ts
    │   │   │   ├── InsertCommandDialog.ts
    │   │   │   ├── InsertImageDialog.ts
    │   │   │   ├── InsertLinkDialog.ts
    │   │   │   ├── InsertMDDialog.ts
    │   │   │   ├── InsertPDFModal.ts
    │   │   │   ├── Messages.ts
    │   │   │   ├── ModifierKeySettings.ts
    │   │   │   ├── OpenDrawing.ts
    │   │   │   ├── PDFExportSettingsComponent.ts
    │   │   │   ├── PenSettingsModal.ts
    │   │   │   ├── Prompt.ts
    │   │   │   ├── PublishOutOfDateFiles.ts
    │   │   │   ├── RankMessage.ts
    │   │   │   ├── ReleaseNotes.ts
    │   │   │   ├── ScriptInstallPrompt.ts
    │   │   │   ├── SelectCard.ts
    │   │   │   └── UniversalInsertFileModal.ts
    │   │   ├── OCR/
    │   │   │   └── Taskbone.ts
    │   │   ├── Suggesters/
    │   │   │   ├── FieldSuggester.ts
    │   │   │   ├── FileSuggestionModal.ts
    │   │   │   ├── FolderSuggestionModal.ts
    │   │   │   ├── PathSuggestionModal.ts
    │   │   │   ├── Suggester.ts
    │   │   │   └── SuggestionModal.ts
    │   │   ├── svgToExcalidraw/
    │   │   │   ├── readme.md
    │   │   │   ├── attributes.ts
    │   │   │   ├── parser.ts
    │   │   │   ├── transform.ts
    │   │   │   ├── types.ts
    │   │   │   ├── utils.ts
    │   │   │   ├── walker.ts
    │   │   │   └── elements/
    │   │   │       ├── ExcalidrawElement.ts
    │   │   │       ├── ExcalidrawScene.ts
    │   │   │       ├── Group.ts
    │   │   │       ├── index.ts
    │   │   │       ├── utils.ts
    │   │   │       └── path/
    │   │   │           ├── index.ts
    │   │   │           └── utils/
    │   │   │               ├── bezier.ts
    │   │   │               ├── ellipse.ts
    │   │   │               └── path-to-points.ts
    │   │   └── Workers/
    │   │       └── compression-worker.ts
    │   ├── types/
    │   │   ├── excalidrawAutomateTypes.ts
    │   │   ├── excalidrawLib.d.ts
    │   │   ├── excalidrawViewTypes.ts
    │   │   ├── penTypes.ts
    │   │   ├── polybooljs.d.ts
    │   │   ├── promptTypes.ts
    │   │   ├── types.d.ts
    │   │   ├── utilTypes.ts
    │   │   └── worker.d.ts
    │   ├── utils/
    │   │   ├── AIUtils.ts
    │   │   ├── carveout.ts
    │   │   ├── customEmbeddableUtils.ts
    │   │   ├── debugHelper.ts
    │   │   ├── dynamicStyling.ts
    │   │   ├── ErrorHandler.ts
    │   │   ├── excalidrawAutomateUtils.ts
    │   │   ├── excalidrawSceneUtils.ts
    │   │   ├── excalidrawViewUtils.ts
    │   │   ├── exportUtils.ts
    │   │   ├── fileUtils.ts
    │   │   ├── getElementAtPointer.ts
    │   │   ├── matic.ts
    │   │   ├── mermaidUtils.ts
    │   │   ├── modifierkeyHelper.ts
    │   │   ├── obsidianUtils.ts
    │   │   ├── PDFUtils.ts
    │   │   ├── pens.ts
    │   │   ├── screenshot.ts
    │   │   ├── sliderUtils.ts
    │   │   ├── typechecks.ts
    │   │   ├── utils.ts
    │   │   └── YoutTubeUtils.ts
    │   └── view/
    │       ├── ExcalidrawLoading.ts
    │       ├── components/
    │       │   ├── CustomEmbeddable.tsx
    │       │   └── menu/
    │       │       ├── ActionButton.tsx
    │       │       ├── EmbeddableActionsMenu.tsx
    │       │       ├── ObsidianMenu.tsx
    │       │       └── ToolsPanel.tsx
    │       └── managers/
    │           ├── CanvasNodeFactory.ts
    │           └── DropManager.ts
    ├── .devcontainer/
    │   └── devcontainer.json
    └── .github/
        ├── dependabot.yml
        ├── ISSUE_TEMPLATE/
        │   ├── bug_report.md.x
        │   ├── bug_report.yml
        │   ├── Contribution.yml.old
        │   ├── feature-request.yml
        │   ├── feature_request.md.old
        │   └── How-to.yml
        └── workflows/
            └── codeql-analysis.yml


Files Content:

(Files content cropped to 300k characters, download full ingest to see more)
================================================
FILE: README.md
================================================
# Excalidraw

【English | [简体中文](./docs/zh-cn/README.md)】

👉👉👉 Check out and contribute to the new [Obsidian-Excalidraw Community Wiki](https://excalidraw-obsidian.online/WIKI/Welcome+to+the+WIKI)

The Obsidian-Excalidraw plugin integrates [Excalidraw](https://excalidraw.com/), a feature rich sketching tool, into Obsidian. You can store and edit Excalidraw files in your vault, you can embed drawings into your documents, and you can link to documents and other drawings to/and from Excalidraw. For a showcase of Excalidraw features, please read my blog post [here](https://www.zsolt.blog/2021/03/showcasing-excalidraw.html) and/or watch the videos below.

Excalidraw for Obsidian keeps evolving; it is extremely feature‑rich and can feel intimidating at first. The Video Walkthrough below should ease that initial overwhelm. For a comprehensive, searchable knowledge base covering features, settings, scripting, workflows, and visual thinking methods, explore the public [NotebookLM workbook](https://notebooklm.google.com/notebook/42d76a2f-c11d-4002-9286-1683c43d0ab0) (a must‑have learning resource). If you are curious about the Visual PKM philosophy behind the plugin, consider my book [Sketch Your Mind](https://sketch-your-mind.com/) and the [Visual Thinking Workshops](https://visual-thinking-workshop.com/). Finally, keep the [Excalidraw Plugin Wiki](https://excalidraw-obsidian.online/) at hand—it is an essential companion.

## Video Walkthrough
<a href="https://youtu.be/P_Q6avJGoWI" target="_blank"><img src="https://github.com/zsviczian/obsidian-excalidraw-plugin/assets/14358394/da34bb33-7610-45e6-b36f-cb7a02a9141b" width="300"/></a>
<a href="https://youtu.be/o0exK-xFP3k" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931370-aa4d88de-c4a8-46cc-aeb2-dc09aa0bea39.jpg" width="300"/></a> 
<a href="https://youtu.be/QKnQgSjJVuc" target="_blank"><img src="https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/thumbnail-getting-started.jpg" width="300"/></a>

### Here's my complete catalog of videos:
<a href="https://excalidraw-obsidian.online/Hobbies/Excalidraw+Blog/Catalogue+of+Videos"><img width="380" alt="image" src="https://github.com/zsviczian/obsidian-excalidraw-plugin/assets/14358394/2577e5ad-7a21-4c62-acd5-4fe80c8a8a95"></a>
<br>

<details><summary>10 Part (slightly outdated) Video Walkthrough</summary>
<a href="https://youtu.be/sY4FoflGaiM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160304-7f211180-e17c-11eb-8363-c52723de1ffd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;1  Getting Started</a><br>
<a href="https://youtu.be/Iy_oVTq12Gw" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160312-8a743d00-e17c-11eb-9fa2-490ef4cbd59e.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;2  Basic shapes and features</a><br>
<a href="https://youtu.be/QOL1KF7-kdc" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160323-96f89580-e17c-11eb-9bce-8eb1067a51bb.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;3  Grouping elements</a><br>
<a href="https://youtu.be/aSgcbfspvfo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160332-9f50d080-e17c-11eb-98e9-fec60fe147d9.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;4  The stencil-library</a><br>
<a href="https://youtu.be/MaJ5jJwBRWs" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160341-a546b180-e17c-11eb-9de8-d87fdc844c9c.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;5  Embedding</a><br>
<a href="https://youtu.be/MXzeCOEExNo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160346-aa0b6580-e17c-11eb-930b-4024807040d1.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;6  Links</a><br>
<a href="https://youtu.be/R0IAg0s-wQE" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160354-b2fc3700-e17c-11eb-81af-9e71e461f6dd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;7  Markdown</a><br>
<a href="https://youtu.be/ibdS7ykwpW4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160360-b8f21800-e17c-11eb-8bd8-79d4e3f6e92d.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;8  Templates</a><br>
<a href="https://youtu.be/VRZVujfVab0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160367-bdb6cc00-e17c-11eb-92f1-6f59faea85fd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;9  Excalidraw Automate</a><br>
<a href="https://youtu.be/D1iBYo1_jjc" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160374-c3141680-e17c-11eb-8cc2-dfaffd903d15.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;10  Miscellaneous</a><br>
</details>
<details><summary>Embedding stuff into Excalidraw</summary>
<a href="https://www.youtube.com/watch?v=_c_0zpBJ4Xc&" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/138607067-ccb62f92-48a4-4880-ac6e-68c1bf86ac2c.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Image Elements</a><br>
<a href="https://youtu.be/r08wk-58DPk" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143732412-1c65227e-4381-406d-847a-b001ab3506ca.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;LaTex Demo</a><br>
<a href="https://youtu.be/tsecSfnTMow" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143732440-90bfa029-8615-462e-ada3-c903d71a82c9.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Markdown embeds</a><br>
<a href="https://youtu.be/K6qZkTz8GHs" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143783906-15cee494-c6d5-4495-a2ca-74634e4e7355.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Markdown embeds advanced features</a><br>
<a href="https://youtu.be/Etskjw7a5zo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931461-0979b821-315a-41dd-86f1-31d169b7c127.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Link to Elements, Vertical text alignment, Markdown Styling</a><br>
</details>
<details><summary>The Script Engine Store - Excalidraw Automation</summary>
<a href="https://youtu.be/hePJcObHIso" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/145684531-8d9c2992-59ac-4ebc-804a-4cce1777ded2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Introducing the Script Engine</a><br>
<a href="https://youtu.be/lzYdOQ6z8F0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/147889174-6c306d0d-2d29-46cc-a53f-3f0013cf14de.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Script Engine Store</a><br>
</details>
<details><summary>Working with colors</summary>
<a href="https://youtu.be/6PLGHBH9VZ4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773147-5418a0ab-6be5-4eb0-a8e4-d6af21b1b483.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Colors - Excalidraw Basics (Custom)</a><br>
<a href="https://youtu.be/epYNx2FSf2w" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773211-9e871be7-0795-4dc7-947e-c6c275e690d0.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Excalidraw color palettes (Custom)</a><br>
<a href="https://youtu.be/Amhlv6r9WvM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773268-400cfb1b-6bde-45e0-9e4b-91bbaa461cf0.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;"Artistic" Color Gradients</a><br>
<a href="https://youtu.be/r9oB1SlK1GU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773527-ef35c8b9-1a6d-4415-9c7e-b667fb17535d.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Simple rules for beautiful sketches</a><br>
<a href="https://youtu.be/7gJDwNgQ6NU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/195988535-a133a9b9-d094-45ba-ba64-c994b9a1e0ef.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;ColorMaster Scripting</a><br>
</details>
<details><summary>Links and block references</summary>
<a href="https://youtu.be/qiKuqMcNWgU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/171635214-30533c45-94fa-436e-83a9-b2ec99f190e2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;6 strategies for linking your visual thoughts v4</a><br>
<a href="https://youtu.be/yZQoJg2RCKI" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/185791706-3d9983ab-7cb1-4b27-a016-30c039d84e34.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Block reference parts of images</a><br>
<a href="https://youtu.be/Etskjw7a5zo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931461-0979b821-315a-41dd-86f1-31d169b7c127.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Link to Elements, Vertical text alignment, Markdown Styling</a><br>
<a href="https://youtu.be/2Y8OhkGiTHg" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/152585752-7eb0371f-0bab-40f6-a194-3b48e5811735.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;How to guide for the Excalidraw-native hyperlinks</a><br>
</details>
<details><summary>Powertools</summary>
<a href="https://youtu.be/NOuddK6xrr8" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/147283367-e5689385-ea51-4983-81a3-04d810d39f62.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Sticky Notes (word wrapping)</a><br>
<a href="https://youtu.be/eKFmrSQhFA4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/149659524-2a4e0a24-40c9-4e66-a6b1-c92f3b88ecd5.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Fourth Font</a><br>
<a href="https://youtu.be/vlC1-iBvIfo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/199207784-8bbe14e0-7d10-47d7-971d-20dce8dbd659.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;SVG import</a><br>
<a href="https://youtu.be/7gu4ETx7zro" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/202916770-28f2fa64-1ba2-4b40-a7fe-d721b42634f7.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;OCR</a><br>
<a href="https://youtu.be/U2LkBRBk4LY" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/159369910-6371f08d-b5fa-454d-9c6c-948f7e7a7d26.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Bind/unbind text from container, Frontmatter tags to customize export</a><br>
<a href="https://youtu.be/uZz5MgzWXiM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/211054371-8872e01a-77d6-4afc-a0c2-86a55410a8d3.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Custom pen support</a><br>
</details>
<details><summary>Quality of life improvements</summary>
<a href="https://youtu.be/qbPIAZguJeo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/151705333-54e9ffd2-0bd7-4d02-b99e-0bd4e4708d4d.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Mobile Support</a><br>
<a href="https://youtu.be/2v9TZmQNO8c" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/153676009-6f86b2d7-c248-49a2-b802-be21c6999e4f.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Tray-mode and Customizable Color Palette</a><br>
<a href="https://youtu.be/xHPGWR3m0c8" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/154821232-a404b6cf-72fb-4ce4-9d53-619132dce491.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Compressed JSON and improved save/sync support</a><br>
<a href="https://youtu.be/gMIKXyhS-dM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931428-b2269fd9-87bd-43ab-8558-5572f40dff93.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;The Obsidian Tools Panel</a><br>
<a href="https://youtu.be/4N6efq1DtH0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/158008902-12c6a851-237e-4edd-a631-d48e81c904b2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Eraser, left-handed mode, improved filename configuration</a><br>
</details>

### Beta testing
The plugin follows a monthly release schedule. If you want to receive more frequent updates with new features (e.g. shiny new stuff available on excalidraw.com, but not yet in Obsidian) and minor bug fixes, then join the beta community.

[![Thumbnail - 20240803 Excalidraw Release Approach (Custom)](https://github.com/user-attachments/assets/ab40648c-f73f-4bda-a416-52839f918f2a)](https://youtu.be/2poSS-Z91lY)

[![Excalidraw Plugin Release Strategy (Phone)](https://github.com/user-attachments/assets/87f1f379-782c-4c32-8b5b-d27fe2d3ac4b)](https://github.com/user-attachments/assets/120a0790-7239-48ae-bfbd-eb249f8b518d)

---

## Features

- The plugin integrates Excalidraw seamlessly into Obsidian, including Command Palette actions, File Explorer features, Option Menu commands, and the Ribbon Button.
- <kbd>CTRL/CMD+Click</kbd> on the ribbon button or in the file explorer to create / open drawings in a new pane.

### Settings

Settings will allow you to customize Excalidraw to your needs. The plugin comes with tons of settings. I tried adding meaningful explanations to these settings, so please be patient and look for the setting, for most requests, a setting already exists.

Plugin settings are grouped into the following sections:
- **Basic settings**: such as default folders to use.
- **Saving**: compression and autosave timer.
- **Filename**: configure the automatically created Excalidraw filename.
- **Display**: settings that affect the handling of Excalidraw (e.g.: left-handed mode, theme settings, mouse wheel and pinch zoom settings, zoom to fit settings).
- **Links and transclusions**: Settings that affect how links and embedded items behave on the Excalidraw canvas.
- **Markdown-embed settings**: These settings control how markdown documents from your Vault embedded into Excalidraw drawings will behave.
- **Embed & Export**: Settings that control how Excalidraw images are displayed when embedding them into markdown documents.
- **Auto-export Settings**: You can configure Excalidraw to create a PNG or SVG copy of your drawing each time it gets saved.
- **Compatibility features**: Check these settings if you edit the Excalidraw drawings outside Obsidian (e.g. in LogSeq, Visual Studio, on the web, etc.).
- **Experimental features**: There are advanced features that are implemented as "clever" hacks. Features include defining a fourth font, adding a custom icon to distinguish Exalidraw files in the Obsidian file explorer, OCR settings, and more.
- **Settings for installed Scripts**: Some of the scripts you install from the Script Library come with settings. Script settings are installed the first time you run the script. So to access settings for a script, install the script, run it for the first time and then look for the settings in plugin settings.

#### Templates

- Template for new drawings. The template will restore stroke properties. This means you can set up defaults in your template for stroke color, stroke width, opacity, font family, font size, fill style, stroke style, etc. This also applies to ExcalidrawAutomate. With versions 1.6.13 or higher make sure to enable "Decompress Excalidraw JSON in Markdown View" in the settings before editing the JSON in the template. This can be disabled after the canges are performed.
  - Via the template, you can customize the color palette used by Excalidraw.
    - Switch to Markdown view.
    - Scroll down to the bottom of the file and find `"AppState": {`.
    - Find `"colorPalette": {` at the end of the AppState section.
        - You may specify the 3 palettes used in Excalidraw by adding any or all of the following 3 variables:
            - `"canvasBackground":[], "elementBackground":[], "elementStroke": []`.
            - Add a comma-separated list of valid HTML colors (e.g. `#FF0000` for red) in the array for each of the variables.
        - To change the previewed colors, a `"topPicks": {` may be specified containing the same three keys:
            - `"canvasBackground":[], "elementBackground":[], "elementStroke": []`.
            - Note that the corresponding arrays must contain 5 elements.
    - See my videos above for further help.

#### Export

- If portability is important to you:
  - Auto-export SVG and/or PNG files, including the keep-in-sync feature, so you can
      embed SVG/PNG into your documents instead of embedding excalidraw files.
  - You can override export settings for an individual file by adding the `excalidraw-autoexport`
      frontmatter key. Valid values for this key are `none`, `both`, 'png', and `svg`.

- Specify the default width of embedded drawings.
- Compatibility features to auto-export and keep in sync markdown excalidraw files and legacy `.excalidraw` files.
- Experimental feature to add custom TAG to file explorer to mark drawing files.
- Enable / disable autosave.

### Embedding your drawings into markdown documents

- You can customize the size and position of the embedded images using the
  - `![[image.excalidraw|100]]`,
  - `![[image.excalidraw|100x100]]`,
  - `![[image.excalidraw|100|left]]`,
  - `![[image.excalidraw|right-wrap]]`, formatting options.
  - `![[<filename.excalidraw>|<width>x<height>|<alignment>]]`.
  - You can add your custom [alignment via CSS](https://www.scaler.com/topics/align-image-in-html/).
  - Any text that appears in `<alignment>` will be added to the rendered SVG element style and to the wrapper DIV element.
  - See [styles.css](https://github.com/zsviczian/obsidian-excalidraw-plugin/blob/master/styles.css) for more insight.
- Excalidraw drawings do not display in Obsidian Publish. If you want to use Excalidraw in your published documents, you can configure in plugin settings, under `Embed & Export`, to automatically insert a PNG or SVG version of the drawing in your document when creating a new file. See `type of file to insert into document`
  - Under `Export settings`, you can also configure to automatically export a dark and light version of the image, in case your published site supports dark and light modes.

### Hyperlinks and Drag & Drop support

![](https://github.com/zsviczian/obsidian-excalidraw-plugin/blob/master/images/excalidraw-modifiers.png)

#### Hyperlinks

- Supports hyperlinks, e.g.
  - `https://zsolt.blog`,
  - `[Obsidian](https://obsidian.md)`, and
  - Internal links, e.g. `[[My file in vault|Alias]]` in drawing text.
- Links will update when files are moved or renamed, if you have the Obsidian setting Files & Links/Automatically Update Internal Links enabled.
- Links in drawings will show up in the backlinks of documents.
- Transclusions are supported:
  - `![[myfile#^blockref]]` will convert the drawing into the transcluded text of the block
  - `![[myfile#section]]` also works, this will transclude the section.
  - You can also specify word wrapping for transcluded text by adding the max character count:
      in curly brackets right after the transclusion e.g. `![[myfile#^blockref]]{40}` will wrap text at 40 characters.
- For convenience, you can also use the command palette to insert links into drawings.
- <kbd>CTRL/CMD + hover</kbd> to bring up the Obsidian quick preview for the link. (On Mac, it is <kbd>CTRL+CMD+hover</kbd>).
- Using the block reference, you can also reference & transclude text that appears on drawings, in other documents.

#### Drag & Drop support

- You can drag files from the Obsidian file explorer, and they will become links to those files in Excalidraw. See the table above for the various modifier key combinations.
- Note: Anchoring an image to 100% of its size is a very niche feature with a very particular behavior that I built primarily for myself.
  - (even more so than other features in Excalidraw Obsidian - also built primarily for myself 😉).
  - This will reset your embedded image to 100% size every time you open the Excalidraw drawing,
      or in case you have embedded an Excalidraw drawing on your canvas inserted using this function,
      every time you update the embedded drawing, it will be scaled back to 100% size.
  - This means that even if you resize the image on the drawing, it will reset to 100% the next time you open
      the file, or you modify the original embedded object. This feature is useful when you
      decompose a drawing into separate Excalidraw files, but when combined onto a single canvas
      you want the individual pieces to maintain their actual sizes. I use this feature to
      construct book-on-a-page summaries from atomic drawings.
- You can drag and drop text from Markdown views onto Excalidraw.
- You can drag and drop web addresses from your browser, and they will become links.
- You can drag and drop YouTube links and thumbnails, and they will be YouTube links with thumbnails in Excalidraw.

### LaTeX

Insert LaTeX formulas using the Command Palette action "Insert LaTeX formula".
You can edit formulas either in Markdown view or by <kbd>CTRL/CMD + Click</kbd> on the formula.

### Image support

- On iOS and Android, you can add images from your camera by pressing the add image button in Excalidraw.
- You can copy/paste images into your drawing. Images will be saved in your vault.
- You can drag and drop images as explained above.
- URL link to images on the web: You can drag images from a webpage to Excalidraw. If you hold down the CTRL button while dropping the image to Excalidraw, the image will not be saved to your vault. Excalidraw will load the image from the URL. Note that if you do not have internet access or if these images are deleted from the internet, they will also disappear from your drawing.
- If you page an image URL to excalidraw (simply click copy on the url, then click paste on the excalidraw canvas), the image will be inserted with a link to the image on the web. Again, the image won't be saved to your vault, only the link.
- If you drop a YouTube video link, it will be converted into a thumbnail photo with an element link pointing to the video.

### Block referencing parts of images

For more details, see this [video](https://youtu.be/yZQoJg2RCKI)
- When referencing an element on the canvas in a link pointing to an Excalidraw file using
  - The elementId or the section header (i.e. a Text Element containing the `# <Section title>`)
      - e.g. `[[file#^elementID]]`,
  - You can add the `group=` prefix,
      - e.g. `[[file#^group=elementID]]` or
  - The `area=` prefix,
      - e.g. `[[file#area=Section heading]]`.
  - If the `group=` prefix is found, Excalidraw will select the group of elements in the
      same group as the element referenced by the elementID (block reference) or the section heading.
  - If the `area=` prefix is found, Excalidraw will insert a cutout of the image around the referenced element.
  - Note that the `area=` selector is not supported when embedding Excalidraw as a PNG into your markdown documents.
  - Referencing the elementID of a text element without the `group=` or `area=` prefix will
      transclude the element as plain text. Referencing a non-Text Element (e.g. rectangle,
      ellipse, etc.) without the `group=` or `area=` prefix will result in an Obsidian error.
      since these elementIds are not present in the Excalidraw markdown file as block
      references.

### Markdown

- Since 1.2.0, drawing files are stored in Markdown files.
  - You can add tags to drawings.
  - You can add metadata to the YAML front matter of drawings.
  - Anything you add between the frontmatter and the `# Text Elements` heading will be ignored by Excalidraw, i.e. you can add whatever you like here, and it will be preserved as part of the document.
  - Excalidraw documents now show up in graph view.
  - The following front matter keys will customize how the drawing is displayed - overriding general settings:
    - `excalidraw-link-prefix: "📍"` preview prefix for internal links
    - `excalidraw-url-prefix: "🌐"` preview prefix for external links
    - `excalidraw-link-brackets: true|false` whether or not to display brackets around links in preview
    - `excalidraw-default-mode: view|zen` Open this document in view mode or zen mode by defult. The default view mode is excellent for presentation slides.
  - Frontmatter tags to customize image export at a file level [519](https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/519). If these keys are present, they will override the default Excalidraw embed and export settings.
    - `excalidraw-export-transparent: true`:  true == Transparent / false == with background.
    - `excalidraw-export-dark`: true == Dark mode / false == light mode.
    - `excalidraw-export-padding`: Specify the export padding for the image.
    - `excalidraw-export-pngscale`: This only affects export to PNG. Specify the export scale for the image. The typical range is between 0.5 and 5, but you can experiment with other values as well.
- Since 1.6.13, enable "Decompress Excalidraw JSON in Markdown View" in the settings if you want to change any JSON content.

### Embed complete markdown files into your drawings

Drag the desired file from the Obsidian file explorer and hold down <kbd>SHIFT</kbd> while dropping the file onto the canvas.
- Use the command palette action: `Insert markdown file from vault`
- Use custom woff, woff2, or TTF font to display the document, you can set the default font to use under Excalidraw Settings.
- You can set a custom CSS for rendering the snapshot image of your markdown document. Only operating system-standard fonts are supported as the font-family ([Win10](https://docs.microsoft.com/en-us/typography/fonts/windows_10_font_list), [Mac & iOS](https://developer.apple.com/fonts/system-fonts/)), plus you can set one additional custom font using the setting explained above.
  - (for a demonstration, watch this [video](https://youtu.be/K6qZkTz8GHs) and check out this
  - [sample css](https://github.com/zsviczian/obsidian-excalidraw-plugin/discussions/281)).
  - To help with styling, you can observe the SVG snapshot of the markdown document created by Excalidraw.
    - Open Obsidian Developer Console (<kbd>CTRL+Shift+i</kbd>/<kbd>CMD+OPT+i</kbd>) and
    - Execute the following command: `ExcalidrawAutomate.mostRecentMarkdownSVG`
- You can control the appearance of the embedded markdown file on a file by file
  bases by adding the following front matter keys to your markdown document:
  - `excalidraw-font: Virgil|Cascadia|font_file_name.extension`
  - `excalidraw-font-color: css-color-name|#HEXcolor|any-other-html-standard-format`,
    - You can find css color names [here](https://www.w3schools.com/colors/colors_names.asp).
  - `excalidraw-border-color: css-color-name|#HEXcolor|any-other-html-standard-format`
  - `excalidraw-css: "css-filename|css snippet"`
- Switch to markdown view or use <kbd>WIN+CTRL</kbd>/<kbd>CMD+CTRL</kbd> click on the image to edit the properties of the embed:
  - `[[filename#^blockref|WIDTHxMAXHEIGHT]]`

### Custom Font, Custom Pen, OCR support, SVG import

- In plugin settings, you can add a custom fourth font. For more details, see this [video](https://youtu.be/eKFmrSQhFA4)
- The plugin includes OCR support using Taskbone OCR. For more details, see this [video](https://youtu.be/7gu4ETx7zro)
- You can convert SVG files into Excalidraw drawings (with some limitation). For more details, see this [video](https://youtu.be/vlC1-iBvIfo)
- You can define custom pens and higlighters and pin them to the sidebar. For more details, see this [video](https://youtu.be/OjNhjaH2KjI). Using ExcalidrawAutomate, you can add support for [auto-toggling](<ea-scripts/Auto Draw for Pen.md>) pen & support for [hardware eraser buttons](<ea-scripts/Hardware Eraser Support.md>).

### Script Engine

- Since 1.5.0, you can easily execute ExcalidrawAutomate macros and assign command palette shortcuts to them, using the ScriptEngine. You will find an intro video and a growing library of ready to install scripts [here](ea-scripts/README.md).
- You can organize scripts into groups on the Obsidian Tools Panel in Excalidraw by moving scripts and accompanying SVG icon files to folders. See the demo [video](https://youtu.be/wTtaXmRJ7wg?t=16).

### Other

- Left-handed mode
- Includes full
    - [QuickAdd](https://github.com/chhoumann/quickadd),
    - [Templater](https://silentvoid13.github.io/Templater/) and
    - [Dataview](https://blacksmithgu.github.io/obsidian-dataview/docs/api/intro/) support through ExcalidrawAutomate.
    - Check out the [detailed help + examples](https://zsviczian.github.io/obsidian-excalidraw-plugin/).
    - I also have a [YouTube ExcalidrawAutomate Playlist](https://www.youtube.com/playlist?list=PL6mqgtMZ4NP1IR4nXxSlMA4PA5E-qpyHZ) with lots of examples.
- REQUIRES AN OBSIDIAN SYNC SUBSCRIPTION: Full drawing file history and synchronization between devices
- Multilanguage support: if you'd like to help out by translating the plugin, please get in contact with me.

---

## Feedback, questions, ideas, problems

Join the conversation about the Excalidraw plugin on
[forum.obsidian.md](https://forum.obsidian.md/t/excalidraw-full-featured-sketching-plugin-in-obsidian)

Please head over to [GitHub](https://github.com/zsviczian/obsidian-excalidraw-plugin/issues) to
report a bug or request an enhancement.

---

## Say Thank You

If you are enjoying Excalidraw, then please support my work and enthusiasm by buying me a coffee on
[https://ko-fi/zsolt](https://ko-fi.com/zsolt).

Please also help spread the word by sharing about the Obsidian Excalidraw Plugin on Twitter, Reddit,
or any other social media platform you regularly use.

You can find me on Twitter [@zsviczian](https://twitter.com/zsviczian), and on my blog [zsolt.blog](https://zsolt.blog).

[<img style="float:left" src="https://user-images.githubusercontent.com/14358394/115450238-f39e8100-a21b-11eb-89d0-fa4b82cdbce8.png" width="200">](https://ko-fi.com/zsolt)

---

## Friends of Excalidraw
If you enjoy Excalidraw, consider giving [ExcaliBrain](https://github.com/zsviczian/excalibrain) a try (also available via Obsidian Community Plugins).

<a href="https://youtu.be/gOkniMkDPyM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/169708346-9e41289d-9536-43ec-8f70-2d2ad2d369d6.png" width="300"/></a>



================================================
FILE: AutomateHowTo.md
================================================
# Excalidraw Automate How To

Excalidraw Automate allows you to create Excalidraw drawings using the [Templater](https://github.com/SilentVoid13/Templater) plugin.

With a little work, using Excalidraw Automate you can generate simple mindmaps, fill out SVG forms, create customized charts, etc. based on documents in your vault.

You can access Excalidraw Automate via the ExcalidrawAutomate object. I recommend starting your Automate scripts with the following code.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
const ea = ExcalidrawAutomate;
ea.reset();
```

The first line creates a practical constant so you can avoid writing ExcalidrawAutomate 100x times.

The second line resets ExcalidrawAutomate to defaults. This is important as you will not know which template you executed before, thus you won't know what state you left Excalidraw in.

## Basic logic of using Excalidraw Automate
1. Set the styling of the elements you want to draw
2. Add elements. As you add elements, each new element is added one layer above the previous, thus in case of overlapping objects the later one will be on the top of the prior one.
3. Call `await ea.create();` to instantiate the drawing

You can change styling between adding different elements. My logic for separating element styling and creation is based on the assumption that you will probably set a stroke color, stroke style, stroke roughness, etc. and draw most of your elements using this. There would be no point in setting all these parameters each time you add an element.

### Before we dive deeper, here are two a simple example scripts
#### Create a new drawing with custom name, in a custom folder, using a template
This simple script gives you significant additional flexibility over Excalidraw Plugin settings to name your drawings, place them into folders, and to apply templates.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  await ea.create({
    filename    : tp.date.now("HH.mm"), 
    foldername  : tp.date.now("YYYY-MM-DD"),
    templatePath: "Excalidraw/Template1.excalidraw",
    onNewPane   : false
  });
%>
```

#### Create a simple drawing
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.addRect(-150,-50,450,300);
  ea.addText(-100,70,"Left to right");
  ea.addArrow([[-100,100],[100,100]]);

  ea.style.strokeColor = "red";
  ea.addText(100,-30,"top to bottom",{width:200,textAligh:"center"});
  ea.addArrow([[200,0],[200,200]]);
  await ea.create();
%>
```
The script will generate the following drawing:

![FristDemo](https://user-images.githubusercontent.com/14358394/116825643-6e5a8b00-ab90-11eb-9e3a-37c524620d0d.png)

## Attributes and functions at a glance
Here's the interface implemented by ExcalidrawAutomate:
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
ExcalidrawAutomate: {
  style: {
    strokeColor: string;
    backgroundColor: string;
    angle: number;
    fillStyle: FillStyle;
    strokeWidth: number;
    storkeStyle: StrokeStyle;
    roughness: number;
    opacity: number;
    strokeSharpness: StrokeSharpness;
    fontFamily: FontFamily;
    fontSize: number;
    textAlign: string;
    verticalAlign: string;
    startArrowHead: string;
    endArrowHead: string;
  }
  canvas: {theme: string, viewBackgroundColor: string};
  setFillStyle: Function;
  setStrokeStyle: Function;
  setStrokeSharpness: Function;
  setFontFamily: Function;
  setTheme: Function;
  addRect: Function;
  addDiamond: Function;
  addEllipse: Function;
  addText: Function;
  addLine: Function;
  addArrow: Function;
  connectObjects: Function;
  addToGroup: Function;
  toClipboard: Function;
  create: Function;
  createPNG: Function;
  createSVG: Function;
  clear: Function;
  reset: Function;
};
```

## Element Style
As you will notice, some styles have setter functions. This is to help you navigate the allowed values for the property. You do not need to use the setter function however, you can use set the value directly as well.

### strokeColor
String. The color of the line. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings, or  e.g. `#FF0000` for red.

### backgroundColor
String. This is the fill color of an object. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings e.g. `#FF0000` for red, or `transparent`.

### angle
Number. Rotation in radian. 90° == `Math.PI/2`.

### fillStyle, setFillStyle()
```typescript
type FillStyle = "hachure" | "cross-hatch" | "solid";
setFillStyle (val:number);
```
fillStyle is a string.

`setFillStyle()` accepts a number:
- 0: "hachure"
- 1: "cross-hatch"
- any other number: "solid"

### strokeWidth
Number, sets the width of the stroke.

### strokeStyle, setStrokeStyle()
```typescript
type StrokeStyle = "solid" | "dashed" | "dotted";
setStrokeStyle (val:number);
```
strokeStyle is a string. 

`setStrokeStyle()` accepts a number:
- 0: "solid"
- 1: "dashed"
- any other number: "dotted"

### roughness
Number. Called sloppiness in Excalidraw. Three values are accepted:
- 0: Architect
- 1: Artist
- 2: Cartoonist

### opacity
Number between 0 and 100. The opacity of an object, both stroke and fill.

### strokeSharpness, setStrokeSharpness()
```typescript
type StrokeSharpness = "round" | "sharp";
setStrokeSharpness(val:number);
```
strokeSharpness is a string.

"round" lines are curvey, "sharp" lines break at the turning point.

`setStrokeSharpness()` accepts a number:
- 0: "round"
- any other number: "sharp"

### fontFamily, setFontFamily()
Number. Valid values are 1,2 and 3.

`setFontFamily()` will also accept a number and return the name of the font.
- 1: "Virgil, Segoe UI Emoji"
- 2: "Helvetica, Segoe UI Emoji"
- 3: "Cascadia, Segoe UI Emoji"

### fontSize
Number. Default value is 20 px

### textAlign
String. Alignment of the text horizontally. Valid values are "left", "center", "right".

This is relevant when setting a fix width using the `addText()` function.

### verticalAlign
String. Alignment of the text vertically. Valid values are "top" and "middle".

This is relevant when setting a fix height using the `addText()` function.

### startArrowHead, endArrowHead
String. Valid values are "arrow", "bar", "dot", and "none". Specifies the beginning and ending of an arrow.

This is relevant when using the `addArrow()` and the `connectObjects()` functions.

## canvas
Sets the properties of the canvas. 

### theme, setTheme()
String. Valid values are "light" and "dark".

`setTheme()` accepts a number:
- 0: "light"
- any other number: "dark"

### viewBackgroundColor
String. This is the fill color of an object. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings e.g. `#FF0000` for red, or `transparent`.

## Adding objects
These functions will add objects to your drawing. The canvas is infinite, and it accepts negative and positive X and Y values. X values increase left to right, Y values increase top to bottom.

![coordinates](https://user-images.githubusercontent.com/14358394/116825632-6569b980-ab90-11eb-827b-ada598e91e46.png)

### addRect(), addDiamond(), addEllipse()
```typescript
addRect(topX:number, topY:number, width:number, height:number):string
addDiamond(topX:number, topY:number, width:number, height:number):string
addEllipse(topX:number, topY:number, width:number, height:number):string
```
Returns the `id` of the object. The `id` is required when connecting objects with lines. See later.

### addText
```typescript
addText(topX:number, topY:number, text:string, formatting?:{width:number, height:number,textAlign: string, verticalAlign:string, box: boolean, boxPadding: number}):string
```

Adds text to the drawing. 

Formatting parameters are optional:
- If `width` and `height` are not specified, the function will calculate the width and height based on the fontFamily, the fontSize and the text provided.
- In case you want to position a text in the center compared to other elements on the drawing, you can provide a fixed height and width, and you can also specify `textAlign` and `verticalAlign` as described above. e.g.: `{width:500, textAlign:"center"}`
- If you want to add a box around the text, set `{box:true}`

Returns the `id` of the object. The `id` is required when connecting objects with lines. See later. If `{box:true}` then returns the id of the enclosing box.

### addLine()
```typescript
addLine(points: [[x:number,y:number]]):void
```
Adds a line following the points provided. Must include at least two points `points.length >= 2`. If more than 2 points are provided the interim points will be added as breakpoints. The line will break with angles if `strokeSharpness` is set to "sharp" and will be curvey if it is set to "round".

### addArrow()
```typescript
addArrow(points: [[x:number,y:number]],formatting?:{startArrowHead:string,endArrowHead:string,startObjectId:string,endObjectId:string}):void
```

Adds an arrow following the points provided. Must include at least two points `points.length >= 2`. If more than 2 points are provided the interim points will be added as breakpoints. The line will break with angles if element `style.strokeSharpness` is set to "sharp" and will be curvey if it is set to "round".

`startArrowHead` and `endArrowHead` specify the type of arrow head to use, as described above. Valid values are "none", "arrow", "dot", and "bar". e.g. `{startArrowHead: "dot", endArrowHead: "arrow"}`

`startObjectId` and `endObjectId` are the object id's of connected objects. I recommend using `connectObjects` instead calling addArrow() for the purpose of connecting objects.

### connectObjects()
```typescript
declare type ConnectionPoint = "top"|"bottom"|"left"|"right";
connectObjects(objectA: string, connectionA: ConnectionPoint, objectB: string, connectionB: ConnectionPoint, formatting?:{numberOfPoints: number,startArrowHead:string,endArrowHead:string, padding: number}):void
```
Connects two objects with an arrow.

`objectA` and `objectB` are strings. These are the ids of the objects to connect. These IDs are returned by addRect(), addDiamond(), addEllipse() and addText() when creating those objects.

`connectionA` and `connectionB` specify where to connect on the object. Valid values are: "top", "bottom", "left", and "right".

`numberOfPoints` set the number of interim break points for the line. Default value is zero, meaning there will be no breakpoint in between the start and the end points of the arrow. When moving objects on the drawing, these breakpoints will influence how the line is rerouted by Excalidraw.

`startArrowHead` and `endArrowHead` work as described for `addArrow()` above.

### addToGroup()
```typescript
addToGroup(objectIds:[]):void
```
Groups objects listed in `objectIds`.

## Utility functions
### clear()
`clear()` will clear objects from cache, but will retain element style settings.

### reset()
`reset()` will first call `clear()` and then reset element style to defaults.

### toClipboard()
```typescript
async toClipboard(templatePath?:string)
```
Places the generated drawing to the clipboard. Useful when you don't want to create a new drawing, but want to paste additional items onto an existing drawing.

### create()
```typescript
async create(params?:{filename: string, foldername:string, templatePath:string, onNewPane: boolean})
```
Creates the drawing and opens it.

`filename` is the filename without extension of the drawing to be created. If `null`, then Excalidraw will generate a filename.

`foldername` is the folder where the file should be created. If `null` then the default folder for new drawings will be used according to Excalidraw settings.

`templatePath` the filename including full path and extension for a template file to use. This template file will be added as the base layer, all additional objects added via ExcalidrawAutomate will appear on top of elements in the template. If `null` then no template will be used, i.e. an empty white drawing will be the base for adding objects.

`onNewPane` defines where the new drawing should be created. `false` will open the drawing on the current active leaf. `true` will open the drawing by vertically splitting the current leaf.

Example:
```javascript
create({filename:"my drawing", foldername:"myfolder/subfolder/", templatePath: "Excalidraw/template.excalidraw", onNewPane: true});
```
### createSVG()
```typescript
async createSVG(templatePath?:string)
```
Returns an HTML SVGSVGElement containing the generated drawing.

### createPNG()
```typescript
async createPNG(templatePath?:string)
```
Returns a blob containing a PNG image of the generated drawing.

## Examples
### Insert new drawing into currently edited document
This template will prompt you for the title of the drawing. It will create a new drawing with the provided title, and in the folder of the document you were editing. It will then transclude the new drawing at the cursor location and open the new drawing in a new workspace leaf by splitting the current leaf.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const defaultTitle = tp.date.now("HHmm")+' '+tp.file.title;
  const title = await tp.system.prompt("Title of the drawing?", defaultTitle);
  const folder = tp.file.folder(true);
  const transcludePath = (folder== '/' ? '' : folder + '/') + title + '.excalidraw';
  tR = String.fromCharCode(96,96,96)+'excalidraw\n[['+transcludePath+']]\n'+String.fromCharCode(96,96,96);
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.setTheme(1); //set Theme to dark
  await ea.create({
    filename : title,
    foldername : folder,
    //templatePath: 'Excalidraw/Template.excalidraw', //uncomment if you want to use a template
    onNewPane : true
  });
%>
```

### Connect objects
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.addText(-130,-100,"Connecting two objects");
  const a = ea.addRect(-100,-100,100,100);
  const b = ea.addEllipse(200,200,100,100);
  ea.connectObjects(a,"bottom",b,"left",{numberOfPoints: 2}); //see how the line breaks differently when moving objects around
  ea.style.strokeColor = "red";
  ea.connectObjects(a,"right",b,"top",1);
  await ea.create();
%>
```
### Using a template
This example is similar to the first one, but rotated 90°, and using a template, plus specifying a filename and folder to save the drawing, and opening the new drawing in a new pane.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.style.angle = Math.PI/2; 
  ea.style.strokeWidth = 3.5;
  ea.addRect(-150,-50,450,300);
  ea.addText(-100,70,"Left to right");
  ea.addArrow([[-100,100],[100,100]]);

  ea.style.strokeColor = "red";
  await ea.addText(100,-30,"top to bottom",{width:200,textAlign:"center"});
  ea.addArrow([[200,0],[200,200]]);
  await ea.create({filename:"My Drawing",foldername:"myfolder/fordemo/",templatePath:"Excalidraw/Template2.excalidraw",onNewPane:true});
%>
```

### Generating a simple mindmap from a text outline
This is a slightly more elaborate example. This will generate an a mindmap from a tabulated outline.

![Drawing 2021-05-05 20 52 34](https://user-images.githubusercontent.com/14358394/117194124-00a69d00-ade4-11eb-8b75-5e18a9cbc3cd.png)

Example input:
```
- Test 1
	- Test 1.1
- Test 2
	- Test 2.1
	- Test 2.2 
		- Test 2.2.1
		- Test 2.2.2
		- Test 2.2.3
			- Test 2.2.3.1
- Test 3
	- Test 3.1
```

The script:

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
const IDX = Object.freeze({"depth":0, "text":1, "parent":2, "size":3, "children": 4, "objectId":5});

//check if an editor is the active view
const editor = this.app.workspace.activeLeaf?.view?.editor;
if(!editor) return;

//initialize the tree with the title of the document as the first element
let tree = [[0,this.app.workspace.activeLeaf?.view?.getDisplayText(),-1,0,[],0]];
const linecount = editor.lineCount();

//helper function, use regex to calculate indentation depth, and to get line text
function getLineProps (i) {
  props = editor.getLine(i).match(/^(\t*)-\s+(.*)/);
  return [props[1].length+1, props[2]];
}

//a vector that will hold last valid parent for each depth
let parents = [0];

//load outline into tree
for(i=0;i<linecount;i++) {
  [depth,text] = getLineProps(i);
  if(depth>parents.length) parents.push(i+1);
  else parents[depth] = i+1;
  tree.push([depth,text,parents[depth-1],1,[]]);
  tree[parents[depth-1]][IDX.children].push(i+1);
}

//recursive function to crawl the tree and identify height aka. size of each node
function crawlTree(i) {
  if(i>linecount) return 0;
  size = 0;
  if((i+1<=linecount && tree[i+1][IDX.depth] <= tree[i][IDX.depth])|| i == linecount) { //I am a leaf
    tree[i][IDX.size] = 1; 
    return 1; 
  }
  tree[i][IDX.children].forEach((node)=>{ 
    size += crawlTree(node);
  });
  tree[i][IDX.size] = size; 
  return size;   
}

crawlTree(0);

//Build the mindmap in Excalidraw
const width = 300;
const height = 100;
const ea = ExcalidrawAutomate;
ea.reset();

//stores position offset of branch/leaf in height units
offsets = [0];

for(i=0;i<=linecount;i++) {
  depth = tree[i][IDX.depth];
  if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16);
  tree[i][IDX.objectId] = ea.addText(depth*width,((tree[i][IDX.size]/2)+offsets[depth])*height,tree[i][IDX.text],{box:true});  
  //set child offset equal to parent offset
  if((depth+1)>offsets.length) offsets.push(offsets[depth]);
  else offsets[depth+1] = offsets[depth];
  offsets[depth] += tree[i][IDX.size];
  if(tree[i][IDX.parent]!=-1) {
    ea.connectObjects(tree[tree[i][IDX.parent]][IDX.objectId],"right",tree[i][IDX.objectId],"left",{startArrowHead: 'dot'});
  }
}

await ea.create({onNewPane: true});
%>
```



================================================
FILE: esbuild.config.json
================================================
{
  "minify": true
}


================================================
FILE: manifest-beta.json
================================================
{
	"id": "obsidian-excalidraw-plugin",
	"name": "Excalidraw",
  "version": "2.15.0",
  "minAppVersion": "1.5.7",
	"description": "An Obsidian plugin to edit and view Excalidraw drawings",
	"author": "Zsolt Viczian",
	"authorUrl": "https://excalidraw-obsidian.online",
	"isDesktopOnly": false
}



================================================
FILE: manifest.json
================================================
{
  "id": "obsidian-excalidraw-plugin",
  "name": "Excalidraw",
  "version": "2.15.0",
  "minAppVersion": "1.5.7",
  "description": "An Obsidian plugin to edit and view Excalidraw drawings",
  "author": "Zsolt Viczian",
  "authorUrl": "https://excalidraw-obsidian.online",
  "fundingUrl": "https://ko-fi.com/zsolt",
  "helpUrl": "https://github.com/zsviczian/obsidian-excalidraw-plugin#readme",
  "isDesktopOnly": false
}


================================================
FILE: package.json
================================================
{
  "name": "obsidian-excalidraw-plugin",
  "version": "2.2.5",
  "description": "This is an Obsidian.md plugin that lets you view and edit Excalidraw drawings",
  "main": "lib/index.js",
  "types": "lib/index.d.ts",
  "files": [
    "lib/**/*"
  ],
  "scripts": {
    "dev": "cross-env NODE_ENV=development rollup --config rollup.config.js",
    "build": "cross-env NODE_ENV=production rollup --config rollup.config.js",
    "lib": "cross-env NODE_ENV=lib rollup --config rollup.config.js",
    "code:fix": "eslint --max-warnings=0 --ext .ts,.tsx ./src --fix",
    "madge": "madge --circular .",
    "build:mathjax": "cd MathjaxToSVG && npm run build",
    "build:all": "npm run build:mathjax && npm run build",
    "dev:mathjax": "cd MathjaxToSVG && npm run dev",
    "dev:all": "npm run dev:mathjax && npm run dev",
    "doc": "node scripts/generate-script-library.js"
  },
  "keywords": [],
  "author": "",
  "license": "MIT",
  "dependencies": {
    "@popperjs/core": "^2.11.8",
    "@zsviczian/excalidraw": "0.18.0-34",
    "chroma-js": "^3.1.2",
    "clsx": "^2.0.0",
    "@zsviczian/colormaster": "^1.2.2",
    "gl-matrix": "^3.4.3",
    "js-yaml": "^4.1.0",
    "lucide-react": "^0.479.0",
    "mathjax-full": "^3.2.2",
    "monkey-around": "^2.3.0",
    "nanoid": "^4.0.2",
    "opentype.js": "^1.3.4",
    "polybooljs": "^1.2.0",
    "react": "^18.2.0",
    "react-dom": "^18.2.0",
    "roughjs": "^4.5.2",
    "woff2sfnt-sfnt2woff": "^1.0.0",
    "es6-promise-pool": "2.5.0"
  },
  "devDependencies": {
    "jsesc": "^3.0.2",
    "@babel/core": "^7.22.9",
    "@babel/preset-env": "^7.22.10",
    "@babel/preset-react": "^7.22.5",
    "@codemirror/commands": "^6.3.3",
    "@codemirror/language": "^6.10.0",
    "@codemirror/search": "^6.5.5",
    "@codemirror/state": "^6.4.0",
    "@codemirror/view": "^6.23.0",
    "@excalidraw/eslint-config": "^1.0.3",
    "@excalidraw/prettier-config": "^1.0.2",
    "@rollup/plugin-babel": "^6.0.3",
    "@rollup/plugin-commonjs": "^26.0.1",
    "@rollup/plugin-node-resolve": "^15.2.3",
    "@rollup/plugin-replace": "^5.0.2",
    "@rollup/plugin-typescript": "^12.1.2",
    "@rollup/plugin-json": "^6.1.0",
    "@types/chroma-js": "^3.1.1",
    "@types/js-beautify": "^1.14.0",
    "@types/js-yaml": "^4.0.9",
    "@types/node": "^20.10.5",
    "@types/opentype.js": "^1.3.8",
    "@types/react": "^18.2.45",
    "@types/react-dom": "^18.2.18",
    "@zerollup/ts-transform-paths": "^1.7.18",
    "cross-env": "^7.0.3",
    "cssnano": "^6.0.2",
    "dotenv": "^16.4.5",
    "eslint-config-prettier": "^9.0.0",
    "eslint-plugin-prettier": "^5.0.0",
    "lz-string": "^1.5.0",
    "obsidian": "^1.7.2",
    "prettier": "^3.0.1",
    "rollup": "^2.70.1",
    "rollup-plugin-copy": "^3.5.0",
    "@zsviczian/rollup-plugin-postprocess": "^1.0.3",
    "rollup-plugin-terser": "^7.0.2",
    "rollup-plugin-typescript2": "^0.36.0",
    "tslib": "^2.8.1",
    "ttypescript": "^1.5.15",
    "typescript": "^5.7.3",
    "fs-extra": "^11.2.0",
    "uglify-js": "^3.19.3"
  },
  "resolutions": {
    "@typescript-eslint/typescript-estree": "5.3.0"
  },
  "prettier": "@excalidraw/prettier-config",
  "engines": {
    "node": ">=20.0.0",
    "npm": ">=10.0.0"
  }
}



================================================
FILE: rollup.config.js
================================================
import { nodeResolve } from '@rollup/plugin-node-resolve';
import commonjs from '@rollup/plugin-commonjs';
import replace from "@rollup/plugin-replace";
import { terser } from "rollup-plugin-terser";
import copy from "rollup-plugin-copy";
import typescript2 from "rollup-plugin-typescript2";
import fs from 'fs';
import path from 'path';
import LZString from 'lz-string';
import postprocess from '@zsviczian/rollup-plugin-postprocess';
import cssnano from 'cssnano';
import jsesc from 'jsesc';
import { minify } from 'uglify-js';
import json from '@rollup/plugin-json';

// Load environment variables
import dotenv from 'dotenv';
dotenv.config();

const DIST_FOLDER = 'dist';
const absolutePath = path.resolve(DIST_FOLDER);
fs.mkdirSync(absolutePath, { recursive: true });
const isProd = (process.env.NODE_ENV === "production");
const isLib = (process.env.NODE_ENV === "lib");
console.log(`Running: ${process.env.NODE_ENV}; isProd: ${isProd}; isLib: ${isLib}`);


// Excalidraw React 19 compatiblity shim
// Create JSX runtime compatibility layer
const jsxRuntimeShim = `
  const jsx = (type, props, key) => {
    return React.createElement(type, props);
  };
  const jsxs = (type, props, key) => {
    return React.createElement(type, props);
  };
  const Fragment = React.Fragment;
  React.jsx = jsx;
  React.jsxs = jsxs;
  React.Fragment = Fragment;
  React.jsxRuntime = { jsx, jsxs, Fragment };
  window.__WEBPACK_EXTERNAL_MODULE_react_jsx_runtime__ = { jsx, jsxs, Fragment };
  window.__WEBPACK_EXTERNAL_MODULE_react_jsx_dev_runtime__ = { jsx, jsxs, Fragment, jsxDEV: jsx };
  window['react/jsx-runtime'] = { jsx, jsxs, Fragment };
  window['react/jsx-dev-runtime'] = { jsx, jsxs, Fragment, jsxDEV: jsx };
`;



const mathjaxtosvg_pkg = isLib ? "" : fs.readFileSync("./MathjaxToSVG/dist/index.js", "utf8");

const LANGUAGES = ['ru', 'zh-cn', 'zh-tw', 'es']; //english is not compressed as it is always loaded by default

function trimLastSemicolon(input) {
  if (input.endsWith(";")) {
    return input.slice(0, -1);
  }
  return input;
}

function minifyCode(code) {
  const minified = minify(code, {
    compress: {
      //https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/2170
      reduce_vars: false,
    },
    mangle: true,
    output: {
      comments: false,
      beautify: false,
    }
  });

  if (minified.error) {
    throw new Error(minified.error);
  }
  return minified.code;
}

function compressLanguageFile(lang) {
  const inputDir = "./src/lang/locale";
  const filePath = `${inputDir}/${lang}.ts`;
  let content = fs.readFileSync(filePath, "utf-8");
  content = trimLastSemicolon(content.split("export default")[1].trim());
  return LZString.compressToBase64(minifyCode(`x = ${content};`));
}

const excalidraw_pkg = isLib ? "" : minifyCode(isProd
  ? fs.readFileSync("./node_modules/@zsviczian/excalidraw/dist/excalidraw.production.min.js", "utf8")
  : fs.readFileSync("./node_modules/@zsviczian/excalidraw/dist/excalidraw.development.js", "utf8"));
const react_pkg = isLib ? "" : minifyCode(isProd
  ? fs.readFileSync("./node_modules/react/umd/react.production.min.js", "utf8")
  : fs.readFileSync("./node_modules/react/umd/react.development.js", "utf8"));
const reactdom_pkg = isLib ? "" : minifyCode(isProd
  ? fs.readFileSync("./node_modules/react-dom/umd/react-dom.production.min.js", "utf8")
  : fs.readFileSync("./node_modules/react-dom/umd/react-dom.development.js", "utf8"));

const lzstring_pkg = isLib ? "" : fs.readFileSync("./node_modules/lz-string/libs/lz-string.min.js", "utf8");
if (!isLib) {
  const excalidraw_styles = isProd
    ? fs.readFileSync("./node_modules/@zsviczian/excalidraw/dist/styles.production.css", "utf8")
    : fs.readFileSync("./node_modules/@zsviczian/excalidraw/dist/styles.development.css", "utf8");
  const plugin_styles = fs.readFileSync("./styles.css", "utf8");
  const styles = plugin_styles + excalidraw_styles;
  cssnano()
    .process(styles) // Process the CSS
    .then(result => {
      fs.writeFileSync(`./${DIST_FOLDER}/styles.css`, result.css);
    })
    .catch(error => {
      console.error('Error while processing CSS:', error);
    });
}

const manifestStr = isLib ? "" : fs.readFileSync("manifest.json", "utf-8");
const manifest = isLib ? {} : JSON.parse(manifestStr);
if (!isLib) {
  console.log(manifest.version);
}

const packageString = isLib
  ? ""
  : ';const INITIAL_TIMESTAMP=Date.now();' + lzstring_pkg +
  '\nlet REACT_PACKAGES = `' +
  jsesc(react_pkg + reactdom_pkg + jsxRuntimeShim, { quotes: 'backtick' }) +
  '`;\n' +
  'const unpackExcalidraw = () => LZString.decompressFromBase64("' + LZString.compressToBase64(excalidraw_pkg) + '");\n' +
  'let {react, reactDOM } = new Function(`${REACT_PACKAGES}; return {react: React, reactDOM: ReactDOM};`)();\n' +
  'let excalidrawLib = {};\n' +
  'const loadMathjaxToSVG = () => new Function(`${LZString.decompressFromBase64("' + LZString.compressToBase64(mathjaxtosvg_pkg) + '")}; return MathjaxToSVG;`)();\n' +
  `const PLUGIN_LANGUAGES = {${LANGUAGES.map(lang => `"${lang}": "${compressLanguageFile(lang)}"`).join(",")}};\n` +
  'const PLUGIN_VERSION="' + manifest.version + '";';

const BASE_CONFIG = {
  input: 'src/core/main.ts',
  external: [
    '@codemirror/autocomplete',
    '@codemirror/collab',
    '@codemirror/commands',
    '@codemirror/language',
    '@codemirror/lint',
    '@codemirror/search',
    '@codemirror/state',
    '@codemirror/view',
    '@lezer/common',
    '@lezer/highlight',
    '@lezer/lr',
    'obsidian',
    '@zsviczian/excalidraw',
    'react',
    'react-dom'
  ],
};

const getRollupPlugins = (tsconfig, ...plugins) => [
  typescript2(tsconfig),
  json(),
  replace({
    preventAssignment: true,
    "process.env.NODE_ENV": JSON.stringify(process.env.NODE_ENV),
  }),
  commonjs(),
  nodeResolve({ browser: true, preferBuiltins: false }),
].concat(plugins);

const BUILD_CONFIG = {
  ...BASE_CONFIG,
  output: {
    dir: DIST_FOLDER,
    entryFileNames: 'main.js',
    format: 'cjs',
    exports: 'default',
    inlineDynamicImports: true, // Add this line only
  },
  plugins: getRollupPlugins(
    {
      tsconfig: isProd ? "tsconfig.json" : "tsconfig.dev.json",
      sourcemap: !isProd,
      clean: true,
      //verbosity: isProd ? 1 : 2,
    },
    ...(isProd ? [
      terser({
        toplevel: false,
        compress: { passes: 2 },
        format: {
          comments: false, // Remove all comments
        },
      }),
      postprocess([
        [/React=require\("react"\),state=require\("@codemirror\/state"\),view=require\("@codemirror\/view"\)/,
        `state=require("@codemirror/state"),view=require("@codemirror/view")` + packageString],
      ]),
    ] : [
      postprocess([ [/var React = require\('react'\);/, packageString] ]),
    ]),
    copy({
      targets: [ { src: 'manifest.json', dest: DIST_FOLDER } ],
      verbose: true,
    }),
  ),
};

const LIB_CONFIG = {
  ...BASE_CONFIG,
  input: "src/core/index.ts",
  output: {
    dir: "lib",
    sourcemap: false,
    format: "cjs",
    name: "Excalidraw (Library)",
  },
  plugins: getRollupPlugins(
    { tsconfig: "tsconfig-lib.json" },
    copy({ targets: [{ src: "src/*.d.ts", dest: "lib/typings" }] })
  ),
};

let config = [];
if (process.env.NODE_ENV === "lib") {
  config.push(LIB_CONFIG);
} else {
  config.push(BUILD_CONFIG);
}

export default config;



================================================
FILE: styles.css
================================================
.App {
    font-family: sans-serif;
    text-align: center;
  }
    
  .excalidraw-wrapper {
    height: 100%;
    margin: 0px;
    background-color: var(--background-primary);
    position:relative;
  }
  
  .context-menu-option__shortcut {
      background-color: transparent !important;
  }

.block-language-excalidraw {
  text-align:center;
}

.excalidraw .github-corner {
  display: none;
}

.excalidraw-embedded-img {
  width: 100%;
}

.excalidraw-svg-right-wrap {
  float: right;
  margin: 0px 0px 20px 20px;
  width: 100%;
}

.excalidraw-svg-left-wrap {
  float: left;
  margin: 0px 35px 20px 0px;
  width: 100%;
}

.excalidraw-svg-right {
  float: right;
}

.excalidraw-svg-center {
  text-align: center;
  margin: auto;
  width: 100%;
}

.excalidraw-svg-left {
  float: left;
}

div.excalidraw-svg-right,
div.excalidraw-svg-left {
  display: table;
  width: 100%;
}

button.ToolIcon_type_button[title="Export"] {
  display:none;
}

.excalidraw-prompt-div {
  display: flex;
  max-width: 800px;
}

.excalidraw-prompt-form {
  display: flex;
  flex-grow: 1;
}

.excalidraw-prompt-input {
  flex-grow: 1;
}

.excalidraw-prompt-button {
  width: 9em;
}

.excalidraw-export-button {
  width: 9em;
  margin-left: 10px;
}

.excalidraw-prompt-buttons-div {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-evenly;
}

.excalidraw-export-buttons-div {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: right;
}

li[data-testid] {
  border: 0 !important;
  margin: 0 !important;
  padding: 0 !important;
  width: 100% !important;
}

.excalidraw .context-menu-option-separator {
  margin: 4px !important;
}

.excalidraw .popover {
  padding: 0 !important;
  border-color: transparent !important;
  border: 0 !important;
  box-shadow: 0 !important;
  background-color: transparent !important;
  overflow-y: auto !important;
} 

.excalidraw .popover {
  position: fixed !important;
}

.disable-zen-mode--visible {
  color: var(--text-primary-color);
}

.disable-zen-mode {
  width: 9em !important;
}

.ex-coffee-div {
	text-align: center;
	margin-bottom: 10px;
}

.excalidraw-scriptengine-install td>img {
  width: 100%;
  max-width:800px;
}

.excalidraw-scriptengine-install img.coffee {
  width: 130px;
}

.excalidraw-scriptengine-install tr {
  vertical-align: top;
}

.excalidraw-scriptengine-install table {
  max-width: 130ch;
}

.excalidraw-scriptengine-install td.label {
  min-width: 11ch;
  font-weight: bold;
  padding-right: 5px;
}

.excalidraw-scriptengine-install td.data {
  width: 100%;
}

.excalidraw-scriptengine-install .modal-content {
  max-width: 130ch;
  user-select: text;
}

.excalidraw-scriptengine-install .modal {
  max-height:90%;
  width: auto;
}

.excalidraw-prompt-center {
  text-align: center !important;
}

.excalidraw-prompt-center button {
  margin: 0 10px;
}

.excalidraw-prompt-center.filepath {
  text-align: center;
  font-weight: bold;
  margin-bottom: 2em;
}

.excalidraw-dirty {
  color: red;
}

.workspace-leaf-content .excalidraw-view {
  padding: 0px 1px; /*1px so on ipad swipe in from left and right still works*/
  overflow: hidden;
}

.excalidraw-videoWrapper {
  max-width:600px;
}
.excalidraw-videoWrapper.settings {
  max-width:340px;
}

.excalidraw-videoWrapper div{
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  margin: 0 auto;
}

.excalidraw-videoWrapper.settings iframe {
  position: relative;
  margin-bottom: 1rem;
}

.excalidraw-videoWrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

.excalidraw-release .modal-content{
  padding-right: 5px;
  margin-right: -5px;
  user-select: text;
}

.excalidraw-release .modal {
  max-height: 80%;
  max-width: 42em;
}

.excalidraw .Island .scrollbar {
  --scrollbar-thumb-bg: silver;
}

.excalidraw .ToolIcon__icon img{
  height: 1rem;
}

.excalidraw-scriptengine-install tbody>tr>td>div>img {
  height:20px;
  background-color: silver;
  padding: 2px;
}

.excalidraw-scriptengine-install tbody>tr>td>div {
  width: 50px;
  display: inline-block;
}

.excalidraw-release p>a>img {
  width: 100%
}

.excalidraw .context-menu-option {
  box-shadow: none;
}

textarea.excalidraw-wysiwyg {
  border: none;
  outline: none;
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  box-shadow: none;
  border-radius: 0;  
}

.is-tablet .excalidraw button,
.is-mobile .excalidraw button {
  padding: initial;
  height: 1.8rem;
}

.excalidraw button,
.ToolIcon button {
  box-shadow: none;
  justify-content: initial;
}

.excalidraw {
  --default-button-size: 2rem !important;
  --default-icon-size: 1rem !important;
  --lg-button-size: 1.8rem !important;
  --lg-icon-size: 1rem !important;
}

.excalidraw .tray-zoom {
  pointer-events: initial;
  padding-bottom: 0.05rem;
  padding-top: 0.05rem;
}

.excalidraw-container.theme--dark {
  background-color: #121212;
  color: #fff;
}

/* https://discordapp.com/channels/686053708261228577/989603365606531104/1041266507256184863 */
/*.workspace-leaf {
	contain: none !important;
}*/

.color-picker-content {
  overflow-y: auto;
  max-height: 10rem;
}

.excalidraw .FixedSideContainer_side_top {
  top: 0.3rem;
}

.excalidraw .ToolIcon__keybinding {
  font-size: 0.45rem !important;
}

.Island > .Stack > .Stack {
  padding:0.2rem;
}

label.color-input-container > input {
  max-width: 5rem;
}

.excalidraw .FixedSideContainer_side_top {
  left: 10px !important;
  top: 10px !important;
  right: 10px !important;
  bottom: 10px !important;
}

.excalidraw-hidden {
  display: none !important;
}

.excalidraw .App-toolbar-content .dropdown-menu {
  max-height: 70vh;
  overflow-y: auto;
}

.excalidraw .selected-shape-actions .panelColumn,
.excalidraw .App-mobile-menu .panelColumn
 {
  max-height: 70vh;
  overflow-y: auto;
}

.excalidraw .App-mobile-menu {
  width: 12.5rem !important;
}

.excalidraw .panelColumn .buttonList {
  max-width: 13rem;
}

.excalidraw button {
  width: initial;
}

.excalidraw input[type="color"] {
  width: 1.65rem;
  height: 1.65rem;
}

.excalidraw input[type="color"]::-webkit-color-swatch {
    height: 1.65rem;
}


.excalidraw input[type="color"]::-webkit-color-swatch-wrapper {
  padding: 0;
}

.excalidraw-settings input[type="text"] {
  min-width: 10em;
}

div.excalidraw-draginfo {
  position: absolute;
  z-index: 1000;
  color: var(--text-normal);
  padding: 3px;
  background: var(--color-base-40);
  display: block;
  border-radius: 5px;
}

.excalidraw [data-radix-popper-content-wrapper] {
  /*Overrides position:fixed in popover*/
  position: absolute !important;
}

/*Arrow Picker Popover Overflow*/
/*
.excalidraw .selected-shape-actions .Island.App-menu__left,
.excalidraw .selected-shape-actions .Island.App-menu__left .panelColumn,
.excalidraw .Island .App-mobile-menu,
.excalidraw .Island .App-mobile-menu .panelColumn {
	overflow: visible;
}*/

.excalidraw__embeddable-container .view-header {
  display: none !important;
}

.excalidraw__embeddable-container input {
  background: initial;
}

.excalidraw .embeddable-menu {
    width: fit-content;
    height: fit-content;
    position: absolute;
    display: block;
    z-index: var(--zIndex-layerUI);
}

.excalidraw .welcome-screen-center__logo svg {
  width: 5rem !important;
}

.excalidraw-image-wrapper {
  text-align: center;
}

.excalidraw-image-wrapper img {
  margin: auto;
}


.modal-content.excalidraw-scriptengine-install .hit-count {
  margin-left: 0.5em;
  white-space: nowrap;
  font-size: smaller;
}

.modal-content.excalidraw-scriptengine-install .active-highlight {
  border: 2px solid var(--color-accent-2);
  background-color: var(--color-accent);
}

.excalidraw-svg svg a {
  text-decoration: none;
}

.excalidraw .Modal {
  background-color: initial;
  border: initial;
  max-width: initial;
  max-height: initial;
  width: initial;
  height: initial;
}

summary.excalidraw-setting-h1 {
  font-variant: var(--h1-variant);
  letter-spacing: -0.015em;
  line-height: var(--h1-line-height);
  font-size: var(--h1-size);
  color: var(--h1-color);
  font-weight: var(--h1-weight);
  font-style: var(--h1-style);
  font-family: var(--h1-font);
  /*margin-block-start: var(--p-spacing);*/
  margin-block-end: var(--p-spacing);
}

summary.excalidraw-setting-h3 {
  font-variant: var(--h3-variant);
  letter-spacing: -0.015em;
  line-height: var(--h3-line-height);
  font-size: var(--h3-size);
  color: var(--h3-color);
  font-weight: var(--h3-weight);
  font-style: var(--h3-style);
  font-family: var(--h3-font);
  margin-block-start: var(--p-spacing);
  margin-block-end: var(--p-spacing);
}

summary.excalidraw-setting-h4 {
  font-variant: var(--h4-variant);
  letter-spacing: -0.015em;
  line-height: var(--h4-line-height);
  font-size: var(--h4-size);
  color: var(--h4-color);
  font-weight: var(--h4-weight);
  font-style: var(--h4-style);
  font-family: var(--h4-font);
  margin-block-start: var(--p-spacing);
  margin-block-end: var(--p-spacing);
}

hr.excalidraw-setting-hr {
  margin: 1rem 0rem 0rem 0rem;
}

.excalidraw-mdEmbed-hideFilename .mod-header {
  display: none;
}

.excalidraw__embeddable-container .canvas-node:not(.is-editing).transparent {
  ::-webkit-scrollbar,
  ::-webkit-scrollbar-horizontal {
    display: none;
  }
}

/* 
//https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/1456
.canvas-node:not(.is-editing):has(.excalidraw-canvas-immersive) {
  ::-webkit-scrollbar,
  ::-webkit-scrollbar-horizontal {
    display: none;
  }
  background-color: transparent !important;
}

.canvas-node:not(.is-editing) .canvas-node-container:has(.excalidraw-canvas-immersive) {
  border:       unset;
  box-shadow:   unset;
}
*/

.excalidraw .canvas-node .ex-md-font-hand-drawn {
  --font-text: "Virgil";
}

.excalidraw .canvas-node .ex-md-font-code {
  --font-text: "Cascadia";
}

.excalidraw__embeddable-container .workspace-leaf,
.excalidraw__embeddable-container .workspace-leaf .view-content {
  ::-webkit-scrollbar,
  ::-webkit-scrollbar-horizontal {
    display: none;
  }
  background-color: transparent !important;
}

.excalidraw__embeddable-container .workspace-leaf-content .view-content {
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 0px;
  padding-bottom: 0px;
}

.excalidraw__embeddable-container .workspace-leaf .view-content {
  display: flex;
  align-items: center;
  justify-content: center;
}

.excalidraw__embeddable-container  .workspace-leaf-content .image-container,
.excalidraw__embeddable-container .workspace-leaf-content .audio-container,
.excalidraw__embeddable-container .workspace-leaf-content .video-container {
  display: flex;
}

.excalidraw__embeddable-container .canvas-node-container {
  border: 2px solid var(--canvas-color);
}

.excalidraw__embeddable-container .canvas-node {
  --shadow-border-themed-inset: inset 0 0 0 1px rgb(var(--canvas-color));;
  --shadow-border-themed: 0 0 0 2px rgb(var(--canvas-color));
}

.excalidraw__embeddable-container .canvas-node.is-selected.is-themed .canvas-node-container,
.excalidraw__embeddable-container .canvas-node.is-focused.is-themed .canvas-node-container {
  border-color: var(--canvas-color);
}

img.excalidraw-cropped-pdfpage,
.excalidraw-cropped-pdfpage svg {
  background-color: white;
}

.excalidraw .pdf-toolbar,
.excalidraw .pdf-container {
  width: 100%;
}

.ex-opacity-30 {
  opacity: 0.3;
}

.ex-opacity-15 {
  opacity: 0.15;
}

.ex-opacity-8 {
  opacity: 0.08;
}

.ex-opacity-5 {
  opacity: 0.05;
}

.ex-opacity-0 {
  opacity: 0;
}

.popover .excalidraw-svg {  
  width: 100%;
  max-width: inherit;
  height: 100%;
  max-height: inherit;
}

root {
 --excalidraw-caret-color: initial;
}

textarea.excalidraw-wysiwyg, .excalidraw input {
  caret-color: var(--excalidraw-caret-color);
}

.excalidraw-settings-links-container {
    align-items: center;
    color: inherit;
    display: flex;
    gap: .3em;
    text-align: center;
    text-decoration: none;
    flex-wrap: wrap;
    justify-content: center;
    flex-direction: row;
}

.excalidraw-settings-links-container a {
  display: flex; /* Align children horizontally */
  align-items: center; /* Center items vertically */
  text-align: left;
  margin-right: 4px;
  margin-left: 4px;
}

.excalidraw-settings-links-container svg,
.ex-setting-actions-container svg {
  margin-right: 8px;
  height: 30px;
  width: 30px;
}

.excalidraw-rank {
  text-align: center;
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}

.excalidraw-rank svg {
  height: 8rem;
  width: 8rem;
}

.excalidraw .color-picker-content input[type="color"] {
  filter: var(--theme-filter);
}

.ExcTextField__input input::placeholder {
  color: var(--select-highlight-color);
}

.excalidraw textarea::placeholder {
  color: var(--color-gray-50);
}

.excalidraw textarea.ttd-dialog-input {
  caret-color: var(--excalidraw-caret-color);
}

.excalidraw .ToolIcon_type_button {
  color: var(--text-primary-color);
}

.excalidraw-setting-desc {
  padding: 10px;
  cursor: pointer;
  background-color: var(--background-secondary);
  border: 1px solid var(--background-modifier-border);
  border-radius: 5px;
  transition: background-color 0.3s ease, color 0.3s ease;
}

.excalidraw-setting-desc:hover {
  background-color: var(--background-modifier-hover);
  color: var(--text-accent);
}

.excalidraw-release .nav-buttons-container {
  display: flex;
  margin-bottom: 20px;
  border-bottom: 2px solid var(--background-modifier-border);
}

.excalidraw-release .nav-button {
  padding: 8px 16px;
  border: none;
  background: transparent;
  cursor: pointer;
}

.excalidraw-release .nav-button.is-active {
  border-bottom: 2px solid var(--interactive-accent);
  margin-bottom: -2px;
}

.excalidraw .picker-content {
  grid-gap: 0.2rem !important;
}

.excalidraw .picker-content button.picker-option{
  width: 1.85rem !important;
  height: 1.85rem !important;
}

.excalidraw .picker {
  padding: 0.2rem !important;
}

.excalidraw .context-menu {
  height: fit-content;
}

.excalidraw-prompt-buttonbar-top,
.excalidraw-prompt-buttonbar-bottom {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;  /* keep both rows top‐aligned */
  row-gap: 0.5em;           /* vertical space when wrapped */
}

/* top bar specifics */
.excalidraw-prompt-buttonbar-top {
  padding: 0.5em 0;
  border-top: 1px solid var(--background-modifier-border);
}

/* bottom bar specifics */
.excalidraw-prompt-buttonbar-bottom {
  margin-top: 1rem;
}

/* make each child a flex row */
.excalidraw-prompt-buttonbar-top  > div,
.excalidraw-prompt-buttonbar-bottom > div {
  display: flex;
}

/* push the first group to the left */
.excalidraw-prompt-buttonbar-top  > div:first-child,
.excalidraw-prompt-buttonbar-bottom > div:first-child {
  margin-right: auto;
}

/* push the second group to the right */
.excalidraw-prompt-buttonbar-top  > div:last-child,
.excalidraw-prompt-buttonbar-bottom > div:last-child {
  margin-left: auto;
}

.excalidraw-search.document-search-container {
  display: flex;
  flex-direction: column;
  background: var(--background-secondary);
  border-radius: 8px;
  box-shadow: 0 1px 4px 0 rgba(0,0,0,0.10);
  padding: 0.5em 0.8em;
  margin-bottom: 2em;
  min-width: 18rem;
  position: sticky;
  top: 1rem;
  margin-right: 1rem;
  margin-left: 1rem;
}

.excalidraw-search .document-search {
  align-items: center;
  max-width: none;
}

.excalidraw-search .search-input-container.document-search-input {
  display: flex;
  align-items: center;
  flex: 1 1 auto;
  background: var(--background-primary);
  border-radius: 6px;
  border: 1px solid var(--background-modifier-border);
  min-width: 0;
}

.excalidraw-search .search-input-container .clickable-icon {
  display: flex;
  align-items: center;
  color: var(--text-faint);
}

.excalidraw-search .search-input-container input[type="text"] {
  background: transparent;
  border: none;
  outline: none;
  color: var(--text-normal);
  font-size: 1em;
  flex: 1 1 auto;
  padding: 0.1em 2em;
  margin: 0;
}

.excalidraw-search .document-search-count {
  margin-left: 0.5em;
  color: var(--text-faint);
  font-size: 0.95em;
  white-space: nowrap;
  min-width: 3.5em;
  text-align: right;
}

.excalidraw-search .document-search-buttons {
  display: flex;
  align-items: center;
  gap: 2px;
}

.excalidraw-search .document-search-button {
  background: none;
  border: none;
  outline: none;
  box-shadow: none;
  padding: 0.1em 0.2em;
  margin: 0 1px;
  border-radius: 4px;
  cursor: pointer;
  color: var(--text-faint);
  transition: background 0.15s;
  height: 2em;
  width: 2em;
  display: flex;
  align-items: center;
  justify-content: center;
}

.excalidraw-search .document-search-button:hover, .excalidraw-search .document-search-button:focus {
  background: var(--background-modifier-hover);
  color: var(--text-accent);
}

.excalidraw-search .document-search-button svg {
  width: 1.3em;
  height: 1.3em;
  stroke: currentColor;
  fill: none;
  pointer-events: none;
}



================================================
FILE: tsconfig-lib.json
================================================
{
  "extends": "./tsconfig.json",
  "compilerOptions": {
    "declaration": true,
    "outDir": "lib",
    //"plugins": [{ "transform": "@zerollup/ts-transform-paths" }],
  },
  "include": ["src/**/*.ts"],
  "exclude": ["src/test/**/*", "lib/**/*"]
}


================================================
FILE: tsconfig.dev.json
================================================
{
  "compilerOptions": {
    "baseUrl": ".",
    "sourceMap": false,
    "module": "es2020",
    "target": "es2022", //min es2017 because script engine requires for async execution and min es2018 for named capture groups
    "allowJs": false,
    "noImplicitAny": true,
    "moduleResolution": "node",
    "esModuleInterop": true,
    "importHelpers": true,
    "resolveJsonModule": true,
    "lib": [
      "dom",
      "scripthost",
      "es2022",
      "DOM.Iterable"
    ],
    "jsx": "react",
    "inlineSourceMap": true,
  },
  "include": [
    "**/*.ts",
    "**/*.tsx", "src/Dialogs/OpenDrawing.ts",
    "src/types/types.d.ts",
  ]
}


================================================
FILE: tsconfig.json
================================================
{
  "compilerOptions": {
    "baseUrl": ".",
    "sourceMap": false,
    "module": "es2020",
    "target": "es2022", //min es2017 because script engine requires for async execution and min es2018 for named capture groups
    "allowJs": false,
    "noImplicitAny": true,
    "moduleResolution": "node",
    "esModuleInterop": true,
    "importHelpers": true,
    "resolveJsonModule": true,
    "lib": [
      "dom",
      "scripthost",
      "es2022",
      "DOM.Iterable"
    ],
    "jsx": "react",
  },
  "include": [
    "**/*.ts",
    "**/*.tsx", "src/shared/Dialogs/OpenDrawing.ts",
    "src/types/types.d.ts",
  ]
}


================================================
FILE: versions.json
================================================
{
  "1.8.20": "1.1.6",
  "1.8.19": "1.0.0",
  "1.8.5": "1.0.0",
  "1.7.13": "0.15.6",
  "1.7.8": "0.15.5",
  "1.7.7": "0.15.4",
  "1.7.6": "0.15.3",
  "1.7.2": "0.15.2",
  "1.6.34": "0.12.16",
  "1.4.2": "0.11.13"
}



================================================
FILE: .babelrc
================================================
{
  "presets": ["@babel/preset-env", "@babel/preset-react"]
}


================================================
FILE: .eslintignore
================================================
node_modules/
.github/
docs/
images/


================================================
FILE: .eslintrc.json
================================================
{
  "extends": ["@excalidraw/eslint-config"],
  "rules": {
    "import/no-anonymous-default-export": "off",
    "no-restricted-globals": "off"
  }
}


================================================
FILE: .nvmrc
================================================
20



================================================
FILE: .replit
================================================
language = "nodejs"
run = "npm run dev"


================================================
FILE: docs/readme.md
================================================
# Excalidraw Automate How To

【English | [简体中文](zh-cn/docs/readme.md)】

Use ExcalidrawAutomate to create or manipulate Excalidraw drawings using the [ExcalidrawAutomate Script Engine](ExcalidrawScriptsEngine.md), the [Templater](https://silentvoid13.github.io/Templater/docs/) or the [QuickAdd](https://github.com/chhoumann/quickadd) plugins, and to generate embedded SVG and PNG images using [DataviewJS](https://blacksmithgu.github.io/obsidian-dataview/docs/api/intro/)

With a little work, using ExcalidrawAutomate you can generate simple mindmaps, build a family tree, fill out SVG forms, create customized charts, or automate simple tasks (i.e. create macros) in Excalidraw.
![image](https://user-images.githubusercontent.com/14358394/117549619-bae41180-b03b-11eb-968d-c909e79a7524.png)

## API documentation
- **start here** [Introduction to the API](API/introduction.md)
- [Overview of Attributes and Functions](API/attributes_functions_overview.md)
- [Element Style](API/element_style.md)
- [Canvas Style](API/canvas_style.md)
- [Adding Objects](API/objects.md)
- [Utility Functions](API/utility.md)

## ExcalidrawAutomate Script Engine
I recommend using the Scripts Engine for "Macro" like automation, when you want to automate a few simple steps, such as adding a box around a text element, or connecting two objects with an arrow, or setting line width or the grid to a custom value.  
- [ExcalidrawAutomate Script Engine](ExcalidrawScriptsEngine.md).

## Examples
- **Templater** 
  - [Insert new drawing into currently edited document](Examples/insert_new_drawing.md)
  - [Connect objects](Examples/connect_objects.md)
  - [Apply an Excalidraw template](Examples/apply_template.md)
  - [Mindmap with Templater](Examples/templater_mindmap.md)

- **Dataview** 
  - [Mindmap with Dataview](Examples/dataviewjs_mindmap.md)
  - [Family tree with Dataview](Examples/dataviewjs_familytree.md)

## If you are enjoying the Obsidian Excalidraw Plugin...
Help spread the word by sharing about the Plugin on social media.

You can find me on Twitter [@zsviczian](https://twitter.com/zsviczian), and on my blog [zsolt.blog](https://zsolt.blog).

[<img style="float:left" src="https://user-images.githubusercontent.com/14358394/115450238-f39e8100-a21b-11eb-89d0-fa4b82cdbce8.png" width="150">](https://ko-fi.com/zsolt)





================================================
FILE: docs/_config.yml
================================================
theme: jekyll-theme-hacker


================================================
FILE: docs/ExcalidrawScriptsEngine.md
================================================
# [◀ Excalidraw Automate How To](./readme.md)

【English | [简体中文](zh-cn/docs/ExcalidrawScriptsEngine.md)】

[![Script Engine](https://user-images.githubusercontent.com/14358394/145684531-8d9c2992-59ac-4ebc-804a-4cce1777ded2.jpg)](https://youtu.be/hePJcObHIso)

## Introduction
Place your ExcalidrawAutomate Scripts into the folder defined in Excalidraw Settings. The Scripts folder may not be the root folder of your Vault.

![image](https://user-images.githubusercontent.com/14358394/145673547-b4f57d01-3643-40f9-abfd-14c3bfa5ab93.png)

EA scripts may be markdown files, plain text files, or .js files. The only requirement is that they must contain valid JavaScript code. 

![image](https://user-images.githubusercontent.com/14358394/145673674-bb59f227-8eea-43dc-83b8-4d750e1920a8.png)

You will be able to access your scripts from Excalidraw via the Obsidian Command Palette. 

![image](https://user-images.githubusercontent.com/14358394/145673652-6b1713e2-edc8-4bc8-8246-3f8df8a4b273.png)

This will allow you to assign hotkeys to your favorite scripts just like to any other Obsidian command. 

![image](https://user-images.githubusercontent.com/14358394/145673633-83b6c969-cead-429b-9721-fd047f980279.png)

## Script development
An Excalidraw script will automatically receive two objects:
- `ea`: The Script Engine will initialize the `ea` object including setting the active view to the View from which the script was called.
- `utils`: I have borrowed functions exposed on utils from [QuickAdd](https://github.com/chhoumann/quickadd/blob/master/docs/QuickAddAPI.md), though currently not all QuickAdd utility functions are implemented in Excalidraw. As of now, these are the available functions. See the example below for details.
  - `inputPrompt: (header: string, placeholder?: string, value?: string, buttons?: [{caption:string, action:Function}])`
    - Opens a prompt that asks for an input. Returns a string with the input.
    - You need to await the result of inputPrompt.
    - `buttons.action(input: string) => string`. The button action will receive the current input string. If action returns null, the input will be unchanged. If action returns a string, the inputPrompt will resolve to this value.
```typescript
let fileType = "";
const filename = await utils.inputPrompt (
  "Filename for new document",
  "Placeholder",
  "DefaultFilename.md",
  [
    {
      caption: "Markdown",
      action: ()=>{fileType="md";return;}
		},
    {
      caption: "Excalidraw",
      action: ()=>{fileType="ex";return;}
    }
  ]
);

```
  - `suggester: (displayItems: string[], items: any[], hint?: string, instructions?:Instruction[])`
    - Opens a suggester. Displays the displayItems and returns the corresponding item from items[].
    - You need to await the result of suggester.
    - If the user cancels (ESC), suggester will return `undefined`
    - Hint and instructions are optional.
    ```typescript
      interface Instruction {
        command: string;
        purpose: string;
      }
    ```
  - Scripts may have settings. These settings are stored as part of plugin settings and may be also changed by the user via the Obsidian plugin settings window.
    - You can access settings for the active script using `ea.getScriptSettings()` and store settings values with `ea.setScriptSettings(settings:any)`
    - Rules for displaying script settings in plugin settings are:
      - If the setting is a simple literal (boolean, number, string) these will be displayed as such in settings. The name of the setting will be the key for the value.
    ```javascript
    ea.setScriptSettings({ 
      "value 1": true, 
      "value 2": 1,
      "value 3": "my string"
    })
    ```
    ![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/SimpleSettings.jpg)
      - If the setting is an object and follows the below structure then a description and a valueset may also be added. Values may also be hidden from the user using the `hidden` key.
      ```javascript
      ea.setScriptSettings({
        "value 1": {
          "value": true,
          "description": "This is the description for my boolean value"
        },
        "value 2": {
          "value": 1,
          "description": "This is the description for my numeric value"
        },
        "value 3": {
          "value": "my string",
          "description": "This is the description for my string value",
          "valueset": ["allowed 1","allowed 2","allowed 3"]
        },
        "value 4": {
          "value": "my value",
          "hidden": true
        }        
      });
      ```
      ![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/ComplexSettings.jpg)

---------

## Example Excalidraw Automate Scripts

These scripts are available as downloadable `.md` files on GitHub in [this](https://github.com/zsviczian/obsidian-excalidraw-plugin/tree/master/ea-scripts) folder 📂.

### Add box around selected elements

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-box-elements.jpg)

This script will add an encapsulating box around the currently selected elements in Excalidraw
```javascript
if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//check if settings exist. If not, set default values on first run
if(!settings["Default padding"]) {
	settings = {
		"Prompt for padding?": true,
	  "Default padding" : {
			value: 10,
		  description: "Padding between the bounding box of the selected elements, and the box the script creates"
		}
	};
	ea.setScriptSettings(settings);
}

let padding = settings["Default padding"].value;

if(settings["Prompt for padding?"]) {
	padding = parseInt (await utils.inputPrompt("padding?","number",padding.toString()));
}

if(isNaN(padding)) {
  new Notice("The padding value provided is not a number");
  return;
}
elements = ea.getViewSelectedElements();
const box = ea.getBoundingBox(elements);
color = ea
        .getExcalidrawAPI()
        .getAppState()
        .currentItemStrokeColor;
//uncomment for random color:
//color = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
ea.style.strokeColor = color;
id = ea.addRect(
	box.topX - padding,
	box.topY - padding,
	box.width + 2*padding,
	box.height + 2*padding
);
ea.copyViewElementsToEAforEditing(elements);
ea.addToGroup([id].concat(elements.map((el)=>el.id)));
ea.addElementsToView(false);
```

----

### Connect selected elements with an arrow

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-connect-elements.jpg)

This script will connect two objects with an arrow. If either of the objects are a set of grouped elements (e.g. a text element grouped with an encapsulating rectangle), the script will identify these groups, and connect the arrow to the largest object in the group (assuming you want to connect the arrow to the box around the text element).
```javascript
if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//set default values on first run
if(!settings["Starting arrowhead"]) {
	settings = {
	  "Starting arrowhead" : {
			value: "none",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Ending arrowhead" : {
			value: "triangle",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Line points" : {
			value: 1,
      description: "Number of line points between start and end"
		}
	};
	ea.setScriptSettings(settings);
}

const arrowStart = settings["Starting arrowhead"].value === "none" ? null : settings["Starting arrowhead"].value;
const arrowEnd = settings["Ending arrowhead"].value === "none" ? null : settings["Ending arrowhead"].value;
const linePoints = Math.floor(settings["Line points"].value);

const elements = ea.getViewSelectedElements();
ea.copyViewElementsToEAforEditing(elements);
groups = ea.getMaximumGroups(elements);

if(groups.length !== 2) {
  //unfortunately getMaxGroups returns duplicated resultset for sticky notes
  //needs additional filtering
  cleanGroups=[];
  idList = [];
  for (group of groups) {
    keep = true;
    for(item of group) if(idList.contains(item.id)) keep = false;
    if(keep) {
      cleanGroups.push(group);
      idList = idList.concat(group.map(el=>el.id))
    }
  }
  if(cleanGroups.length !== 2) return;
  groups = cleanGroups;
}

els = [ 
  ea.getLargestElement(groups[0]),
  ea.getLargestElement(groups[1])
];

ea.style.strokeColor = els[0].strokeColor;
ea.style.strokeWidth = els[0].strokeWidth;
ea.style.strokeStyle = els[0].strokeStyle;
ea.style.strokeSharpness = els[0].strokeSharpness;

ea.connectObjects(
  els[0].id,
  null,
  els[1].id,
  null, 
  {
	endArrowHead: arrowEnd,
	startArrowHead: arrowStart, 
	numberOfPoints: linePoints
  }
);
ea.addElementsToView();
```

----
### Reverse selected arrows

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-reverse-arrow.jpg)

Reverse the direction of **arrows** within the scope of selected elements.

```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="arrow");
if(!elements || elements.length===0) return;
elements.forEach((el)=>{
	const start = el.startArrowhead;
	el.startArrowhead = el.endArrowhead;
	el.endArrowhead = start;
});
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```

----

### Set line width of selected elements

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-stroke-width.jpg)

This is helpful, for example, when you scale freedraw sketches and want to reduce or increase their line width.
```javascript
let width = (ea.getViewSelectedElement().strokeWidth??1).toString();
width = await utils.inputPrompt("Width?","number",width);
const elements=ea.getViewSelectedElements();
ea.copyViewElementsToEAforEditing(elements);
ea.getElements().forEach((el)=>el.strokeWidth=width);
ea.addElementsToView();
```

----

### Set grid size

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-grid.jpg)

The default grid size in Excalidraw is 20. Currently there is no way to change the grid size via the user interface. 
```javascript
const grid = parseInt(await utils.inputPrompt("Grid size?",null,"20"));
const api = ea.getExcalidrawAPI();
let appState = api.getAppState();
appState.gridSize = grid;
api.updateScene({
  appState,
  commitToHistory:false
});
```

----

### Set element dimensions and position

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-dimensions.jpg)

Currently there is no way to specify the exact location and size of objects in Excalidraw. You can bridge this gap with the following simple script.
```javascript
const elements = ea.getViewSelectedElements();
if(elements.length === 0) return;
const el = ea.getLargestElement(elements);
const sizeIn = [el.x,el.y,el.width,el.height].join(",");
let res = await utils.inputPrompt("x,y,width,height?",null,sizeIn);
res = res.split(",");
if(res.length !== 4) return;
let size = [];
for (v of res) {
  const i = parseInt(v);
  if(isNaN(i)) return;
  size.push(i);
}
el.x = size[0];
el.y = size[1];
el.width = size[2];
el.height = size[3];
ea.copyViewElementsToEAforEditing([el]);
ea.addElementsToView();
```

----

### Bullet points

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-bullet-point.jpg)

This script will add a small circle to the top left of each text element in the selection and add the text and the "bullet point" into a group.
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
ea.copyViewElementsToEAforEditing(elements);
const padding = 10;
elements.forEach((el)=>{
  ea.style.strokeColor = el.strokeColor;
  const size = el.fontSize/2;
  const ellipseId = ea.addEllipse(
    el.x-padding-size,
    el.y+size/2,
    size,
    size
  );
  ea.addToGroup([el.id,ellipseId]);
});
ea.addElementsToView();
```

----

### Split text by lines
**!!!Requires Excalidraw 1.5.1 or higher**

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-split-lines.jpg)

Split lines of text into separate text elements for easier reorganization
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
elements.forEach((el)=>{
  ea.style.strokeColor = el.strokeColor;
  ea.style.fontFamily  = el.fontFamily;
  ea.style.fontSize    = el.fontSize;
  const text = el.text.split("\n");
  for(i=0;i<text.length;i++) {
	ea.addText(el.x,el.y+i*el.height/text.length,text[i]);
  }
});
ea.addElementsToView();
ea.deleteViewElements(elements);
```

----

### Set Text Alignment

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-text-align.jpg)

Sets text alignment of text block (cetner, right, left). Useful if you want to set a keyboard shortcut for selecting text alignment.
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
if(elements.length===0) return;
let align = ["left","right","center"];
align = await utils.suggester(align,align);
elements.forEach((el)=>el.textAlign = align);
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```

----

### Set Font Family

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-font-family.jpg)

Sets font family of the text block (Virgil, Helvetica, Cascadia). Useful if you want to set a keyboard shortcut for selecting font family.
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
if(elements.length===0) return;
let font = ["Virgil","Helvetica","Cascadia"];
font = parseInt(await utils.suggester(font,["1","2","3"]));
if (isNaN(font)) return;
elements.forEach((el)=>el.fontFamily = font);
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```



================================================
FILE: docs/API/attributes_functions_overview.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Attributes and functions overview
Here's the interface implemented by ExcalidrawAutomate:

You can find the source file here: [ExcalidrawAutomate.d.ts](ExcalidrawAutomate.d.ts).

```javascript
/// <reference types="react" />
import ExcalidrawPlugin from "src/main";
import { FillStyle, StrokeStyle, ExcalidrawElement, ExcalidrawBindableElement, FileId, NonDeletedExcalidrawElement, ExcalidrawImageElement, StrokeRoundness, RoundnessType } from "@zsviczian/excalidraw/types/element/types";
import { Editor, OpenViewState, TFile, WorkspaceLeaf } from "obsidian";
import * as obsidian_module from "obsidian";
import ExcalidrawView, { ExportSettings } from "src/ExcalidrawView";
import { AppState, BinaryFileData, DataURL, ExcalidrawImperativeAPI, Point } from "@zsviczian/excalidraw/types/types";
import { EmbeddedFilesLoader } from "src/EmbeddedFileLoader";
import { ConnectionPoint, DeviceType } from "src/types";
import { ColorMaster } from "colormaster";
import { TInput } from "colormaster/types";
import { ClipboardData } from "@zsviczian/excalidraw/types/clipboard";
import { PaneTarget } from "src/utils/modifierkeyHelper";
export declare class ExcalidrawAutomate {
    /**
     * Utility function that returns the Obsidian Module object.
     */
    get obsidian(): typeof obsidian_module;
    get DEVICE(): DeviceType;
    getAttachmentFilepath(filename: string): Promise<string>;
    /**
     * Prompts the user with a dialog to select new file action.
     * - create markdown file
     * - create excalidraw file
     * - cancel action
     * The new file will be relative to this.targetView.file.path, unless parentFile is provided.
     * If shouldOpenNewFile is true, the new file will be opened in a workspace leaf.
     * targetPane control which leaf will be used for the new file.
     * Returns the TFile for the new file or null if the user cancelled the action.
     * @param newFileNameOrPath
     * @param shouldOpenNewFile
     * @param targetPane //type PaneTarget = "active-pane"|"new-pane"|"popout-window"|"new-tab"|"md-properties";
     * @param parentFile
     * @returns
     */
    newFilePrompt(newFileNameOrPath: string, shouldOpenNewFile: boolean, targetPane?: PaneTarget, parentFile?: TFile): Promise<TFile | null>;
    /**
     * Generates a new Obsidian Leaf following Excalidraw plugin settings such as open in Main Workspace or not, open in adjacent pane if available, etc.
     * @param origo // the currently active leaf, the origin of the new leaf
     * @param targetPane //type PaneTarget = "active-pane"|"new-pane"|"popout-window"|"new-tab"|"md-properties";
     * @returns
     */
    getLeaf(origo: WorkspaceLeaf, targetPane?: PaneTarget): WorkspaceLeaf;
    /**
     * Returns the editor or leaf.view of the currently active embedded obsidian file.
     * If view is not provided, ea.targetView is used.
     * If the embedded file is a markdown document the function will return
     * {file:TFile, editor:Editor} otherwise it will return {view:any}. You can check view type with view.getViewType();
     * @param view
     * @returns
     */
    getActiveEmbeddableViewOrEditor(view?: ExcalidrawView): {
        view: any;
    } | {
        file: TFile;
        editor: Editor;
    } | null;
    plugin: ExcalidrawPlugin;
    elementsDict: {
        [key: string]: any;
    };
    imagesDict: {
        [key: FileId]: any;
    };
    mostRecentMarkdownSVG: SVGSVGElement;
    style: {
        strokeColor: string;
        backgroundColor: string;
        angle: number;
        fillStyle: FillStyle;
        strokeWidth: number;
        strokeStyle: StrokeStyle;
        roughness: number;
        opacity: number;
        strokeSharpness?: StrokeRoundness;
        roundness: null | {
            type: RoundnessType;
            value?: number;
        };
        fontFamily: number;
        fontSize: number;
        textAlign: string;
        verticalAlign: string;
        startArrowHead: string;
        endArrowHead: string;
    };
    canvas: {
        theme: string;
        viewBackgroundColor: string;
        gridSize: number;
    };
    colorPalette: {};
    constructor(plugin: ExcalidrawPlugin, view?: ExcalidrawView);
    /**
     *
     * @returns the last recorded pointer position on the Excalidraw canvas
     */
    getViewLastPointerPosition(): {
        x: number;
        y: number;
    };
    /**
     *
     * @returns
     */
    getAPI(view?: ExcalidrawView): ExcalidrawAutomate;
    /**
     * @param val //0:"hachure", 1:"cross-hatch" 2:"solid"
     * @returns
     */
    setFillStyle(val: number): "hachure" | "cross-hatch" | "solid";
    /**
     * @param val //0:"solid", 1:"dashed", 2:"dotted"
     * @returns
     */
    setStrokeStyle(val: number): "solid" | "dashed" | "dotted";
    /**
     * @param val //0:"round", 1:"sharp"
     * @returns
     */
    setStrokeSharpness(val: number): "round" | "sharp";
    /**
     * @param val //1: Virgil, 2:Helvetica, 3:Cascadia
     * @returns
     */
    setFontFamily(val: number): "Virgil, Segoe UI Emoji" | "Helvetica, Segoe UI Emoji" | "Cascadia, Segoe UI Emoji" | "LocalFont";
    /**
     * @param val //0:"light", 1:"dark"
     * @returns
     */
    setTheme(val: number): "light" | "dark";
    /**
     * @param objectIds
     * @returns
     */
    addToGroup(objectIds: string[]): string;
    /**
     * @param templatePath
     */
    toClipboard(templatePath?: string): Promise<void>;
    /**
     * @param file: TFile
     * @returns ExcalidrawScene
     */
    getSceneFromFile(file: TFile): Promise<{
        elements: ExcalidrawElement[];
        appState: AppState;
    }>;
    /**
     * get all elements from ExcalidrawAutomate elementsDict
     * @returns elements from elementsDict
     */
    getElements(): ExcalidrawElement[];
    /**
     * get single element from ExcalidrawAutomate elementsDict
     * @param id
     * @returns
     */
    getElement(id: string): ExcalidrawElement;
    /**
     * create a drawing and save it to filename
     * @param params
     *   filename: if null, default filename as defined in Excalidraw settings
     *   foldername: if null, default folder as defined in Excalidraw settings
     * @returns
     */
    create(params?: {
        filename?: string;
        foldername?: string;
        templatePath?: string;
        onNewPane?: boolean;
        frontmatterKeys?: {
            "excalidraw-plugin"?: "raw" | "parsed";
            "excalidraw-link-prefix"?: string;
            "excalidraw-link-brackets"?: boolean;
            "excalidraw-url-prefix"?: string;
            "excalidraw-export-transparent"?: boolean;
            "excalidraw-export-dark"?: boolean;
            "excalidraw-export-padding"?: number;
            "excalidraw-export-pngscale"?: number;
            "excalidraw-default-mode"?: "view" | "zen";
            "excalidraw-onload-script"?: string;
            "excalidraw-linkbutton-opacity"?: number;
            "excalidraw-autoexport"?: boolean;
        };
        plaintext?: string;
    }): Promise<string>;
    /**
     *
     * @param templatePath
     * @param embedFont
     * @param exportSettings use ExcalidrawAutomate.getExportSettings(boolean,boolean)
     * @param loader use ExcalidrawAutomate.getEmbeddedFilesLoader(boolean?)
     * @param theme
     * @returns
     */
    createSVG(templatePath?: string, embedFont?: boolean, exportSettings?: ExportSettings, loader?: EmbeddedFilesLoader, theme?: string, padding?: number): Promise<SVGSVGElement>;
    /**
     *
     * @param templatePath
     * @param scale
     * @param exportSettings use ExcalidrawAutomate.getExportSettings(boolean,boolean)
     * @param loader use ExcalidrawAutomate.getEmbeddedFilesLoader(boolean?)
     * @param theme
     * @returns
     */
    createPNG(templatePath?: string, scale?: number, exportSettings?: ExportSettings, loader?: EmbeddedFilesLoader, theme?: string, padding?: number): Promise<any>;
    /**
     *
     * @param text
     * @param lineLen
     * @returns
     */
    wrapText(text: string, lineLen: number): string;
    private boxedElement;
    addIFrame(topX: number, topY: number, width: number, height: number, url?: string, file?: TFile): string;
    /**
   *
   * @param topX
   * @param topY
   * @param width
   * @param height
   * @returns
   */
    addEmbeddable(topX: number, topY: number, width: number, height: number, url?: string, file?: TFile): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addRect(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addDiamond(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addEllipse(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addBlob(topX: number, topY: number, width: number, height: number): string;
    /**
     * Refresh the size of a text element to fit its contents
     * @param id - the id of the text element
     */
    refreshTextElementSize(id: string): void;
    /**
     *
     * @param topX
     * @param topY
     * @param text
     * @param formatting
     *   box: if !null, text will be boxed
     * @param id
     * @returns
     */
    addText(topX: number, topY: number, text: string, formatting?: {
        wrapAt?: number;
        width?: number;
        height?: number;
        textAlign?: "left" | "center" | "right";
        box?: boolean | "box" | "blob" | "ellipse" | "diamond";
        boxPadding?: number;
        boxStrokeColor?: string;
        textVerticalAlign?: "top" | "middle" | "bottom";
    }, id?: string): string;
    /**
     *
     * @param points
     * @returns
     */
    addLine(points: [[x: number, y: number]]): string;
    /**
     *
     * @param points
     * @param formatting
     * @returns
     */
    addArrow(points: [x: number, y: number][], formatting?: {
        startArrowHead?: string;
        endArrowHead?: string;
        startObjectId?: string;
        endObjectId?: string;
    }): string;
    /**
     *
     * @param topX
     * @param topY
     * @param imageFile
     * @returns
     */
    addImage(topX: number, topY: number, imageFile: TFile | string, scale?: boolean, //default is true which will scale the image to MAX_IMAGE_SIZE, false will insert image at 100% of its size
    anchor?: boolean): Promise<string>;
    /**
     *
     * @param topX
     * @param topY
     * @param tex
     * @returns
     */
    addLaTex(topX: number, topY: number, tex: string): Promise<string>;
    /**
     *
     * @param objectA
     * @param connectionA type ConnectionPoint = "top" | "bottom" | "left" | "right" | null
     * @param objectB
     * @param connectionB when passed null, Excalidraw will automatically decide
     * @param formatting
     *   numberOfPoints: points on the line. Default is 0 ie. line will only have a start and end point
     *   startArrowHead: "triangle"|"dot"|"arrow"|"bar"|null
     *   endArrowHead: "triangle"|"dot"|"arrow"|"bar"|null
     *   padding:
     * @returns
     */
    connectObjects(objectA: string, connectionA: ConnectionPoint | null, objectB: string, connectionB: ConnectionPoint | null, formatting?: {
        numberOfPoints?: number;
        startArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        endArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        padding?: number;
    }): string;
    /**
     * Adds a text label to a line or arrow. Currently only works with a straight (2 point - start & end - line)
     * @param lineId id of the line or arrow object in elementsDict
     * @param label the label text
     * @returns undefined (if unsuccessful) or the id of the new text element
     */
    addLabelToLine(lineId: string, label: string): string;
    /**
     * clear elementsDict and imagesDict only
     */
    clear(): void;
    /**
     * clear() + reset all style values to default
     */
    reset(): void;
    /**
     * returns true if MD file is an Excalidraw file
     * @param f
     * @returns
     */
    isExcalidrawFile(f: TFile): boolean;
    targetView: ExcalidrawView;
    /**
     * sets the target view for EA. All the view operations and the access to Excalidraw API will be performend on this view
     * if view is null or undefined, the function will first try setView("active"), then setView("first").
     * @param view
     * @returns targetView
     */
    setView(view?: ExcalidrawView | "first" | "active"): ExcalidrawView;
    /**
     *
     * @returns https://github.com/excalidraw/excalidraw/tree/master/src/packages/excalidraw#ref
     */
    getExcalidrawAPI(): any;
    /**
     * get elements in View
     * @returns
     */
    getViewElements(): ExcalidrawElement[];
    /**
     *
     * @param elToDelete
     * @returns
     */
    deleteViewElements(elToDelete: ExcalidrawElement[]): boolean;
    /**
     * get the selected element in the view, if more are selected, get the first
     * @returns
     */
    getViewSelectedElement(): any;
    /**
     *
     * @returns
     */
    getViewSelectedElements(): any[];
    /**
     *
     * @param el
     * @returns TFile file handle for the image element
     */
    getViewFileForImageElement(el: ExcalidrawElement): TFile | null;
    /**
     * copies elements from view to elementsDict for editing
     * @param elements
     */
    copyViewElementsToEAforEditing(elements: ExcalidrawElement[]): void;
    /**
     *
     * @param forceViewMode
     * @returns
     */
    viewToggleFullScreen(forceViewMode?: boolean): void;
    setViewModeEnabled(enabled: boolean): void;
    /**
     * This function gives you a more hands on access to Excalidraw.
     * @param scene - The scene you want to load to Excalidraw
     * @param restore - Use this if the scene includes legacy excalidraw file elements that need to be converted to the latest excalidraw data format (not a typical usecase)
     * @returns
     */
    viewUpdateScene(scene: {
        elements?: ExcalidrawElement[];
        appState?: AppState;
        files?: BinaryFileData;
        commitToHistory?: boolean;
    }, restore?: boolean): void;
    /**
     * connect an object to the selected element in the view
     * @param objectA ID of the element
     * @param connectionA
     * @param connectionB
     * @param formatting
     * @returns
     */
    connectObjectWithViewSelectedElement(objectA: string, connectionA: ConnectionPoint | null, connectionB: ConnectionPoint | null, formatting?: {
        numberOfPoints?: number;
        startArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        endArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        padding?: number;
    }): boolean;
    /**
     * zoom tarteView to fit elements provided as input
     * elements === [] will zoom to fit the entire scene
     * selectElements toggles whether the elements should be in a selected state at the end of the operation
     * @param selectElements
     * @param elements
     */
    viewZoomToElements(selectElements: boolean, elements: ExcalidrawElement[]): void;
    /**
     * Adds elements from elementsDict to the current view
     * @param repositionToCursor default is false
     * @param save default is true
     * @param newElementsOnTop controls whether elements created with ExcalidrawAutomate
     *   are added at the bottom of the stack or the top of the stack of elements already in the view
     *   Note that elements copied to the view with copyViewElementsToEAforEditing retain their
     *   position in the stack of elements in the view even if modified using EA
     *   default is false, i.e. the new elements get to the bottom of the stack
     * @param shouldRestoreElements - restore elements - auto-corrects broken, incomplete or old elements included in the update
     * @returns
     */
    addElementsToView(repositionToCursor?: boolean, save?: boolean, newElementsOnTop?: boolean, shouldRestoreElements?: boolean): Promise<boolean>;
    /**
     * Register instance of EA to use for hooks with TargetView
     * By default ExcalidrawViews will check window.ExcalidrawAutomate for event hooks.
     * Using this event you can set a different instance of Excalidraw Automate for hooks
     * @returns true if successful
     */
    registerThisAsViewEA(): boolean;
    /**
     * Sets the targetView EA to window.ExcalidrawAutomate
     * @returns true if successful
     */
    deregisterThisAsViewEA(): boolean;
    /**
     * If set, this callback is triggered when the user closes an Excalidraw view.
     */
    onViewUnloadHook: (view: ExcalidrawView) => void;
    /**
     * If set, this callback is triggered, when the user changes the view mode.
     * You can use this callback in case you want to do something additional when the user switches to view mode and back.
     */
    onViewModeChangeHook: (isViewModeEnabled: boolean, view: ExcalidrawView, ea: ExcalidrawAutomate) => void;
    /**
    * If set, this callback is triggered, when the user hovers a link in the scene.
    * You can use this callback in case you want to do something additional when the onLinkHover event occurs.
    * This callback must return a boolean value.
    * In case you want to prevent the excalidraw onLinkHover action you must return false, it will stop the native excalidraw onLinkHover management flow.
    */
    onLinkHoverHook: (element: NonDeletedExcalidrawElement, linkText: string, view: ExcalidrawView, ea: ExcalidrawAutomate) => boolean;
    /**
    * If set, this callback is triggered, when the user clicks a link in the scene.
    * You can use this callback in case you want to do something additional when the onLinkClick event occurs.
    * This callback must return a boolean value.
    * In case you want to prevent the excalidraw onLinkClick action you must return false, it will stop the native excalidraw onLinkClick management flow.
    */
    onLinkClickHook: (element: ExcalidrawElement, linkText: string, event: MouseEvent, view: ExcalidrawView, ea: ExcalidrawAutomate) => boolean;
    /**
     * If set, this callback is triggered, when Excalidraw receives an onDrop event.
     * You can use this callback in case you want to do something additional when the onDrop event occurs.
     * This callback must return a boolean value.
     * In case you want to prevent the excalidraw onDrop action you must return false, it will stop the native excalidraw onDrop management flow.
     */
    onDropHook: (data: {
        ea: ExcalidrawAutomate;
        event: React.DragEvent<HTMLDivElement>;
        draggable: any;
        type: "file" | "text" | "unknown";
        payload: {
            files: TFile[];
            text: string;
        };
        excalidrawFile: TFile;
        view: ExcalidrawView;
        pointerPosition: {
            x: number;
            y: number;
        };
    }) => boolean;
    /**
     * If set, this callback is triggered, when Excalidraw receives an onPaste event.
     * You can use this callback in case you want to do something additional when the
     * onPaste event occurs.
     * This callback must return a boolean value.
     * In case you want to prevent the excalidraw onPaste action you must return false,
     * it will stop the native excalidraw onPaste management flow.
     */
    onPasteHook: (data: {
        ea: ExcalidrawAutomate;
        payload: ClipboardData;
        event: ClipboardEvent;
        excalidrawFile: TFile;
        view: ExcalidrawView;
        pointerPosition: {
            x: number;
            y: number;
        };
    }) => boolean;
    /**
     * if set, this callback is triggered, when an Excalidraw file is opened
     * You can use this callback in case you want to do something additional when the file is opened.
     * This will run before the file level script defined in the `excalidraw-onload-script` frontmatter.
     */
    onFileOpenHook: (data: {
        ea: ExcalidrawAutomate;
        excalidrawFile: TFile;
        view: ExcalidrawView;
    }) => Promise<void>;
    /**
     * if set, this callback is triggered, when an Excalidraw file is created
     * see also: https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/1124
     */
    onFileCreateHook: (data: {
        ea: ExcalidrawAutomate;
        excalidrawFile: TFile;
        view: ExcalidrawView;
    }) => Promise<void>;
    /**
     * If set, this callback is triggered whenever the active canvas color changes
     */
    onCanvasColorChangeHook: (ea: ExcalidrawAutomate, view: ExcalidrawView, //the excalidraw view 
    color: string) => void;
    /**
     * utility function to generate EmbeddedFilesLoader object
     * @param isDark
     * @returns
     */
    getEmbeddedFilesLoader(isDark?: boolean): EmbeddedFilesLoader;
    /**
     * utility function to generate ExportSettings object
     * @param withBackground
     * @param withTheme
     * @returns
     */
    getExportSettings(withBackground: boolean, withTheme: boolean): ExportSettings;
    /**
     * get bounding box of elements
     * bounding box is the box encapsulating all of the elements completely
     * @param elements
     * @returns
     */
    getBoundingBox(elements: ExcalidrawElement[]): {
        topX: number;
        topY: number;
        width: number;
        height: number;
    };
    /**
     * elements grouped by the highest level groups
     * @param elements
     * @returns
     */
    getMaximumGroups(elements: ExcalidrawElement[]): ExcalidrawElement[][];
    /**
     * gets the largest element from a group. useful when a text element is grouped with a box, and you want to connect an arrow to the box
     * @param elements
     * @returns
     */
    getLargestElement(elements: ExcalidrawElement[]): ExcalidrawElement;
    /**
     * @param element
     * @param a
     * @param b
     * @param gap
     * @returns 2 or 0 intersection points between line going through `a` and `b`
     *   and the `element`, in ascending order of distance from `a`.
     */
    intersectElementWithLine(element: ExcalidrawBindableElement, a: readonly [number, number], b: readonly [number, number], gap?: number): Point[];
    /**
     * Gets the groupId for the group that contains all the elements, or null if such a group does not exist
     * @param elements
     * @returns null or the groupId
     */
    getCommonGroupForElements(elements: ExcalidrawElement[]): string;
    /**
     * Gets all the elements from elements[] that share one or more groupIds with element.
     * @param element
     * @param elements - typically all the non-deleted elements in the scene
     * @returns
     */
    getElementsInTheSameGroupWithElement(element: ExcalidrawElement, elements: ExcalidrawElement[]): ExcalidrawElement[];
    /**
     * Gets all the elements from elements[] that are contained in the frame.
     * @param element
     * @param elements - typically all the non-deleted elements in the scene
     * @returns
     */
    getElementsInFrame(frameElement: ExcalidrawElement, elements: ExcalidrawElement[]): ExcalidrawElement[];
    /**
     * See OCR plugin for example on how to use scriptSettings
     * Set by the ScriptEngine
     */
    activeScript: string;
    /**
     *
     * @returns script settings. Saves settings in plugin settings, under the activeScript key
     */
    getScriptSettings(): {};
    /**
     * sets script settings.
     * @param settings
     * @returns
     */
    setScriptSettings(settings: any): Promise<void>;
    /**
     * Open a file in a new workspaceleaf or reuse an existing adjacent leaf depending on Excalidraw Plugin Settings
     * @param file
     * @param openState - if not provided {active: true} will be used
     * @returns
     */
    openFileInNewOrAdjacentLeaf(file: TFile, openState?: OpenViewState): WorkspaceLeaf;
    /**
     * measure text size based on current style settings
     * @param text
     * @returns
     */
    measureText(text: string): {
        width: number;
        height: number;
    };
    /**
     * Returns the size of the image element at 100% (i.e. the original size)
     * @param imageElement an image element from the active scene on targetView
     */
    getOriginalImageSize(imageElement: ExcalidrawImageElement): Promise<{
        width: number;
        height: number;
    }>;
    /**
     * verifyMinimumPluginVersion returns true if plugin version is >= than required
     * recommended use:
     * if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.20")) {new Notice("message");return;}
     * @param requiredVersion
     * @returns
     */
    verifyMinimumPluginVersion(requiredVersion: string): boolean;
    /**
     * Check if view is instance of ExcalidrawView
     * @param view
     * @returns
     */
    isExcalidrawView(view: any): boolean;
    /**
     * sets selection in view
     * @param elements
     * @returns
     */
    selectElementsInView(elements: ExcalidrawElement[] | string[]): void;
    /**
     * @returns an 8 character long random id
     */
    generateElementId(): string;
    /**
     * @param element
     * @returns a clone of the element with a new id
     */
    cloneElement(element: ExcalidrawElement): ExcalidrawElement;
    /**
     * Moves the element to a specific position in the z-index
     */
    moveViewElementToZIndex(elementId: number, newZIndex: number): void;
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    hexStringToRgb(color: string): number[];
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    rgbToHexString(color: number[]): string;
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    hslToRgb(color: number[]): number[];
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    rgbToHsl(color: number[]): number[];
    /**
     *
     * @param color
     * @returns
     */
    colorNameToHex(color: string): string;
    /**
     * https://github.com/lbragile/ColorMaster
     * @param color
     * @returns
     */
    getCM(color: TInput): ColorMaster;
    importSVG(svgString: string): boolean;
}
export declare function initExcalidrawAutomate(plugin: ExcalidrawPlugin): Promise<ExcalidrawAutomate>;
export declare function destroyExcalidrawAutomate(): void;
export declare function _measureText(newText: string, fontSize: number, fontFamily: number, lineHeight: number): {
    w: number;
    h: number;
    baseline: number;
};
export declare const generatePlaceholderDataURL: (width: number, height: number) => DataURL;
export declare function createPNG(templatePath: string, scale: number, exportSettings: ExportSettings, loader: EmbeddedFilesLoader, forceTheme: string, canvasTheme: string, canvasBackgroundColor: string, automateElements: ExcalidrawElement[], plugin: ExcalidrawPlugin, depth: number, padding?: number, imagesDict?: any): Promise<Blob>;
export declare function createSVG(templatePath: string, embedFont: boolean, exportSettings: ExportSettings, loader: EmbeddedFilesLoader, forceTheme: string, canvasTheme: string, canvasBackgroundColor: string, automateElements: ExcalidrawElement[], plugin: ExcalidrawPlugin, depth: number, padding?: number, imagesDict?: any, convertMarkdownLinksToObsidianURLs?: boolean): Promise<SVGSVGElement>;
export declare function estimateBounds(elements: ExcalidrawElement[]): [number, number, number, number];
export declare function repositionElementsToCursor(elements: ExcalidrawElement[], newPosition: {
    x: number;
    y: number;
}, center: boolean, api: ExcalidrawImperativeAPI): ExcalidrawElement[];
export declare const insertLaTeXToView: (view: ExcalidrawView) => void;
export declare const search: (view: ExcalidrawView) => Promise<void>;
/**
 *
 * @param elements
 * @param query
 * @param exactMatch - when searching for section header exactMatch should be set to true
 * @returns the elements matching the query
 */
export declare const getTextElementsMatchingQuery: (elements: ExcalidrawElement[], query: string[], exactMatch?: boolean) => ExcalidrawElement[];
/**
 *
 * @param elements
 * @param query
 * @param exactMatch - when searching for section header exactMatch should be set to true
 * @returns the elements matching the query
 */
export declare const getFrameElementsMatchingQuery: (elements: ExcalidrawElement[], query: string[], exactMatch?: boolean) => ExcalidrawElement[];
export declare const cloneElement: (el: ExcalidrawElement) => any;
export declare const verifyMinimumPluginVersion: (requiredVersion: string) => boolean;
```


================================================
FILE: docs/API/canvas_style.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Canvas style settings
Sets the properties of the canvas. 

### theme, setTheme()
String. Valid values are "light" and "dark".

`setTheme()` accepts a number:
- 0: "light"
- any other number: "dark"

### viewBackgroundColor
String. This is the fill color of an object. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings e.g. `#FF0000` for red, or `transparent`.

### gridSize
Number. The size of the grid. If set to zero, no grid is displayed.


================================================
FILE: docs/API/element_style.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Element style settings
As you will notice, some styles have setter functions. This is to help you navigate the allowed values for the property. You do not need to use the setter function however, you can use set the value directly as well.

### strokeColor
String. The color of the line. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings, or  e.g. `#FF0000` for red.

### backgroundColor
String. This is the fill color of an object. [CSS Legal Color Values](https://www.w3schools.com/cssref/css_colors_legal.asp)

Allowed values are [HTML color names](https://www.w3schools.com/colors/colors_names.asp), hexadecimal RGB strings e.g. `#FF0000` for red, or `transparent`.

### angle
Number. Rotation in radian. 90° == `Math.PI/2`.

### fillStyle, setFillStyle()
```typescript
type FillStyle = "hachure" | "cross-hatch" | "solid";
setFillStyle (val:number);
```
fillStyle is a string.

`setFillStyle()` accepts a number:
- 0: "hachure"
- 1: "cross-hatch"
- any other number: "solid"

### strokeWidth
Number, sets the width of the stroke.

### strokeStyle, setStrokeStyle()
```typescript
type StrokeStyle = "solid" | "dashed" | "dotted";
setStrokeStyle (val:number);
```
strokeStyle is a string. 

`setStrokeStyle()` accepts a number:
- 0: "solid"
- 1: "dashed"
- any other number: "dotted"

### roughness
Number. Called sloppiness in Excalidraw. Three values are accepted:
- 0: Architect
- 1: Artist
- 2: Cartoonist

### opacity
Number between 0 and 100. The opacity of an object, both stroke and fill.

### strokeSharpness, setStrokeSharpness()
```typescript
type StrokeSharpness = "round" | "sharp";
setStrokeSharpness(val:number);
```
strokeSharpness is a string.

"round" lines are curvey, "sharp" lines break at the turning point.

`setStrokeSharpness()` accepts a number:
- 0: "round"
- any other number: "sharp"

### fontFamily, setFontFamily()
Number. Valid values are 1,2 and 3.

`setFontFamily()` will also accept a number and return the name of the font.
- 1: "Virgil, Segoe UI Emoji"
- 2: "Helvetica, Segoe UI Emoji"
- 3: "Cascadia, Segoe UI Emoji"

### fontSize
Number. Default value is 20 px

### textAlign
String. Alignment of the text horizontally. Valid values are "left", "center", "right".

This is relevant when setting a fix width using the `addText()` function.

### verticalAlign
String. Alignment of the text vertically. Valid values are "top" and "middle".

This is relevant when setting a fix height using the `addText()` function.

### startArrowHead, endArrowHead
String. Valid values are "arrow", "bar", "dot", and "none". Specifies the beginning and ending of an arrow.

This is relevant when using the `addArrow()` and the `connectObjects()` functions.


================================================
FILE: docs/API/introduction.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Introduction to the API
You can access Excalidraw Automate via the ExcalidrawAutomate object. I recommend starting Templater, DataView and QuickAdd scripts with the following code:

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
const ea = ExcalidrawAutomate;
ea.reset();
```

The first line creates a constant so you can avoid writing ExcalidrawAutomate 100x times.

The second line resets ExcalidrawAutomate to defaults. This is important as you will not know which template you executed before, thus you won't know what state you left Excalidraw in.

**⚠ Note:** In case you are using the Excalidraw plugin's built in [Scripting Engine](../ExcalidrawScriptsEngine.md), the engine will take care of initializing the `ea` object.

### Basic logic of using Excalidraw Automate
1. Set the styling of the elements you want to draw
2. Add elements. As you add elements, each new element is added one layer above the previous, thus in case of overlapping objects the later one will be on the top of the prior one.
3. Call `await ea.create();` to instantiate the drawing, or use `ea.setView();` followed by `ea.addElementsToView();` to add your elements to an existing view, or create a PNG or SVG image out of your elements using `await ea.createSVG();` or `await ea.createPNG();`;

You can change the styling between adding different elements. My logic for separating element styling and creation is based on the assumption that you will probably set a stroke color, stroke style, stroke roughness, etc. and draw most of your elements using that. There would be no point in setting all these parameters each time you add an element.

### Before we dive deeper, here are three simple example [Templater](https://github.com/SilentVoid13/Templater) scripts
#### Create a new drawing with custom name, in a custom folder, using a template
This simple script gives you significant additional flexibility over Excalidraw Plugin settings to name your drawings, place them into folders, and to apply templates.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  await ea.create({
    filename    : tp.date.now("HH.mm"), 
    foldername  : tp.date.now("YYYY-MM-DD"),
    templatePath: "Excalidraw/Template1.excalidraw",
    onNewPane   : false
  });
%>
```

#### Create a simple drawing
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.addRect(-150,-50,450,300);
  ea.addText(-100,70,"Left to right");
  ea.addArrow([[-100,100],[100,100]]);

  ea.style.strokeColor = "red";
  ea.addText(100,-30,"top to bottom",{width:200,textAligh:"center"});
  ea.addArrow([[200,0],[200,200]]);
  await ea.create();
%>
```
The script will generate the following drawing:

![FristDemo](https://user-images.githubusercontent.com/14358394/116825643-6e5a8b00-ab90-11eb-9e3a-37c524620d0d.png)

#### Add a TextElement in a box to an open Excalidraw View. 
Position the new element under the currently selected element, with an arrow from the selected element to the added text.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.setView("first"); 
  selectedElement = ea.getViewSelectedElement();
  ea.setStrokeSharpness(0);
  const boxPadding = 5;
  id = ea.addText(
    selectedElement.x + boxPadding,
    selectedElement.y+selectedElement.height+100,
    "[[Next process step]]",
    {
      textAlign:"center",
      box:true,
      boxPadding:boxPadding,
      width:selectedElement.width-boxPadding*2,
    }
  );
  ea.setStrokeSharpness(1);
  ea.style.roughness= 0;
  ea.connectObjectWithViewSelectedElement(
    id,
    "top",
    "bottom",
    {
      numberOfPoints:2,
      startArrowHead:"arrow",
      endArrowHead:"dot", 
      padding:5
  });
  ea.addElementsToView();
%>
```
[Click here to view animation](https://user-images.githubusercontent.com/14358394/131967188-2a488e38-f742-49d9-ae98-33238a8d4712.mp4)





================================================
FILE: docs/API/objects.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Adding objects
These functions will add objects to your drawing. The canvas is infinite, and it accepts negative and positive X and Y values. X values increase left to right, Y values increase top to bottom.

![coordinates](https://user-images.githubusercontent.com/14358394/116825632-6569b980-ab90-11eb-827b-ada598e91e46.png)

### addRect(), addDiamond(), addEllipse()
```typescript
addRect(topX:number, topY:number, width:number, height:number):string
addDiamond(topX:number, topY:number, width:number, height:number):string
addEllipse(topX:number, topY:number, width:number, height:number):string
```
Returns the `id` of the object. The `id` is required when connecting objects with lines. See later.

### addText()
```typescript
addText( 
  topX:number, 
  topY:number, 
  text:string, 
  formatting?:{
    wrapAt?:number, 
    width?:number, 
    height?:number,
    textAlign?:string, 
    box?: "box"|"blob"|"ellipse"|"diamond", 
    boxPadding?:number
  },
  id?:string
):string
```

Adds text to the drawing. 

Formatting parameters are optional:
- If `width` and `height` are not specified, the function will calculate the width and height based on the fontFamily, the fontSize and the text provided.
- In case you want to position a text in the center compared to other elements on the drawing, you can provide a fixed height and width, and you can also specify `textAlign` and `verticalAlign` as described above. e.g.: `{width:500, textAlign:"center"}`
- If you want to add a box around the text, set `{box:"box"|"blob"|"ellipse"|"diamond"}`

Returns the `id` of the object. The `id` is required when connecting objects with lines. See later. If `{box:}` then returns the id of the enclosing box object.

### addLine()
```typescript
addLine(points: [[x:number,y:number]]):string
```
Adds a line following the points provided. Must include at least two points `points.length >= 2`. If more than 2 points are provided the interim points will be added as breakpoints. The line will break with angles if `strokeSharpness` is set to "sharp" and will be curvey if it is set to "round".

Returns the `id` of the object.

### addArrow()
```typescript
addArrow(points: [[x:number,y:number]],formatting?:{startArrowHead?:string,endArrowHead?:string,startObjectId?:string,endObjectId?:string}):string ;
```

Adds an arrow following the points provided. Must include at least two points `points.length >= 2`. If more than 2 points are provided the interim points will be added as breakpoints. The line will break with angles if element `style.strokeSharpness` is set to "sharp" and will be curvey if it is set to "round".

`startArrowHead` and `endArrowHead` specify the type of arrow head to use, as described above. Valid values are "none", "arrow", "dot", and "bar". e.g. `{startArrowHead: "dot", endArrowHead: "arrow"}`

`startObjectId` and `endObjectId` are the object id's of connected objects. I recommend using `connectObjects` instead calling addArrow() for the purpose of connecting objects.

Returns the `id` of the object.

### connectObjects()
```typescript
declare type ConnectionPoint = "top"|"bottom"|"left"|"right";
connectObjects(objectA: string, connectionA: ConnectionPoint, objectB: string, connectionB: ConnectionPoint, formatting?:{numberOfPoints: number,startArrowHead:string,endArrowHead:string, padding: number}):void
```
Connects two objects with an arrow. Will do nothing if either of the two elements is of type `line`, `arrow`, or `freedraw`.

`objectA` and `objectB` are strings. These are the ids of the objects to connect. These IDs are returned by addRect(), addDiamond(), addEllipse() and addText() when creating those objects.

`connectionA` and `connectionB` specify where to connect on the object. Valid values are: "top", "bottom", "left", and "right".

`numberOfPoints` set the number of interim break points for the line. Default value is zero, meaning there will be no breakpoint in between the start and the end points of the arrow. When moving objects on the drawing, these breakpoints will influence how the line is rerouted by Excalidraw.

`startArrowHead` and `endArrowHead` work as described for `addArrow()` above.

### addToGroup()
```typescript
addToGroup(objectIds:[]):string
```
Groups objects listed in `objectIds`. Returns the `id` of the group.


================================================
FILE: docs/API/utility.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Utility functions
### isExcalidrawFile()
```typescript
isExcalidrawFile(f:TFile): boolean
```
Returns true if the file provided is a valid Excalidraw file (either a legacy `*.excalidraw` file or a markdown file with the excalidraw key in the front-matter).

### clear()
`clear()` will clear objects from cache, but will retain element style settings.

### reset()
`reset()` will first call `clear()` and then reset element style to defaults.

### toClipboard()
```typescript
async toClipboard(templatePath?:string)
```
Places the generated drawing to the clipboard. Useful when you don't want to create a new drawing, but want to paste additional items onto an existing drawing.

### getElements()
```typescript
getElements():ExcalidrawElement[];
```
Returns the elements in ExcalidrawAutomate as an array of ExcalidrawElements. This format is useful when working with ExcalidrawRef.

### getElement()
```typescript
getElement(id:string):ExcalidrawElement;
```

Returns the element object matching the id. If the element does not exist, returns null.

### create()
```typescript
async create(params?:{filename: string, foldername:string, templatePath:string, onNewPane: boolean})
```
Creates the drawing and opens it. Returns the full filepath of the created file.

`filename` is the filename without extension of the drawing to be created. If `null`, then Excalidraw will generate a filename.

`foldername` is the folder where the file should be created. If `null` then the default folder for new drawings will be used according to Excalidraw settings.

`templatePath` the filename including full path and extension for a template file to use. This template file will be added as the base layer, all additional objects added via ExcalidrawAutomate will appear on top of elements in the template. If `null` then no template will be used, i.e. an empty white drawing will be the base for adding objects.

`onNewPane` defines where the new drawing should be created. `false` will open the drawing on the current active leaf. `true` will open the drawing by vertically splitting the current leaf.

`frontmatterKeys` are the set of frontmatter keys to apply to the document
  {
    excalidraw-plugin?: "raw"|"parsed",
    excalidraw-link-prefix?: string,
    excalidraw-link-brackets?: boolean,
    excalidraw-url-prefix?: string
  }

Example:
```javascript
create (
  {
    filename:"my drawing", 
    foldername:"myfolder/subfolder/", 
    templatePath: "Excalidraw/template.excalidraw", 
    onNewPane: true, 
    frontmatterKeys: {
      "excalidraw-plugin": "parsed",
      "excalidraw-link-prefix": "",
      "excalidraw-link-brackets": true,
      "excalidraw-url-prefix": "🌐",
    }
  }
);
```
### createSVG()
```typescript
async createSVG(templatePath?:string)
```
Returns an HTML SVGSVGElement containing the generated drawing.

### createPNG()
```typescript
async createPNG(templatePath?:string, scale:number=1)
```
Returns a blob containing a PNG image of the generated drawing.

### wrapText()
```typescript
wrapText(text:string, lineLen:number):string
```
Returns a string wrapped to the provided max lineLen.


### Accessing the open Excalidraw view
You first need to initialize targetView, before using any of the view manipulation functions.

#### targetView
```typescript
targetView: ExcalidrawView
```
The open Excalidraw View configured as the target of the view operations. User `setView` to initialize.

#### setView()
```typescript
setView(view:ExcalidrawView|"first"|"active"):ExcalidrawView
```
Setting the ExcalidrawView that will be the target of the View operations. Valid `view` input values are:
- an object instance of ExcalidrawView
- "first": meaning if there are multiple Excalidraw Views open, pick the first that is returned by `app.workspace.getLeavesOfType("Excalidraw")`
- "active": meaning the currently active view

#### getExcalidrawAPI()
```typescript
getExcalidrawAPI():any
```
Returns the native Excalidraw API (ref.current) for the active drawing specified in `targetView`.
See Excalidraw documentation here: https://www.npmjs.com/package/@excalidraw/excalidraw#ref

#### getViewElements()
```typescript
getViewElements():ExcalidrawElement[] 
```

Returns all the elements from the view.

#### deleteViewElements()
```typescript
deleteViewElements(elToDelete: ExcalidrawElement[]):boolean 
```

Deletes those elements from the view that match the elements provided as the input parameter.

Example to delete the selected elements from the view:
```typescript
ea = ExcalidrawAutomate;
ea.setView("active");
el = ea.getViewSelectedElements();
ea.deleteViewElements();
```

#### getViewSelectedElement()
```typescript
getViewSelectedElement():ExcalidrawElement
```

You first need to set the view calling `setView()`.

If an element is selected in the targetView the function returns the selected element. If multiple elements are selected, either by <kbd>SHIFT+Clicking</kbd> to select multiple elements, or by selecting a group, the first of the elements will be selected. If you want to specify which element to select from a group, double click the desired element in the group.

This function is helpful if you want to add a new element in relation to an existing element in your drawing.

#### getViewSelectedElements()
```typescript
getViewSelectedElements():ExcalidrawElement[]
```

You first need to set the view calling `setView()`.

Gets the array of selected elements in the scene. Returns [] if no elements are selected.

Note: you can call `getExcalidrawAPI().getSceneElements()` to retrieve all the elements in the scene.

#### viewToggleFullScreen()
```typescript
viewToggleFullScreen(forceViewMode?:boolean):void;
```

Toggles targetView between fullscreen mode and normal mode. By setting forceViewMode to `true` will change Excalidraw mode to View mode. Default is `false`.

The function will do nothing on Obsidian Mobile.

#### connectObjectWithViewSelectedElement()
```typescript 
connectObjectWithViewSelectedElement(objectA:string,connectionA: ConnectionPoint, connectionB: ConnectionPoint, formatting?:{numberOfPoints?: number,startArrowHead?:string,endArrowHead?:string, padding?: number}):boolean
```
Same as `connectObjects()`, but ObjectB is the currently selected element in the target ExcalidrawView. The function helps with placing an arrow between a newly created object and the selected element in the target ExcalidrawView.

#### addElementsToView()
```typescript
async addElementsToView(repositionToCursor:boolean=false, save:boolean=false):Promise<boolean>
```
Adds elements created with ExcalidrawAutomate to the target ExcalidrawView.
`repositionToCursor` default is false
- true: the elements will be moved such that the center point of the elements will be aligned with the current position of the pointer on ExcalidrawView. You can point and place elements to a desired location in your drawing using this switch.
- false: elements will be positioned as defined by the x&y coordinates of each element.

`save` default is false
- true: the drawing will be saved after the elements were added.
- false: the drawing will be saved at the next autosave cycle. Use false when adding multiple elements one after the other. Else, best to use true, to minimize risk of data loss.

### onDropHook
```typescript
onDropHook (data: {
  ea: ExcalidrawAutomate, 
  event: React.DragEvent<HTMLDivElement>,
  draggable: any, //Obsidian draggable object
  type: "file"|"text"|"unknown",
  payload: {
    files: TFile[], //TFile[] array of dropped files
    text: string, //string 
  },
  excalidrawFile: TFile, //the file receiving the drop event
  view: ExcalidrawView, //the excalidraw view receiving the drop
  pointerPosition: {x:number, y:number} //the pointer position on canvas at the time of drop
}):boolean;
```

Callback function triggered when an draggable item is dropped on Excalidraw.
The function should return a boolean value. True if the drop was handled by the hook and further native processing should be stopped, and false if Excalidraw should continue with the processing of the drop.
type of drop can be one of:
- "file" if a file from Obsidian file explorer is dropped onto Excalidraw. In this case payload.files will contain the list of files dropped.
- "text" if a link (e.g. url, or wiki link) or other text is dropped. In this case payload.text will contain the received string
- "unknown" if Excalidraw plugin does not recognize the type of dropped object. In this case you can use React.DragEvent to analysed the dropped object.

Use Templater startup templates or similar to set the Hook function. 

```typescript
ea = ExcalidrawAutomate;
ea.onDropHook = (data) => {
  console.log(data); 
  return false;
}
```



================================================
FILE: docs/Examples/apply_template.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Applying an Excalidraw Template to a New Drawing
This example is similar to the one in the introduction, only rotated 90°, and using a template, plus specifying a filename and folder to save the drawing, and opening the new drawing in a new pane.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.style.angle = Math.PI/2; 
  ea.style.strokeWidth = 3.5;
  ea.addRect(-150,-50,450,300);
  ea.addText(-100,70,"Left to right");
  ea.addArrow([[-100,100],[100,100]]);

  ea.style.strokeColor = "red";
  await ea.addText(100,-30,"top to bottom",{width:200,textAlign:"center"});
  ea.addArrow([[200,0],[200,200]]);
  await ea.create({
    filename    :"My Drawing",
    foldername  :"myfolder/fordemo/",
    templatePath:"Excalidraw/Template2.excalidraw",
    onNewPane   :true});
%>
```


================================================
FILE: docs/Examples/connect_objects.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Connect Objects
This [Templater](https://github.com/SilentVoid13/Templater) template demonstrates how to connect two objects using ExcalidrawAutomate.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.addText(-130,-100,"Connecting two objects");
  const a = ea.addRect(-100,-100,100,100);
  const b = ea.addEllipse(200,200,100,100);
  ea.connectObjects(a,"bottom",b,"left",{numberOfPoints: 2}); //see how the line breaks differently when moving objects around
  ea.style.strokeColor = "red";
  ea.connectObjects(a,"right",b,"top",1);
  await ea.create();
%>
```



================================================
FILE: docs/Examples/dataviewjs_familytree.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Family tree from Tasklist using dataviewjs
This is similar to the mindmap script using dataviewjs, but the output is rendered vertically.

### Output
![image](https://user-images.githubusercontent.com/14358394/117549637-d3ecc280-b03b-11eb-952a-840a9a75b6ca.png)

### Input file
Task List looks like:
```markdown
- [ ] OBSIDIAN
    - [ ] Silver
        - [ ] PawPaw Silv
        - [ ] MawMaw Silv
    - [ ] Licat
        - [ ] PeePaw Li
        - [ ] MeeMaw Li
```

### dataviewjs script
Code to render the excalidraw looks like:
```javascript
function crawl(subtasks) {
  let size = subtasks.length > 0 ? 0 : 1; //if no children then a leaf with size 1
  for (let task of subtasks) {
    task["size"] = crawl(task.subtasks);
    size += task.size;
  }
  return size;
}

const tasks = dv.page("FamilyTree.md").file.tasks[0];
tasks["size"] = crawl(tasks.subtasks);

const width = 300;
const height = 150;
const ea = ExcalidrawAutomate;
ea.reset();

function buildMindmap(subtasks, depth, offset, parentObjectID) {
  if (subtasks.length == 0) return;
  let task;
  
  for (let i = 0; i < subtasks.length; i++) {
  task = subtasks[i]
  if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
    task["objectID"] = ea.addText((task.size/2+offset)*width,depth*height,task.text,{box:true})
    ea.connectObjects(parentObjectID,"top",task.objectID,"bottom",{startArrowHead: 'arrow', endArrowHead: 'dot'});
    if (i >= 1) {
            ea.connectObjects(subtasks[i-1]['objectID'],"right",task.objectID,"left", {endArrowHead: 'none'});
    }

    buildMindmap(task.subtasks, depth-1,offset,task.objectID);
    offset += task.size/1.5;
  }
 
}

tasks["objectID"] = ea.addText(width*1.5,height*(tasks.size-1),tasks.text,{box:true, textAlign:"center"});    
buildMindmap(tasks.subtasks, 2, 0, tasks.objectID);

ea.createSVG().then((svg)=>dv.span(svg.outerHTML));
```


================================================
FILE: docs/Examples/dataviewjs_mindmap.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Mindmap from Tasklist using dataviewjs
This is similar to the mindmap script using templater, but because dataview already returns tasks in a tree, it is slightly simpler

### Output
![image](https://user-images.githubusercontent.com/14358394/117548665-71dd8e80-b036-11eb-8a45-4169fdd7cc05.png)

### Input file
The input file is `Demo.md` with the following contents:
```markdown
- [ ] Root task
    - [ ] task 1.1
    - [ ] task 1.2
        - [ ] task 1.2.1
        - [ ] task 1.2.2
    - [ ] task 1.3
        - [ ] task 1.3.1
```

### dataviewjs script
The `dataviewjs` script looks like this: 
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
function crawl(subtasks) {
  let size = subtasks.length > 0 ? 0 : 1; //if no children then a leaf with size 1
  for (let task of subtasks) {
    task["size"] = crawl(task.subtasks);
    size += task.size;
  }
  return size;
}

const tasks = dv.page("Demo.md").file.tasks[0];
tasks["size"] = crawl(tasks.subtasks);

const width = 300;
const height = 100;
const ea = ExcalidrawAutomate;
ea.reset();

function buildMindmap(subtasks, depth, offset, parentObjectID) {
  if (subtasks.length == 0) return;
  for (let task of subtasks) {
    if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
    task["objectID"] = ea.addText(depth*width,(task.size/2+offset)*height,task.text,{box:true})
    ea.connectObjects(parentObjectID,"right",task.objectID,"left",{startArrowHead: 'dot'});
    buildMindmap(task.subtasks, depth+1,offset,task.objectID);
    offset += task.size;
  }
}

tasks["objectID"] = ea.addText(0,(tasks.size/2)*height,tasks.text,{box:true});    
buildMindmap(tasks.subtasks, 1, 0, tasks.objectID);

ea.createSVG().then((svg)=>dv.span(svg.outerHTML));
```


================================================
FILE: docs/Examples/insert_new_drawing.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Insert new drawing into currently edited document
This [Templater](https://github.com/SilentVoid13/Templater) template will prompt you for the title of the drawing. It will create a new drawing with the provided title, and in the folder of the document you were editing. It will then transclude the new drawing at the cursor location and open the new drawing in a new workspace leaf by splitting the current leaf.

*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
  const defaultTitle = tp.date.now("HHmm")+' '+tp.file.title;
  const title = await tp.system.prompt("Title of the drawing?", defaultTitle);
  const folder = tp.file.folder(true);
  const transcludePath = (folder== '/' ? '' : folder + '/') + title + '.excalidraw';
  tR = '![['+transcludePath+']]';
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.setTheme(1); //set Theme to dark
  await ea.create({
    filename : title,
    foldername : folder,
    //templatePath: 'Excalidraw/Template.excalidraw', //uncomment if you want to use a template
    onNewPane : true
  });
%>
```


================================================
FILE: docs/Examples/templater_mindmap.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)
## Generating a simple mindmap from a text outline
This is a slightly more elaborate example. This will generate a mindmap from a tabulated outline.

### Output
![Drawing 2021-05-05 20 52 34](https://user-images.githubusercontent.com/14358394/117194124-00a69d00-ade4-11eb-8b75-5e18a9cbc3cd.png)

### Input file
Example input:
```
- Test 1
	- Test 1.1
- Test 2
	- Test 2.1
	- Test 2.2 
		- Test 2.2.1
		- Test 2.2.2
		- Test 2.2.3
			- Test 2.2.3.1
- Test 3
	- Test 3.1
```

### Templater script
*Use <kbd>CTRL+Shift+V</kbd> to paste code into Obsidian!*
```javascript
<%*
const IDX = Object.freeze({"depth":0, "text":1, "parent":2, "size":3, "children": 4, "objectId":5});

//check if an editor is the active view
const editor = this.app.workspace.activeLeaf?.view?.editor;
if(!editor) return;

//initialize the tree with the title of the document as the first element
let tree = [[0,this.app.workspace.activeLeaf?.view?.getDisplayText(),-1,0,[],0]];
const linecount = editor.lineCount();

//helper function, use regex to calculate indentation depth, and to get line text
function getLineProps (i) {
  props = editor.getLine(i).match(/^(\t*)-\s+(.*)/);
  return [props[1].length+1, props[2]];
}

//a vector that will hold last valid parent for each depth
let parents = [0];

//load outline into tree
for(i=0;i<linecount;i++) {
  [depth,text] = getLineProps(i);
  if(depth>parents.length) parents.push(i+1);
  else parents[depth] = i+1;
  tree.push([depth,text,parents[depth-1],1,[]]);
  tree[parents[depth-1]][IDX.children].push(i+1);
}

//recursive function to crawl the tree and identify height aka. size of each node
function crawlTree(i) {
  if(i>linecount) return 0;
  size = 0;
  if((i+1<=linecount && tree[i+1][IDX.depth] <= tree[i][IDX.depth])|| i == linecount) { //I am a leaf
    tree[i][IDX.size] = 1; 
    return 1; 
  }
  tree[i][IDX.children].forEach((node)=>{ 
    size += crawlTree(node);
  });
  tree[i][IDX.size] = size; 
  return size;   
}

crawlTree(0);

//Build the mindmap in Excalidraw
const width = 300;
const height = 100;
const ea = ExcalidrawAutomate;
ea.reset();

//stores position offset of branch/leaf in height units
offsets = [0];

for(i=0;i<=linecount;i++) {
  depth = tree[i][IDX.depth];
  if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
  tree[i][IDX.objectId] = ea.addText(depth*width,((tree[i][IDX.size]/2)+offsets[depth])*height,tree[i][IDX.text],{box:true});  
  //set child offset equal to parent offset
  if((depth+1)>offsets.length) offsets.push(offsets[depth]);
  else offsets[depth+1] = offsets[depth];
  offsets[depth] += tree[i][IDX.size];
  if(tree[i][IDX.parent]!=-1) {
    ea.connectObjects(tree[tree[i][IDX.parent]][IDX.objectId],"right",tree[i][IDX.objectId],"left",{startArrowHead: 'dot'});
  }
}

await ea.create({onNewPane: true});
%>
```



================================================
FILE: docs/zh-cn/README.md
================================================
# Excalidraw

> 此说明当前更新至 `5569cff`。

【[English](../../README.md) | 简体中文】

👉👉👉 快来查看并为新的 [Obsidian-Excalidraw 社区维基](https://excalidraw-obsidian.online/Hobbies/Excalidraw+Blog/WIKI/Welcome+to+the+WIKI)贡献你的力量吧

Obsidian-Excalidraw 插件将 [Excalidraw](https://excalidraw.com/) 这一功能丰富的草图工具集成到 Obsidian 中。您可以在您的库中存储和编辑 Excalidraw 文件，可以将图形嵌入到文档中，还可以在 Excalidraw 中链接到文档和其他图形。有关 Excalidraw 功能的展示，请查看我的博客文章 [这里](https://www.zsolt.blog/2021/03/showcasing-excalidraw.html) 或观看以下视频。

## 视频演示

<a href="https://youtu.be/P_Q6avJGoWI" target="_blank"><img src="https://github.com/zsviczian/obsidian-excalidraw-plugin/assets/14358394/da34bb33-7610-45e6-b36f-cb7a02a9141b" width="300"/></a>
<a href="https://youtu.be/o0exK-xFP3k" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931370-aa4d88de-c4a8-46cc-aeb2-dc09aa0bea39.jpg" width="300"/></a> 
<a href="https://youtu.be/QKnQgSjJVuc" target="_blank"><img src="https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/thumbnail-getting-started.jpg" width="300"/></a>

### 这是我完整的视频目录：

<a href="https://excalidraw-obsidian.online/Hobbies/Excalidraw+Blog/Catalogue+of+Videos"><img width="380" alt="image" src="https://github.com/zsviczian/obsidian-excalidraw-plugin/assets/14358394/2577e5ad-7a21-4c62-acd5-4fe80c8a8a95"></a>
<br>

<details><summary>10 部分（稍微过时）视频演示</summary>
<a href="https://youtu.be/sY4FoflGaiM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160304-7f211180-e17c-11eb-8363-c52723de1ffd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;1  入门</a><br>
<a href="https://youtu.be/Iy_oVTq12Gw" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160312-8a743d00-e17c-11eb-9fa2-490ef4cbd59e.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;2  基本形状和功能</a><br>
<a href="https://youtu.be/QOL1KF7-kdc" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160323-96f89580-e17c-11eb-9bce-8eb1067a51bb.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;3  元素分组</a><br>
<a href="https://youtu.be/aSgcbfspvfo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160332-9f50d080-e17c-11eb-98e9-fec60fe147d9.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;4  模板库</a><br>
<a href="https://youtu.be/MaJ5jJwBRWs" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160341-a546b180-e17c-11eb-9de8-d87fdc844c9c.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;5  嵌入</a><br>
<a href="https://youtu.be/MXzeCOEExNo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160346-aa0b6580-e17c-11eb-930b-4024807040d1.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;6  链接</a><br>
<a href="https://youtu.be/R0IAg0s-wQE" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160354-b2fc3700-e17c-11eb-81af-9e71e461f6dd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;7  Markdown</a><br>
<a href="https://youtu.be/ibdS7ykwpW4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160360-b8f21800-e17c-11eb-8bd8-79d4e3f6e92d.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;8  模板</a><br>
<a href="https://youtu.be/VRZVujfVab0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160367-bdb6cc00-e17c-11eb-92f1-6f59faea85fd.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;9  Excalidraw 自动化</a><br>
<a href="https://youtu.be/D1iBYo1_jjc" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/125160374-c3141680-e17c-11eb-8cc2-dfaffd903d15.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;10  杂项</a><br>
</details>

<details><summary>将内容嵌入 Excalidraw</summary>
<a href="https://www.youtube.com/watch?v=_c_0zpBJ4Xc&" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/138607067-ccb62f92-48a4-4880-ac6e-68c1bf86ac2c.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;图像元素</a><br>
<a href="https://youtu.be/r08wk-58DPk" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143732412-1c65227e-4381-406d-847a-b001ab3506ca.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;LaTeX 演示</a><br>
<a href="https://youtu.be/tsecSfnTMow" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143732440-90bfa029-8615-462e-ada3-c903d71a82c9.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Markdown 嵌入</a><br>
<a href="https://youtu.be/K6qZkTz8GHs" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/143783906-15cee494-c6d5-4495-a2ca-74634e4e7355.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Markdown 嵌入高级功能</a><br>
<a href="https://youtu.be/Etskjw7a5zo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931461-0979b821-315a-41dd-86f1-31d169b7c127.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;链接到元素、垂直文本对齐、Markdown 样式</a><br>
</details>
<details><summary>脚本引擎商店 - Excalidraw 自动化</summary>
<a href="https://youtu.be/hePJcObHIso" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/145684531-8d9c2992-59ac-4ebc-804a-4cce1777ded2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;介绍脚本引擎</a><br>
<a href="https://youtu.be/lzYdOQ6z8F0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/147889174-6c306d0d-2d29-46cc-a53f-3f0013cf14de.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;脚本引擎商店</a><br>
</details>
<details><summary>使用颜色</summary>
<a href="https://youtu.be/6PLGHBH9VZ4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773147-5418a0ab-6be5-4eb0-a8e4-d6af21b1b483.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;颜色 - Excalidraw 基础（自定义）</a><br>
<a href="https://youtu.be/epYNx2FSf2w" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773211-9e871be7-0795-4dc7-947e-c6c275e690d0.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Excalidraw 调色板（自定义）</a><br>
<a href="https://youtu.be/Amhlv6r9WvM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773268-400cfb1b-6bde-45e0-9e4b-91bbaa461cf0.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;“艺术”颜色渐变</a><br>
<a href="https://youtu.be/r9oB1SlK1GU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/194773527-ef35c8b9-1a6d-4415-9c7e-b667fb17535d.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;美丽草图的简单规则</a><br>
<a href="https://youtu.be/7gJDwNgQ6NU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/195988535-a133a9b9-d094-45ba-ba64-c994b9a1e0ef.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;ColorMaster 脚本编写</a><br>
</details>
<details><summary>链接和块引用</summary>
<a href="https://youtu.be/qiKuqMcNWgU" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/171635214-30533c45-94fa-436e-83a9-b2ec99f190e2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;链接视觉思维的 6 种策略 v4</a><br>
<a href="https://youtu.be/yZQoJg2RCKI" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/185791706-3d9983ab-7cb1-4b27-a016-30c039d84e34.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;图像的块引用部分</a><br>
<a href="https://youtu.be/Etskjw7a5zo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931461-0979b821-315a-41dd-86f1-31d169b7c127.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;链接到元素、垂直文本对齐、Markdown 样式</a><br>
<a href="https://youtu.be/2Y8OhkGiTHg" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/152585752-7eb0371f-0bab-40f6-a194-3b48e5811735.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Excalidraw 原生超链接使用指南</a><br>
</details>
<details><summary>强大工具</summary>
<a href="https://youtu.be/NOuddK6xrr8" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/147283367-e5689385-ea51-4983-81a3-04d810d39f62.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;便签（自动换行）</a><br>
<a href="https://youtu.be/eKFmrSQhFA4" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/149659524-2a4e0a24-40c9-4e66-a6b1-c92f3b88ecd5.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;本地字体</a><br>
<a href="https://youtu.be/vlC1-iBvIfo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/199207784-8bbe14e0-7d10-47d7-971d-20dce8dbd659.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;SVG 导入</a><br>
<a href="https://youtu.be/7gu4ETx7zro" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/202916770-28f2fa64-1ba2-4b40-a7fe-d721b42634f7.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;OCR</a><br>
<a href="https://youtu.be/U2LkBRBk4LY" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/159369910-6371f08d-b5fa-454d-9c6c-948f7e7a7d26.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;绑定/解绑文本与容器，前置标签自定义导出</a><br>
<a href="https://youtu.be/uZz5MgzWXiM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/211054371-8872e01a-77d6-4afc-a0c2-86a55410a8d3.png" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;自定义笔支持</a><br>
</details>
<details><summary>生活质量改善</summary>
<a href="https://youtu.be/qbPIAZguJeo" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/151705333-54e9ffd2-0bd7-4d02-b99e-0bd4e4708d4d.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;移动支持</a><br>
<a href="https://youtu.be/2v9TZmQNO8c" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/153676009-6f86b2d7-c248-49a2-b802-be21c6999e4f.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;托盘模式和可自定义调色板</a><br>
<a href="https://youtu.be/xHPGWR3m0c8" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/154821232-a404b6cf-72fb-4ce4-9d53-619132dce491.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;压缩 JSON 和改进的保存/同步支持</a><br>
<a href="https://youtu.be/gMIKXyhS-dM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/156931428-b2269fd9-87bd-43ab-8558-5572f40dff93.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;Obsidian 工具面板</a><br>
<a href="https://youtu.be/4N6efq1DtH0" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/158008902-12c6a851-237e-4edd-a631-d48e81c904b2.jpg" width="100" style="vertical-align: middle;"/>&nbsp;&nbsp;橡皮擦、左利手模式、改进的文件名配置</a><br>
</details>

### Beta 测试

该插件遵循每月发布的计划。如果您希望获得更频繁的更新，包括新功能（例如，excalidraw.com 上的新内容，但尚未在 Obsidian 中提供）和小的 bug 修复，请加入 beta 社区。

[![缩略图 - 20240803 Excalidraw 发布方法（自定义）](https://github.com/user-attachments/assets/ab40648c-f73f-4bda-a416-52839f918f2a)](https://youtu.be/2poSS-Z91lY)

[![Excalidraw 插件发布策略（手机）](https://github.com/user-attachments/assets/87f1f379-782c-4c32-8b5b-d27fe2d3ac4b)](https://github.com/user-attachments/assets/120a0790-7239-48ae-bfbd-eb249f8b518d)

---

## 功能

- 该插件将 Excalidraw 无缝集成到 Obsidian 中，包括命令面板操作、文件资源管理器功能、选项菜单命令和工具栏按钮。
- 在工具栏按钮或文件资源管理器中 <kbd>CTRL/CMD+鼠标左键</kbd> 以在新面板中创建/打开绘图。

### 设置

设置将允许您根据需要自定义 Excalidraw。该插件提供了大量设置。我尝试为这些设置添加有意义的解释，所以请耐心查找，对于大多数请求，已经存在相关设置。

插件设置分为以下几个部分：

- **基本设置**：例如使用的默认文件夹。
- **保存**：压缩和自动保存间隔。
- **文件名**：配置自动生成的 Excalidraw 文件名。
- **显示**：影响 Excalidraw 处理的设置（例如：左利手模式、主题设置、鼠标滚轮和捏合缩放设置、适应缩放设置）。
- **链接和嵌入**：影响链接和嵌入项在 Excalidraw 画布上行为的设置。
- **Markdown 嵌入设置**：这些设置控制从您的 Vault 嵌入到 Excalidraw 绘图中的 Markdown 文档的行为。
- **嵌入与导出**：控制 Excalidraw 图像在嵌入到 Markdown 文档时的显示方式的设置。
- **自动导出设置**：您可以配置 Excalidraw 在每次保存时创建绘图的 PNG 或 SVG 副本。
- **兼容性功能**：如果您在 Obsidian 之外编辑 Excalidraw 绘图（例如在 LogSeq、Visual Studio、网页等），请检查这些设置。
- **实验性功能**：有一些高级功能作为“巧妙”的 hacks 实现，包括定义本地字体、添加自定义图标以区分 Obsidian 文件资源管理器中的 Excalidraw 文件、OCR 设置等。
- **已安装脚本的设置**：从脚本库安装的一些脚本附带设置。脚本设置在您第一次运行脚本时安装。因此，要访问脚本的设置，请安装脚本，首次运行后在插件设置中查找设置。

#### 模板

- 新绘图的模板。该模板将恢复笔画属性。这意味着您可以在模板中设置笔画颜色、笔画宽度、不透明度、字体系列、字体大小、填充样式、笔画样式等的默认值。这同样适用于 ExcalidrawAutomate。对于 1.6.13 或更高版本，在编辑模板中的 JSON 之前，请确保在设置中启用"在 Markdown 视图中解压缩 Excalidraw JSON"。完成更改后可以禁用此选项。
  - 通过模板，您可以自定义 Excalidraw 使用的调色板。
    - 切换到 Markdown 视图。
    - 滚动到文件底部，找到 `"AppState": {`。
    - 在 AppState 部分末尾找到 `"customColorPalette": {`。
    - 您可以通过添加以下三个变量中的任何一个或全部来指定 Excalidraw 使用的 3 个调色板：
        - `"canvasBackground":[], "elementBackground":[], "elementStroke": []`。
    - 在每个变量的数组中添加有效 HTML 颜色的逗号分隔列表（例如，`#FF0000` 表示红色）。
    - 有关更多帮助，请查看我上面的录像。

#### 导出

- 如果便携性对您很重要：
  - 自动导出 SVG 和/或 PNG 文件，包括同步保持功能，这样您可以将 SVG/PNG 嵌入到文档中，而不是嵌入 Excalidraw 文件。
  - 您可以通过添加 `excalidraw-autoexport` 前置字段键来覆盖单个文件的导出设置。该键的有效值为 `none`、`both`、`png` 和 `svg`。

- 指定嵌入绘图的默认宽度。
- 兼容性功能以自动导出和保持同步 Markdown Excalidraw 文件及旧版 `.excalidraw` 文件。
- 实验性功能可在文件资源管理器中添加自定义标签以标记绘图文件。
- 启用/禁用自动保存。

### 将您的绘图嵌入到 Markdown 文档中

- 您可以使用以下格式自定义嵌入图像的大小和位置：
  - `![[image.excalidraw|100]]`，
  - `![[image.excalidraw|100x100]]`，
  - `![[image.excalidraw|100|left]]`，
  - `![[image.excalidraw|right-wrap]]`，
  - `![[<filename.excalidraw>|<width>x<height>|<alignment>]]`。
  - 您可以通过 CSS 添加自定义 [对齐方式](https://www.scaler.com/topics/align-image-in-html/)。
  - 出现在 `<alignment>` 中的任何文本将被添加到渲染的 SVG 元素样式和包装 DIV 元素中。
  - 有关更多信息，请参见 [styles.css](https://github.com/zsviczian/obsidian-excalidraw-plugin/blob/master/styles.css)。
- Excalidraw 绘图在 Obsidian Publish 中不显示。如果您希望在发布的文档中使用 Excalidraw，可以在插件设置中的 `Embed & Export` 下进行配置，以便在创建新文件时自动将绘图的 PNG 或 SVG 版本插入到文档中。请参见 `type of file to insert into document`。
  - 在 `Export settings` 下，您还可以配置自动导出图像的深色和浅色版本，以便您的发布网站支持深色和浅色模式。

### 超链接和拖放支持

![](https://github.com/zsviczian/obsidian-excalidraw-plugin/blob/master/images/excalidraw-modifiers.png)

#### 超链接

- 支持超链接，例如：
  - `https://zsolt.blog`，
  - `[Obsidian](https://obsidian.md)`，以及
  - 内部链接，例如在绘图文本中使用 `[[My file in vault|Alias]]`。
- 如果您启用了 Obsidian 设置中的“文件与链接/自动更新内部链接”，则文件移动或重命名时链接会自动更新。
- 绘图中的链接会出现在文档的反向链接中。
- 支持嵌入：
  - `![[myfile#^blockref]]` 将绘图转换为该块的嵌入文本。
  - `![[myfile#section]]` 也有效，这将嵌入该部分。
  - 您还可以通过在嵌入后加上最大字符数的花括号来指定嵌入文本的换行，例如 `![[myfile#^blockref]]{40}` 将在 40 个字符处换行。
- 为了方便，您还可以使用命令面板将链接插入到绘图中。
- <kbd>CTRL/CMD + 鼠标悬停</kbd> 可以调出链接的 Obsidian 快速预览。（在 Mac 上为 <kbd>CTRL+CMD+鼠标悬停</kbd>）。
- 使用块引用，您还可以在其他文档中引用和嵌入绘图中出现的文本。

#### 拖放支持

- 您可以从 Obsidian 文件资源管理器中拖动文件，它们将成为 Excalidraw 中指向这些文件的链接。有关各种修饰键组合，请参见上面的表格。
- 注意：将图像锚定到其 100% 尺寸是一个非常小众的功能，具有非常特定的行为，我主要是为自己开发的。
  - （甚至 Excalidraw Obsidian 中的其他功能更是如此 - 也是主要为自己开发的 😉）。
  - 每次打开 Excalidraw 绘图时，这将重置您嵌入的图像为 100% 尺寸，或者如果您在画布上嵌入了使用此功能插入的 Excalidraw 绘图，每次更新嵌入的绘图时，它将缩放回 100% 尺寸。
  - 这意味着即使您在绘图中调整了图像的大小，下次打开文件或修改原始嵌入对象时，它也会重置为 100%。此功能在将绘图分解为单独的 Excalidraw 文件时非常有用，但当它们组合到单个画布上时，您希望各个部分保持其实际大小。我使用此功能从原子绘图构建“一页书”摘要。
- 您可以将文本从 Markdown 视图拖放到 Excalidraw 中。
- 您可以从浏览器中拖放网页地址，它们将成为链接。
- 您可以拖放 YouTube 链接和缩略图，它们将在 Excalidraw 中成为带缩略图的 YouTube 链接。

### LaTeX

使用命令面板操作“插入 LaTeX 公式”插入 LaTeX 公式。您可以在 Markdown 视图中编辑公式，或者通过 <kbd>CTRL/CMD + 鼠标左键</kbd> 点击公式进行编辑。

### 图像支持

- 在 iOS 和 Android 上，您可以通过按下 Excalidraw 中的添加图像按钮从相机添加图像。
- 您可以将图像复制/粘贴到绘图中。图像将保存在您的 Vault 中。
- 您可以按照上面的说明拖放图像。
- URL 链接到网络上的图像：您可以从网页将图像拖放到 Excalidraw。如果在将图像拖放到 Excalidraw 时按住 CTRL 键，图像将不会保存到您的 Vault 中。Excalidraw 将从 URL 加载图像。请注意，如果您没有互联网连接，或者这些图像从互联网上被删除，它们也会从您的绘图中消失。
- 如果您将图像 URL 粘贴到 Excalidraw（只需点击 URL 复制，然后在 Excalidraw 画布上点击粘贴），图像将以链接形式插入到网络图像上。同样，图像不会保存到您的 Vault 中，只有链接会被保存。
- 如果您拖放 YouTube 视频链接，它将转换为一个缩略图，并带有指向视频的元素链接。

### 引用图像部分的块

有关更多详细信息，请参见此 [视频](https://youtu.be/yZQoJg2RCKI)。
- 当通过链接引用 Excalidraw 文件中的画布元素时，可以使用：
  - 元素 ID 或章节标题（即包含 `# <章节标题>` 的文本元素）
      - 例如 `[[file#^elementID]]`，
  - 您可以添加 `group=` 前缀，
      - 例如 `[[file#^group=elementID]]`，或
  - `area=` 前缀，
      - 例如 `[[file#area=Section heading]]`。
  - 如果找到 `group=` 前缀，Excalidraw 将选择与通过元素 ID（块引用）或章节标题引用的元素在同一组中的元素。
  - 如果找到 `area=` 前缀，Excalidraw 将在引用的元素周围插入图像的剪切部分。
  - 请注意，当将 Excalidraw 嵌入为 PNG 到您的 Markdown 文档时，不支持 `area=` 选择器。
  - 引用文本元素的元素 ID 而不带 `group=` 或 `area=` 前缀将以普通文本嵌入该元素。引用非文本元素（例如矩形、椭圆等）而不带 `group=` 或 `area=` 前缀将导致 Obsidian 错误，因为这些元素 ID 在 Excalidraw Markdown 文件中不能够作为块引用。

### Markdown

- 从 1.2.0 版本开始，绘图文件存储在 Markdown 文件中。
  - 您可以为绘图添加标签。
  - 您可以在绘图的 YAML 前置字段中添加元数据。
  - 您在前置字段和 `# Text Elements` 标题之间添加的任何内容将被 Excalidraw 忽略，即您可以在这里添加任何内容，它将作为文档的一部分被保留。
  - Excalidraw 文档现在会在图形视图中显示。
  - 以下前置字段键将自定义绘图的显示方式 - 覆盖一般设置：
    - `excalidraw-link-prefix: "📍"` 内部链接的预览前缀
    - `excalidraw-url-prefix: "🌐"` 外部链接的预览前缀
    - `excalidraw-link-brackets: true|false` 是否在预览中显示链接周围的括号
    - `excalidraw-default-mode: view|zen` 默认以查看模式或禅模式打开此文档。默认查看模式非常适合演示幻灯片。
  - 前置字段标签用于在文件级别自定义图像导出 [519](https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/519)。如果这些键存在，它们将覆盖默认的 Excalidraw 嵌入和导出设置。
    - `excalidraw-export-transparent: true`： true == 透明 / false == 有背景。
    - `excalidraw-export-dark`： true == 深色模式 / false == 浅色模式。
    - `excalidraw-export-padding`：指定图像的导出边距。
    - `excalidraw-export-pngscale`：这仅影响导出为 PNG。指定图像的导出比例。典型范围在 0.5 到 5 之间，但您也可以尝试其他值。
- 从 1.6.13 版本开始，如果您想修改任何 JSON 内容，请在设置中启用"在 Markdown 视图中解压缩 Excalidraw JSON"。

### 将完整的 Markdown 文件嵌入到您的绘图中

从 Obsidian 文件资源管理器中拖动所需文件，同时按住 <kbd>SHIFT</kbd> 将文件放到画布上。
- 使用命令面板操作：`从 Vault 插入 Markdown 文件`
- 使用自定义的 woff、woff2 或 TTF 字体来显示文档，您可以在 Excalidraw 设置中设置默认字体。
- 您可以为渲染 Markdown 文档的快照图像设置自定义 CSS。仅支持操作系统标准字体作为字体系列（[Win10](https://docs.microsoft.com/en-us/typography/fonts/windows_10_font_list)、[Mac & iOS](https://developer.apple.com/fonts/system-fonts/)），此外，您可以使用上述设置添加一个额外的自定义字体。
  - （要查看演示，请观看此 [视频](https://youtu.be/K6qZkTz8GHs) 并查看此
  - [示例 CSS](https://github.com/zsviczian/obsidian-excalidraw-plugin/discussions/281)）。
  - 为了帮助样式设置，您可以查看 Excalidraw 创建的 Markdown 文档的 SVG 快照。
    - 打开 Obsidian 开发者控制台 (<kbd>CTRL+Shift+i</kbd>/<kbd>CMD+OPT+i</kbd>)，并
    - 执行以下命令：`ExcalidrawAutomate.mostRecentMarkdownSVG`
- 您可以通过将以下前置字段键添加到您的 Markdown 文档，按文件控制嵌入 Markdown 文件的外观：
  - `excalidraw-font: Virgil|Cascadia|font_file_name.extension`
  - `excalidraw-font-color: css-color-name|#HEXcolor|any-other-html-standard-format`，
    - 您可以在 [这里](https://www.w3schools.com/colors/colors_names.asp) 找到 CSS 颜色名称。
  - `excalidraw-border-color: css-color-name|#HEXcolor|any-other-html-standard-format`
  - `excalidraw-css: "css-filename|css snippet"`
- 切换到 Markdown 视图或使用 <kbd>WIN+CTRL</kbd>/<kbd>CMD+CTRL</kbd> 点击图像以编辑嵌入的属性：
  - `[[filename#^blockref|WIDTHxMAXHEIGHT]]`

### 自定义字体、自定义笔、OCR 支持、SVG 导入

- 在插件设置中，您可以添加自定义的本地字体。有关更多详细信息，请参见此 [视频](https://youtu.be/eKFmrSQhFA4)。
- 该插件包括使用 Taskbone OCR 的 OCR 支持。有关更多详细信息，请参见此 [视频](https://youtu.be/7gu4ETx7zro)。
- 您可以将 SVG 文件转换为 Excalidraw 绘图（有一些限制）。有关更多详细信息，请参见此 [视频](https://youtu.be/vlC1-iBvIfo)。
- 您可以定义自定义笔和荧光笔，并将其固定到侧边栏。有关更多详细信息，请参见此 [视频](https://youtu.be/OjNhjaH2KjI)。使用 ExcalidrawAutomate，您可以添加对 [自动切换](<ea-scripts/Auto Draw for Pen.md>) 笔的支持，以及对 [硬件橡皮擦按钮](<ea-scripts/Hardware Eraser Support.md>) 的支持。

### 脚本引擎

- 从 1.5.0 版本开始，您可以轻松执行 ExcalidrawAutomate 宏，并为它们分配命令面板快捷键，使用脚本引擎。您可以在 [这里](ea-scripts/README.md) 找到介绍视频和不断增加的可安装脚本库。
- 您可以通过将脚本和随附的 SVG 图标文件移动到文件夹中，将脚本组织成组，放在 Excalidraw 的 Obsidian 工具面板中。请参见演示 [视频](https://youtu.be/wTtaXmRJ7wg?t=16)。

### 其他

- 左利手模式
- 包含完整的
    - [QuickAdd](https://github.com/chhoumann/quickadd)，
    - [Templater](https://silentvoid13.github.io/Templater/) 和
    - [Dataview](https://blacksmithgu.github.io/obsidian-dataview/docs/api/intro/) 支持，通过 ExcalidrawAutomate 实现。
    - 查看 [详细帮助 + 示例](https://zsviczian.github.io/obsidian-excalidraw-plugin/)。
    - 我还有一个 [YouTube ExcalidrawAutomate 播放列表](https://www.youtube.com/playlist?list=PL6mqgtMZ4NP1IR4nXxSlMA4PA5E-qpyHZ)，里面有很多示例。
- 需要 Obsidian Sync 订阅：完整的绘图文件历史记录和设备之间的同步。
- 多语言支持：如果您想通过翻译插件来帮助，请与我联系。

## 反馈、问题、想法、问题

请在 [forum.obsidian.md](https://forum.obsidian.md/t/excalidraw-full-featured-sketching-plugin-in-obsidian) 上参与关于 Excalidraw 插件的讨论。

请前往 [GitHub](https://github.com/zsviczian/obsidian-excalidraw-plugin/issues) 报告错误或请求增强功能。

---

## 感谢支持

如果您喜欢 Excalidraw，请通过在 [https://ko-fi/zsolt](https://ko-fi.com/zsolt) 上请我喝杯咖啡来支持我的工作和热情。

请通过在 Twitter、Reddit 或其他您常用的社交媒体平台上分享 Obsidian Excalidraw 插件来帮助传播消息。

您可以在 Twitter 上找到我 [@zsviczian](https://twitter.com/zsviczian)，以及我的博客 [zsolt.blog](https://zsolt.blog)。

[<img style="float:left" src="https://user-images.githubusercontent.com/14358394/115450238-f39e8100-a21b-11eb-89d0-fa4b82cdbce8.png" width="200">](https://ko-fi.com/zsolt)

---

## Excalidraw 的朋友们
如果您喜欢 Excalidraw，可以考虑尝试 [ExcaliBrain](https://github.com/zsviczian/excalibrain)（也可通过 Obsidian 社区插件获得）。

<a href="https://youtu.be/gOkniMkDPyM" target="_blank"><img src="https://user-images.githubusercontent.com/14358394/169708346-9e41289d-9536-43ec-8f70-2d2ad2d369d6.png" width="300"/></a>


================================================
FILE: docs/zh-cn/AutomateHowTo.md
================================================
[Binary file]


================================================
FILE: docs/zh-cn/docs/readme.md
================================================
[Binary file]


================================================
FILE: docs/zh-cn/docs/ExcalidrawScriptsEngine.md
================================================
# [◀ Excalidraw 自动化使用指南](./readme.md)

> 此说明当前更新至 `768aebf`。

【[English](../../ExcalidrawScriptsEngine.md) | 简体中文】

[![脚本引擎](https://user-images.githubusercontent.com/14358394/145684531-8d9c2992-59ac-4ebc-804a-4cce1777ded2.jpg)](https://youtu.be/hePJcObHIso)

## 简介

请将你的 ExcalidrawAutomate 脚本放入 Excalidraw 设置中定义的文件夹中。脚本文件夹不能是你的 Vault 根目录。

![image](https://user-images.githubusercontent.com/14358394/145673547-b4f57d01-3643-40f9-abfd-14c3bfa5ab93.png)

EA 脚本可以是 markdown 文件、纯文本文件或 .js 文件。唯一的要求是它们必须包含有效的 JavaScript 代码。

![image](https://user-images.githubusercontent.com/14358394/145673674-bb59f227-8eea-43dc-83b8-4d750e1920a8.png)

你可以通过 Obsidian 命令面板从 Excalidraw 访问你的脚本。

![image](https://user-images.githubusercontent.com/14358394/145673652-6b1713e2-edc8-4bc8-8246-3f8df8a4b273.png)

这样你就可以像设置其他 Obsidian 命令一样，为你喜欢的脚本分配快捷键。

![image](https://user-images.githubusercontent.com/14358394/145673633-83b6c969-cead-429b-9721-fd047f980279.png)

## 脚本开发

Excalidraw 脚本会自动接收两个对象：

- `ea`：脚本引擎会初始化 `ea` 对象，包括设置调用脚本时的活动视图为当前视图。
- `utils`：我从 [QuickAdd](https://github.com/chhoumann/quickadd/blob/master/docs/QuickAddAPI.md) 借用了一些实用函数，但目前并非所有 QuickAdd 实用函数都在 Excalidraw 中实现。目前可用的函数如下。详见下方示例。
  - `inputPrompt: (header: string, placeholder?: string, value?: string, buttons?: [{caption:string, action:Function}])`
    - 打开一个提示框请求输入。返回输入的字符串。
    - 你需要使用 await 等待 inputPrompt 的结果。
    - `buttons.action(input: string) => string`。按钮动作将接收当前输入字符串。如果动作返回 null，输入将保持不变。如果动作返回字符串，inputPrompt 将解析为该值。
```typescript
let fileType = "";
const filename = await utils.inputPrompt (
  "Filename for new document",
  "Placeholder",
  "DefaultFilename.md",
  [
    {
      caption: "Markdown",
      action: ()=>{fileType="md";return;}
		},
    {
      caption: "Excalidraw",
      action: ()=>{fileType="ex";return;}
    }
  ]
);

```
  - `suggester: (displayItems: string[], items: any[], hint?: string, instructions?:Instruction[])`
    - 打开一个建议器。显示 displayItems 并返回 items[] 中对应的项。
    - 你需要使用 await 等待 suggester 的结果。
    - 如果用户取消(按ESC键)，suggester 将返回 `undefined`
    - Hint(提示)和 instructions(说明)参数是可选的。
    ```typescript
      interface Instruction {
        command: string;
        purpose: string;
      }
    ```
  - 脚本可以有设置。这些设置作为插件设置的一部分存储，用户也可以通过 Obsidian 插件设置窗口更改。
    - 你可以使用 `ea.getScriptSettings()` 访问当前脚本的设置，并使用 `ea.setScriptSettings(settings:any)` 存储设置值
    - 在插件设置中显示脚本设置的规则如下：
      - 如果设置是简单的字面量(布尔值、数字、字符串)，这些将按原样显示在设置中。设置的名称将作为值的键。
    ```javascript
    ea.setScriptSettings({ 
      "value 1": true, 
      "value 2": 1,
      "value 3": "my string"
    })
    ```
    ![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/SimpleSettings.jpg)
      - 如果设置是一个对象并遵循以下结构，则可以添加描述和值集。也可以使用 `hidden` 键从用户界面中隐藏值。
      ```javascript
      ea.setScriptSettings({
        "value 1": {
          "value": true,
          "description": "This is the description for my boolean value"
        },
        "value 2": {
          "value": 1,
          "description": "This is the description for my numeric value"
        },
        "value 3": {
          "value": "my string",
          "description": "This is the description for my string value",
          "valueset": ["allowed 1","allowed 2","allowed 3"]
        },
        "value 4": {
          "value": "my value",
          "hidden": true
        }        
      });
      ```
      ![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/ComplexSettings.jpg)

---------

## Excalidraw 自动化脚本示例

这些脚本可以在 GitHub [这个](https://github.com/zsviczian/obsidian-excalidraw-plugin/tree/master/ea-scripts)文件夹 📂 中下载为 `.md` 文件。

### 为选中元素添加边框

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-box-elements.jpg)

此脚本将在 Excalidraw 中当前选中的元素周围添加一个包围框

```javascript
if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//check if settings exist. If not, set default values on first run
if(!settings["Default padding"]) {
	settings = {
		"Prompt for padding?": true,
	  "Default padding" : {
			value: 10,
		  description: "Padding between the bounding box of the selected elements, and the box the script creates"
		}
	};
	ea.setScriptSettings(settings);
}

let padding = settings["Default padding"].value;

if(settings["Prompt for padding?"]) {
	padding = parseInt (await utils.inputPrompt("padding?","number",padding.toString()));
}

if(isNaN(padding)) {
  new Notice("The padding value provided is not a number");
  return;
}
elements = ea.getViewSelectedElements();
const box = ea.getBoundingBox(elements);
color = ea
        .getExcalidrawAPI()
        .getAppState()
        .currentItemStrokeColor;
//uncomment for random color:
//color = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
ea.style.strokeColor = color;
id = ea.addRect(
	box.topX - padding,
	box.topY - padding,
	box.width + 2*padding,
	box.height + 2*padding
);
ea.copyViewElementsToEAforEditing(elements);
ea.addToGroup([id].concat(elements.map((el)=>el.id)));
ea.addElementsToView(false);
```

----

### 用箭头连接选中的元素

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-connect-elements.jpg)

此脚本将用箭头连接两个对象。如果任一对象是一组分组元素（例如，一个文本元素与一个包围它的矩形分组），脚本会识别这些组，并将箭头连接到组中最大的对象（假设你想将箭头连接到文本元素周围的框）。
```javascript
if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//set default values on first run
if(!settings["Starting arrowhead"]) {
	settings = {
	  "Starting arrowhead" : {
			value: "none",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Ending arrowhead" : {
			value: "triangle",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Line points" : {
			value: 1,
      description: "Number of line points between start and end"
		}
	};
	ea.setScriptSettings(settings);
}

const arrowStart = settings["Starting arrowhead"].value === "none" ? null : settings["Starting arrowhead"].value;
const arrowEnd = settings["Ending arrowhead"].value === "none" ? null : settings["Ending arrowhead"].value;
const linePoints = Math.floor(settings["Line points"].value);

const elements = ea.getViewSelectedElements();
ea.copyViewElementsToEAforEditing(elements);
groups = ea.getMaximumGroups(elements);

if(groups.length !== 2) {
  //unfortunately getMaxGroups returns duplicated resultset for sticky notes
  //needs additional filtering
  cleanGroups=[];
  idList = [];
  for (group of groups) {
    keep = true;
    for(item of group) if(idList.contains(item.id)) keep = false;
    if(keep) {
      cleanGroups.push(group);
      idList = idList.concat(group.map(el=>el.id))
    }
  }
  if(cleanGroups.length !== 2) return;
  groups = cleanGroups;
}

els = [ 
  ea.getLargestElement(groups[0]),
  ea.getLargestElement(groups[1])
];

ea.style.strokeColor = els[0].strokeColor;
ea.style.strokeWidth = els[0].strokeWidth;
ea.style.strokeStyle = els[0].strokeStyle;
ea.style.strokeSharpness = els[0].strokeSharpness;

ea.connectObjects(
  els[0].id,
  null,
  els[1].id,
  null, 
  {
	endArrowHead: arrowEnd,
	startArrowHead: arrowStart, 
	numberOfPoints: linePoints
  }
);
ea.addElementsToView();
```

----
### 反转选中的箭头

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-reverse-arrow.jpg)

反转选中元素范围内**箭头**的方向。

```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="arrow");
if(!elements || elements.length===0) return;
elements.forEach((el)=>{
	const start = el.startArrowhead;
	el.startArrowhead = el.endArrowhead;
	el.endArrowhead = start;
});
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```

----

### 设置选中元素的线条宽度

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-stroke-width.jpg)

当你缩放自由绘制的草图并想要减小或增加它们的线条宽度时，这个脚本会很有帮助。
```javascript
let width = (ea.getViewSelectedElement().strokeWidth??1).toString();
width = await utils.inputPrompt("Width?","number",width);
const elements=ea.getViewSelectedElements();
ea.copyViewElementsToEAforEditing(elements);
ea.getElements().forEach((el)=>el.strokeWidth=width);
ea.addElementsToView();
```

----

### 设置网格大小

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-grid.jpg)

Excalidraw 中默认的网格大小是 20。目前通过用户界面无法更改网格大小。
```javascript
const grid = parseInt(await utils.inputPrompt("Grid size?",null,"20"));
const api = ea.getExcalidrawAPI();
let appState = api.getAppState();
appState.gridSize = grid;
api.updateScene({
  appState,
  commitToHistory:false
});
```

----

### 设置元素尺寸和位置

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-dimensions.jpg)

目前在 Excalidraw 中还没有办法指定对象的精确位置和大小。你可以使用以下简单脚本来解决这个问题。
```javascript
const elements = ea.getViewSelectedElements();
if(elements.length === 0) return;
const el = ea.getLargestElement(elements);
const sizeIn = [el.x,el.y,el.width,el.height].join(",");
let res = await utils.inputPrompt("x,y,width,height?",null,sizeIn);
res = res.split(",");
if(res.length !== 4) return;
let size = [];
for (v of res) {
  const i = parseInt(v);
  if(isNaN(i)) return;
  size.push(i);
}
el.x = size[0];
el.y = size[1];
el.width = size[2];
el.height = size[3];
ea.copyViewElementsToEAforEditing([el]);
ea.addElementsToView();
```

----

### 项目符号

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-bullet-point.jpg)

此脚本会在选中的每个文本元素的左上角添加一个小圆圈，并将文本和"项目符号"组合成一个组。
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
ea.copyViewElementsToEAforEditing(elements);
const padding = 10;
elements.forEach((el)=>{
  ea.style.strokeColor = el.strokeColor;
  const size = el.fontSize/2;
  const ellipseId = ea.addEllipse(
    el.x-padding-size,
    el.y+size/2,
    size,
    size
  );
  ea.addToGroup([el.id,ellipseId]);
});
ea.addElementsToView();
```

----

### 按行分割文本

**!!!需要 Excalidraw 1.5.1 或更高版本**

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-split-lines.jpg)

将文本块按行分割成单独的文本元素，以便更容易重新组织
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
elements.forEach((el)=>{
  ea.style.strokeColor = el.strokeColor;
  ea.style.fontFamily  = el.fontFamily;
  ea.style.fontSize    = el.fontSize;
  const text = el.text.split("\n");
  for(i=0;i<text.length;i++) {
	ea.addText(el.x,el.y+i*el.height/text.length,text[i]);
  }
});
ea.addElementsToView();
ea.deleteViewElements(elements);
```

----

### 设置文本对齐方式

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-text-align.jpg)

设置文本块的对齐方式（居中、右对齐、左对齐）。如果你想为选择文本对齐方式设置键盘快捷键，这个脚本会很有用。
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
if(elements.length===0) return;
let align = ["left","right","center"];
align = await utils.suggester(align,align);
elements.forEach((el)=>el.textAlign = align);
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```

----

### 设置字体

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-font-family.jpg)

设置文本块的字体(Virgil、Helvetica、Cascadia)。如果你想为选择字体设置键盘快捷键，这个功能会很有用。
```javascript
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
if(elements.length===0) return;
let font = ["Virgil","Helvetica","Cascadia"];
font = parseInt(await utils.suggester(font,["1","2","3"]));
if (isNaN(font)) return;
elements.forEach((el)=>el.fontFamily = font);
ea.copyViewElementsToEAforEditing(elements);
ea.addElementsToView();
```



================================================
FILE: docs/zh-cn/docs/API/attributes_functions_overview.md
================================================
# [◀ Excalidraw 自动化使用指南](../readme.md)

## 属性和函数概览

以下是 ExcalidrawAutomate 实现的接口:

你可以在这里找到源文件: [ExcalidrawAutomate.d.ts](ExcalidrawAutomate.d.ts)。

```javascript
/// <reference types="react" />
import ExcalidrawPlugin from "src/main";
import { FillStyle, StrokeStyle, ExcalidrawElement, ExcalidrawBindableElement, FileId, NonDeletedExcalidrawElement, ExcalidrawImageElement, StrokeRoundness, RoundnessType } from "@zsviczian/excalidraw/types/element/types";
import { Editor, OpenViewState, TFile, WorkspaceLeaf } from "obsidian";
import * as obsidian_module from "obsidian";
import ExcalidrawView, { ExportSettings } from "src/ExcalidrawView";
import { AppState, BinaryFileData, DataURL, ExcalidrawImperativeAPI, Point } from "@zsviczian/excalidraw/types/types";
import { EmbeddedFilesLoader } from "src/EmbeddedFileLoader";
import { ConnectionPoint, DeviceType } from "src/types";
import { ColorMaster } from "colormaster";
import { TInput } from "colormaster/types";
import { ClipboardData } from "@zsviczian/excalidraw/types/clipboard";
import { PaneTarget } from "src/utils/modifierkeyHelper";
export declare class ExcalidrawAutomate {
    /**
     * Utility function that returns the Obsidian Module object.
     */
    get obsidian(): typeof obsidian_module;
    get DEVICE(): DeviceType;
    getAttachmentFilepath(filename: string): Promise<string>;
    /**
     * Prompts the user with a dialog to select new file action.
     * - create markdown file
     * - create excalidraw file
     * - cancel action
     * The new file will be relative to this.targetView.file.path, unless parentFile is provided.
     * If shouldOpenNewFile is true, the new file will be opened in a workspace leaf.
     * targetPane control which leaf will be used for the new file.
     * Returns the TFile for the new file or null if the user cancelled the action.
     * @param newFileNameOrPath
     * @param shouldOpenNewFile
     * @param targetPane //type PaneTarget = "active-pane"|"new-pane"|"popout-window"|"new-tab"|"md-properties";
     * @param parentFile
     * @returns
     */
    newFilePrompt(newFileNameOrPath: string, shouldOpenNewFile: boolean, targetPane?: PaneTarget, parentFile?: TFile): Promise<TFile | null>;
    /**
     * Generates a new Obsidian Leaf following Excalidraw plugin settings such as open in Main Workspace or not, open in adjacent pane if available, etc.
     * @param origo // the currently active leaf, the origin of the new leaf
     * @param targetPane //type PaneTarget = "active-pane"|"new-pane"|"popout-window"|"new-tab"|"md-properties";
     * @returns
     */
    getLeaf(origo: WorkspaceLeaf, targetPane?: PaneTarget): WorkspaceLeaf;
    /**
     * Returns the editor or leaf.view of the currently active embedded obsidian file.
     * If view is not provided, ea.targetView is used.
     * If the embedded file is a markdown document the function will return
     * {file:TFile, editor:Editor} otherwise it will return {view:any}. You can check view type with view.getViewType();
     * @param view
     * @returns
     */
    getActiveEmbeddableViewOrEditor(view?: ExcalidrawView): {
        view: any;
    } | {
        file: TFile;
        editor: Editor;
    } | null;
    plugin: ExcalidrawPlugin;
    elementsDict: {
        [key: string]: any;
    };
    imagesDict: {
        [key: FileId]: any;
    };
    mostRecentMarkdownSVG: SVGSVGElement;
    style: {
        strokeColor: string;
        backgroundColor: string;
        angle: number;
        fillStyle: FillStyle;
        strokeWidth: number;
        strokeStyle: StrokeStyle;
        roughness: number;
        opacity: number;
        strokeSharpness?: StrokeRoundness;
        roundness: null | {
            type: RoundnessType;
            value?: number;
        };
        fontFamily: number;
        fontSize: number;
        textAlign: string;
        verticalAlign: string;
        startArrowHead: string;
        endArrowHead: string;
    };
    canvas: {
        theme: string;
        viewBackgroundColor: string;
        gridSize: number;
    };
    colorPalette: {};
    constructor(plugin: ExcalidrawPlugin, view?: ExcalidrawView);
    /**
     *
     * @returns the last recorded pointer position on the Excalidraw canvas
     */
    getViewLastPointerPosition(): {
        x: number;
        y: number;
    };
    /**
     *
     * @returns
     */
    getAPI(view?: ExcalidrawView): ExcalidrawAutomate;
    /**
     * @param val //0:"hachure", 1:"cross-hatch" 2:"solid"
     * @returns
     */
    setFillStyle(val: number): "hachure" | "cross-hatch" | "solid";
    /**
     * @param val //0:"solid", 1:"dashed", 2:"dotted"
     * @returns
     */
    setStrokeStyle(val: number): "solid" | "dashed" | "dotted";
    /**
     * @param val //0:"round", 1:"sharp"
     * @returns
     */
    setStrokeSharpness(val: number): "round" | "sharp";
    /**
     * @param val //1: Virgil, 2:Helvetica, 3:Cascadia
     * @returns
     */
    setFontFamily(val: number): "Virgil, Segoe UI Emoji" | "Helvetica, Segoe UI Emoji" | "Cascadia, Segoe UI Emoji" | "LocalFont";
    /**
     * @param val //0:"light", 1:"dark"
     * @returns
     */
    setTheme(val: number): "light" | "dark";
    /**
     * @param objectIds
     * @returns
     */
    addToGroup(objectIds: string[]): string;
    /**
     * @param templatePath
     */
    toClipboard(templatePath?: string): Promise<void>;
    /**
     * @param file: TFile
     * @returns ExcalidrawScene
     */
    getSceneFromFile(file: TFile): Promise<{
        elements: ExcalidrawElement[];
        appState: AppState;
    }>;
    /**
     * get all elements from ExcalidrawAutomate elementsDict
     * @returns elements from elementsDict
     */
    getElements(): ExcalidrawElement[];
    /**
     * get single element from ExcalidrawAutomate elementsDict
     * @param id
     * @returns
     */
    getElement(id: string): ExcalidrawElement;
    /**
     * create a drawing and save it to filename
     * @param params
     *   filename: if null, default filename as defined in Excalidraw settings
     *   foldername: if null, default folder as defined in Excalidraw settings
     * @returns
     */
    create(params?: {
        filename?: string;
        foldername?: string;
        templatePath?: string;
        onNewPane?: boolean;
        frontmatterKeys?: {
            "excalidraw-plugin"?: "raw" | "parsed";
            "excalidraw-link-prefix"?: string;
            "excalidraw-link-brackets"?: boolean;
            "excalidraw-url-prefix"?: string;
            "excalidraw-export-transparent"?: boolean;
            "excalidraw-export-dark"?: boolean;
            "excalidraw-export-padding"?: number;
            "excalidraw-export-pngscale"?: number;
            "excalidraw-default-mode"?: "view" | "zen";
            "excalidraw-onload-script"?: string;
            "excalidraw-linkbutton-opacity"?: number;
            "excalidraw-autoexport"?: boolean;
        };
        plaintext?: string;
    }): Promise<string>;
    /**
     *
     * @param templatePath
     * @param embedFont
     * @param exportSettings use ExcalidrawAutomate.getExportSettings(boolean,boolean)
     * @param loader use ExcalidrawAutomate.getEmbeddedFilesLoader(boolean?)
     * @param theme
     * @returns
     */
    createSVG(templatePath?: string, embedFont?: boolean, exportSettings?: ExportSettings, loader?: EmbeddedFilesLoader, theme?: string, padding?: number): Promise<SVGSVGElement>;
    /**
     *
     * @param templatePath
     * @param scale
     * @param exportSettings use ExcalidrawAutomate.getExportSettings(boolean,boolean)
     * @param loader use ExcalidrawAutomate.getEmbeddedFilesLoader(boolean?)
     * @param theme
     * @returns
     */
    createPNG(templatePath?: string, scale?: number, exportSettings?: ExportSettings, loader?: EmbeddedFilesLoader, theme?: string, padding?: number): Promise<any>;
    /**
     *
     * @param text
     * @param lineLen
     * @returns
     */
    wrapText(text: string, lineLen: number): string;
    private boxedElement;
    addIFrame(topX: number, topY: number, width: number, height: number, url?: string, file?: TFile): string;
    /**
   *
   * @param topX
   * @param topY
   * @param width
   * @param height
   * @returns
   */
    addEmbeddable(topX: number, topY: number, width: number, height: number, url?: string, file?: TFile): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addRect(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addDiamond(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addEllipse(topX: number, topY: number, width: number, height: number): string;
    /**
     *
     * @param topX
     * @param topY
     * @param width
     * @param height
     * @returns
     */
    addBlob(topX: number, topY: number, width: number, height: number): string;
    /**
     * Refresh the size of a text element to fit its contents
     * @param id - the id of the text element
     */
    refreshTextElementSize(id: string): void;
    /**
     *
     * @param topX
     * @param topY
     * @param text
     * @param formatting
     *   box: if !null, text will be boxed
     * @param id
     * @returns
     */
    addText(topX: number, topY: number, text: string, formatting?: {
        wrapAt?: number;
        width?: number;
        height?: number;
        textAlign?: "left" | "center" | "right";
        box?: boolean | "box" | "blob" | "ellipse" | "diamond";
        boxPadding?: number;
        boxStrokeColor?: string;
        textVerticalAlign?: "top" | "middle" | "bottom";
    }, id?: string): string;
    /**
     *
     * @param points
     * @returns
     */
    addLine(points: [[x: number, y: number]]): string;
    /**
     *
     * @param points
     * @param formatting
     * @returns
     */
    addArrow(points: [x: number, y: number][], formatting?: {
        startArrowHead?: string;
        endArrowHead?: string;
        startObjectId?: string;
        endObjectId?: string;
    }): string;
    /**
     *
     * @param topX
     * @param topY
     * @param imageFile
     * @returns
     */
    addImage(topX: number, topY: number, imageFile: TFile | string, scale?: boolean, //default is true which will scale the image to MAX_IMAGE_SIZE, false will insert image at 100% of its size
    anchor?: boolean): Promise<string>;
    /**
     *
     * @param topX
     * @param topY
     * @param tex
     * @returns
     */
    addLaTex(topX: number, topY: number, tex: string): Promise<string>;
    /**
     *
     * @param objectA
     * @param connectionA type ConnectionPoint = "top" | "bottom" | "left" | "right" | null
     * @param objectB
     * @param connectionB when passed null, Excalidraw will automatically decide
     * @param formatting
     *   numberOfPoints: points on the line. Default is 0 ie. line will only have a start and end point
     *   startArrowHead: "triangle"|"dot"|"arrow"|"bar"|null
     *   endArrowHead: "triangle"|"dot"|"arrow"|"bar"|null
     *   padding:
     * @returns
     */
    connectObjects(objectA: string, connectionA: ConnectionPoint | null, objectB: string, connectionB: ConnectionPoint | null, formatting?: {
        numberOfPoints?: number;
        startArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        endArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        padding?: number;
    }): string;
    /**
     * Adds a text label to a line or arrow. Currently only works with a straight (2 point - start & end - line)
     * @param lineId id of the line or arrow object in elementsDict
     * @param label the label text
     * @returns undefined (if unsuccessful) or the id of the new text element
     */
    addLabelToLine(lineId: string, label: string): string;
    /**
     * clear elementsDict and imagesDict only
     */
    clear(): void;
    /**
     * clear() + reset all style values to default
     */
    reset(): void;
    /**
     * returns true if MD file is an Excalidraw file
     * @param f
     * @returns
     */
    isExcalidrawFile(f: TFile): boolean;
    targetView: ExcalidrawView;
    /**
     * sets the target view for EA. All the view operations and the access to Excalidraw API will be performend on this view
     * if view is null or undefined, the function will first try setView("active"), then setView("first").
     * @param view
     * @returns targetView
     */
    setView(view?: ExcalidrawView | "first" | "active"): ExcalidrawView;
    /**
     *
     * @returns https://github.com/excalidraw/excalidraw/tree/master/src/packages/excalidraw#ref
     */
    getExcalidrawAPI(): any;
    /**
     * get elements in View
     * @returns
     */
    getViewElements(): ExcalidrawElement[];
    /**
     *
     * @param elToDelete
     * @returns
     */
    deleteViewElements(elToDelete: ExcalidrawElement[]): boolean;
    /**
     * get the selected element in the view, if more are selected, get the first
     * @returns
     */
    getViewSelectedElement(): any;
    /**
     *
     * @returns
     */
    getViewSelectedElements(): any[];
    /**
     *
     * @param el
     * @returns TFile file handle for the image element
     */
    getViewFileForImageElement(el: ExcalidrawElement): TFile | null;
    /**
     * copies elements from view to elementsDict for editing
     * @param elements
     */
    copyViewElementsToEAforEditing(elements: ExcalidrawElement[]): void;
    /**
     *
     * @param forceViewMode
     * @returns
     */
    viewToggleFullScreen(forceViewMode?: boolean): void;
    setViewModeEnabled(enabled: boolean): void;
    /**
     * This function gives you a more hands on access to Excalidraw.
     * @param scene - The scene you want to load to Excalidraw
     * @param restore - Use this if the scene includes legacy excalidraw file elements that need to be converted to the latest excalidraw data format (not a typical usecase)
     * @returns
     */
    viewUpdateScene(scene: {
        elements?: ExcalidrawElement[];
        appState?: AppState;
        files?: BinaryFileData;
        commitToHistory?: boolean;
    }, restore?: boolean): void;
    /**
     * connect an object to the selected element in the view
     * @param objectA ID of the element
     * @param connectionA
     * @param connectionB
     * @param formatting
     * @returns
     */
    connectObjectWithViewSelectedElement(objectA: string, connectionA: ConnectionPoint | null, connectionB: ConnectionPoint | null, formatting?: {
        numberOfPoints?: number;
        startArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        endArrowHead?: "triangle" | "dot" | "arrow" | "bar" | null;
        padding?: number;
    }): boolean;
    /**
     * zoom tarteView to fit elements provided as input
     * elements === [] will zoom to fit the entire scene
     * selectElements toggles whether the elements should be in a selected state at the end of the operation
     * @param selectElements
     * @param elements
     */
    viewZoomToElements(selectElements: boolean, elements: ExcalidrawElement[]): void;
    /**
     * Adds elements from elementsDict to the current view
     * @param repositionToCursor default is false
     * @param save default is true
     * @param newElementsOnTop controls whether elements created with ExcalidrawAutomate
     *   are added at the bottom of the stack or the top of the stack of elements already in the view
     *   Note that elements copied to the view with copyViewElementsToEAforEditing retain their
     *   position in the stack of elements in the view even if modified using EA
     *   default is false, i.e. the new elements get to the bottom of the stack
     * @param shouldRestoreElements - restore elements - auto-corrects broken, incomplete or old elements included in the update
     * @returns
     */
    addElementsToView(repositionToCursor?: boolean, save?: boolean, newElementsOnTop?: boolean, shouldRestoreElements?: boolean): Promise<boolean>;
    /**
     * Register instance of EA to use for hooks with TargetView
     * By default ExcalidrawViews will check window.ExcalidrawAutomate for event hooks.
     * Using this event you can set a different instance of Excalidraw Automate for hooks
     * @returns true if successful
     */
    registerThisAsViewEA(): boolean;
    /**
     * Sets the targetView EA to window.ExcalidrawAutomate
     * @returns true if successful
     */
    deregisterThisAsViewEA(): boolean;
    /**
     * If set, this callback is triggered when the user closes an Excalidraw view.
     */
    onViewUnloadHook: (view: ExcalidrawView) => void;
    /**
     * If set, this callback is triggered, when the user changes the view mode.
     * You can use this callback in case you want to do something additional when the user switches to view mode and back.
     */
    onViewModeChangeHook: (isViewModeEnabled: boolean, view: ExcalidrawView, ea: ExcalidrawAutomate) => void;
    /**
    * If set, this callback is triggered, when the user hovers a link in the scene.
    * You can use this callback in case you want to do something additional when the onLinkHover event occurs.
    * This callback must return a boolean value.
    * In case you want to prevent the excalidraw onLinkHover action you must return false, it will stop the native excalidraw onLinkHover management flow.
    */
    onLinkHoverHook: (element: NonDeletedExcalidrawElement, linkText: string, view: ExcalidrawView, ea: ExcalidrawAutomate) => boolean;
    /**
    * If set, this callback is triggered, when the user clicks a link in the scene.
    * You can use this callback in case you want to do something additional when the onLinkClick event occurs.
    * This callback must return a boolean value.
    * In case you want to prevent the excalidraw onLinkClick action you must return false, it will stop the native excalidraw onLinkClick management flow.
    */
    onLinkClickHook: (element: ExcalidrawElement, linkText: string, event: MouseEvent, view: ExcalidrawView, ea: ExcalidrawAutomate) => boolean;
    /**
     * If set, this callback is triggered, when Excalidraw receives an onDrop event.
     * You can use this callback in case you want to do something additional when the onDrop event occurs.
     * This callback must return a boolean value.
     * In case you want to prevent the excalidraw onDrop action you must return false, it will stop the native excalidraw onDrop management flow.
     */
    onDropHook: (data: {
        ea: ExcalidrawAutomate;
        event: React.DragEvent<HTMLDivElement>;
        draggable: any;
        type: "file" | "text" | "unknown";
        payload: {
            files: TFile[];
            text: string;
        };
        excalidrawFile: TFile;
        view: ExcalidrawView;
        pointerPosition: {
            x: number;
            y: number;
        };
    }) => boolean;
    /**
     * If set, this callback is triggered, when Excalidraw receives an onPaste event.
     * You can use this callback in case you want to do something additional when the
     * onPaste event occurs.
     * This callback must return a boolean value.
     * In case you want to prevent the excalidraw onPaste action you must return false,
     * it will stop the native excalidraw onPaste management flow.
     */
    onPasteHook: (data: {
        ea: ExcalidrawAutomate;
        payload: ClipboardData;
        event: ClipboardEvent;
        excalidrawFile: TFile;
        view: ExcalidrawView;
        pointerPosition: {
            x: number;
            y: number;
        };
    }) => boolean;
    /**
     * if set, this callback is triggered, when an Excalidraw file is opened
     * You can use this callback in case you want to do something additional when the file is opened.
     * This will run before the file level script defined in the `excalidraw-onload-script` frontmatter.
     */
    onFileOpenHook: (data: {
        ea: ExcalidrawAutomate;
        excalidrawFile: TFile;
        view: ExcalidrawView;
    }) => Promise<void>;
    /**
     * if set, this callback is triggered, when an Excalidraw file is created
     * see also: https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/1124
     */
    onFileCreateHook: (data: {
        ea: ExcalidrawAutomate;
        excalidrawFile: TFile;
        view: ExcalidrawView;
    }) => Promise<void>;
    /**
     * If set, this callback is triggered whenever the active canvas color changes
     */
    onCanvasColorChangeHook: (ea: ExcalidrawAutomate, view: ExcalidrawView, //the excalidraw view 
    color: string) => void;
    /**
     * utility function to generate EmbeddedFilesLoader object
     * @param isDark
     * @returns
     */
    getEmbeddedFilesLoader(isDark?: boolean): EmbeddedFilesLoader;
    /**
     * utility function to generate ExportSettings object
     * @param withBackground
     * @param withTheme
     * @returns
     */
    getExportSettings(withBackground: boolean, withTheme: boolean): ExportSettings;
    /**
     * get bounding box of elements
     * bounding box is the box encapsulating all of the elements completely
     * @param elements
     * @returns
     */
    getBoundingBox(elements: ExcalidrawElement[]): {
        topX: number;
        topY: number;
        width: number;
        height: number;
    };
    /**
     * elements grouped by the highest level groups
     * @param elements
     * @returns
     */
    getMaximumGroups(elements: ExcalidrawElement[]): ExcalidrawElement[][];
    /**
     * gets the largest element from a group. useful when a text element is grouped with a box, and you want to connect an arrow to the box
     * @param elements
     * @returns
     */
    getLargestElement(elements: ExcalidrawElement[]): ExcalidrawElement;
    /**
     * @param element
     * @param a
     * @param b
     * @param gap
     * @returns 2 or 0 intersection points between line going through `a` and `b`
     *   and the `element`, in ascending order of distance from `a`.
     */
    intersectElementWithLine(element: ExcalidrawBindableElement, a: readonly [number, number], b: readonly [number, number], gap?: number): Point[];
    /**
     * Gets the groupId for the group that contains all the elements, or null if such a group does not exist
     * @param elements
     * @returns null or the groupId
     */
    getCommonGroupForElements(elements: ExcalidrawElement[]): string;
    /**
     * Gets all the elements from elements[] that share one or more groupIds with element.
     * @param element
     * @param elements - typically all the non-deleted elements in the scene
     * @returns
     */
    getElementsInTheSameGroupWithElement(element: ExcalidrawElement, elements: ExcalidrawElement[]): ExcalidrawElement[];
    /**
     * Gets all the elements from elements[] that are contained in the frame.
     * @param element
     * @param elements - typically all the non-deleted elements in the scene
     * @returns
     */
    getElementsInFrame(frameElement: ExcalidrawElement, elements: ExcalidrawElement[]): ExcalidrawElement[];
    /**
     * See OCR plugin for example on how to use scriptSettings
     * Set by the ScriptEngine
     */
    activeScript: string;
    /**
     *
     * @returns script settings. Saves settings in plugin settings, under the activeScript key
     */
    getScriptSettings(): {};
    /**
     * sets script settings.
     * @param settings
     * @returns
     */
    setScriptSettings(settings: any): Promise<void>;
    /**
     * Open a file in a new workspaceleaf or reuse an existing adjacent leaf depending on Excalidraw Plugin Settings
     * @param file
     * @param openState - if not provided {active: true} will be used
     * @returns
     */
    openFileInNewOrAdjacentLeaf(file: TFile, openState?: OpenViewState): WorkspaceLeaf;
    /**
     * measure text size based on current style settings
     * @param text
     * @returns
     */
    measureText(text: string): {
        width: number;
        height: number;
    };
    /**
     * Returns the size of the image element at 100% (i.e. the original size)
     * @param imageElement an image element from the active scene on targetView
     */
    getOriginalImageSize(imageElement: ExcalidrawImageElement): Promise<{
        width: number;
        height: number;
    }>;
    /**
     * verifyMinimumPluginVersion returns true if plugin version is >= than required
     * recommended use:
     * if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.20")) {new Notice("message");return;}
     * @param requiredVersion
     * @returns
     */
    verifyMinimumPluginVersion(requiredVersion: string): boolean;
    /**
     * Check if view is instance of ExcalidrawView
     * @param view
     * @returns
     */
    isExcalidrawView(view: any): boolean;
    /**
     * sets selection in view
     * @param elements
     * @returns
     */
    selectElementsInView(elements: ExcalidrawElement[] | string[]): void;
    /**
     * @returns an 8 character long random id
     */
    generateElementId(): string;
    /**
     * @param element
     * @returns a clone of the element with a new id
     */
    cloneElement(element: ExcalidrawElement): ExcalidrawElement;
    /**
     * Moves the element to a specific position in the z-index
     */
    moveViewElementToZIndex(elementId: number, newZIndex: number): void;
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    hexStringToRgb(color: string): number[];
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    rgbToHexString(color: number[]): string;
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    hslToRgb(color: number[]): number[];
    /**
     * Deprecated. Use getCM / ColorMaster instead
     * @param color
     * @returns
     */
    rgbToHsl(color: number[]): number[];
    /**
     *
     * @param color
     * @returns
     */
    colorNameToHex(color: string): string;
    /**
     * https://github.com/lbragile/ColorMaster
     * @param color
     * @returns
     */
    getCM(color: TInput): ColorMaster;
    importSVG(svgString: string): boolean;
}
export declare function initExcalidrawAutomate(plugin: ExcalidrawPlugin): Promise<ExcalidrawAutomate>;
export declare function destroyExcalidrawAutomate(): void;
export declare function _measureText(newText: string, fontSize: number, fontFamily: number, lineHeight: number): {
    w: number;
    h: number;
    baseline: number;
};
export declare const generatePlaceholderDataURL: (width: number, height: number) => DataURL;
export declare function createPNG(templatePath: string, scale: number, exportSettings: ExportSettings, loader: EmbeddedFilesLoader, forceTheme: string, canvasTheme: string, canvasBackgroundColor: string, automateElements: ExcalidrawElement[], plugin: ExcalidrawPlugin, depth: number, padding?: number, imagesDict?: any): Promise<Blob>;
export declare function createSVG(templatePath: string, embedFont: boolean, exportSettings: ExportSettings, loader: EmbeddedFilesLoader, forceTheme: string, canvasTheme: string, canvasBackgroundColor: string, automateElements: ExcalidrawElement[], plugin: ExcalidrawPlugin, depth: number, padding?: number, imagesDict?: any, convertMarkdownLinksToObsidianURLs?: boolean): Promise<SVGSVGElement>;
export declare function estimateBounds(elements: ExcalidrawElement[]): [number, number, number, number];
export declare function repositionElementsToCursor(elements: ExcalidrawElement[], newPosition: {
    x: number;
    y: number;
}, center: boolean, api: ExcalidrawImperativeAPI): ExcalidrawElement[];
export declare const insertLaTeXToView: (view: ExcalidrawView) => void;
export declare const search: (view: ExcalidrawView) => Promise<void>;
/**
 *
 * @param elements
 * @param query
 * @param exactMatch - when searching for section header exactMatch should be set to true
 * @returns the elements matching the query
 */
export declare const getTextElementsMatchingQuery: (elements: ExcalidrawElement[], query: string[], exactMatch?: boolean) => ExcalidrawElement[];
/**
 *
 * @param elements
 * @param query
 * @param exactMatch - when searching for section header exactMatch should be set to true
 * @returns the elements matching the query
 */
export declare const getFrameElementsMatchingQuery: (elements: ExcalidrawElement[], query: string[], exactMatch?: boolean) => ExcalidrawElement[];
export declare const cloneElement: (el: ExcalidrawElement) => any;
export declare const verifyMinimumPluginVersion: (requiredVersion: string) => boolean;
```


================================================
FILE: docs/zh-cn/docs/API/canvas_style.md
================================================
# [◀ Excalidraw 自动化指南](../readme.md)

## 画布样式设置
设置画布的属性。

### theme, setTheme()
字符串。有效值为 "light"（明亮）和 "dark"（黑暗）。

`setTheme()` 接受一个数字参数：
- 0："light"（明亮）
- 其他任何数字："dark"（黑暗）

### viewBackgroundColor
字符串。这是对象的填充颜色。[CSS 合法颜色值](https://www.w3schools.com/cssref/css_colors_legal.asp)

允许的值包括 [HTML 颜色名称](https://www.w3schools.com/colors/colors_names.asp)、十六进制 RGB 字符串（例如红色使用 `#FF0000`）或 `transparent`（透明）。

### gridSize
数字。网格的大小。如果设置为零，则不显示网格。



================================================
FILE: docs/zh-cn/docs/API/element_style.md
================================================
# [◀ Excalidraw 自动化指南](../readme.md)

## 元素样式设置

你会注意到，一些样式有setter函数。这是为了帮助你设置属性的允许值。但是你不必使用setter函数，也可以直接设置值。

### strokeColor

字符串类型。线条的颜色。[CSS合法颜色值](https://www.w3schools.com/cssref/css_colors_legal.asp)

允许的值包括[HTML颜色名称](https://www.w3schools.com/colors/colors_names.asp)、十六进制RGB字符串，例如红色为`#FF0000`。

### backgroundColor

字符串类型。这是对象的填充颜色。[CSS合法颜色值](https://www.w3schools.com/cssref/css_colors_legal.asp)

允许的值包括[HTML颜色名称](https://www.w3schools.com/colors/colors_names.asp)、十六进制RGB字符串，例如红色为`#FF0000`，或者`transparent`（透明）。

### angle

数字类型。以弧度为单位的旋转角度。90度等于`Math.PI/2`。

### fillStyle, setFillStyle()

```typescript
type FillStyle = "hachure" | "cross-hatch" | "solid";
setFillStyle (val:number);
```

fillStyle 是一个字符串。

`setFillStyle()` 接受一个数字参数：
- 0: "hachure"（斜线填充）
- 1: "cross-hatch"（交叉填充）
- 其他任意数字: "solid"（实心填充）

### strokeWidth

数字类型。设置线条的宽度。

### strokeStyle, setStrokeStyle()

```typescript
type StrokeStyle = "solid" | "dashed" | "dotted";
setStrokeStyle (val:number);
```

strokeStyle 是一个字符串。

`setStrokeStyle()` 接受一个数字参数：
- 0: "solid"（实线）
- 1: "dashed"（虚线）
- 其他任意数字: "dotted"（点线）

### roughness

数字类型。在 Excalidraw 中称为随意度。接受三个值：
- 0：建筑师风格
- 1：艺术家风格
- 2：卡通家风格

### opacity

数字类型，取值范围在 0~100 之间。用于设置对象的不透明度，同时影响线条和填充的透明度。

### strokeSharpness, setStrokeSharpness()

```typescript
type StrokeSharpness = "round" | "sharp";
setStrokeSharpness(val:number);
```

strokeSharpness 是一个字符串。

"round"（圆滑）线条是弯曲的，"sharp"（尖锐）线条在转折点处会形成尖角。

`setStrokeSharpness()` 接受一个数字参数：
- 0："round"（圆滑）
- 其他任意数字："sharp"（尖锐）

### fontFamily, setFontFamily()

数字类型。有效值为 1、2 和 3。

`setFontFamily()` 也接受一个数字参数并返回字体名称：
- 1: "Virgil, Segoe UI Emoji"
- 2: "Helvetica, Segoe UI Emoji"
- 3: "Cascadia, Segoe UI Emoji"

### fontSize

数字类型。默认值为 20px。

### textAlign

字符串类型。文本的水平对齐方式。有效值为 "left"（左对齐）、"center"（居中对齐）、"right"（右对齐）。

这在使用 `addText()` 函数设置固定宽度时很有用。

### verticalAlign

字符串类型。文本的垂直对齐方式。有效值为 "top"（顶部对齐）和 "middle"（居中对齐）。

这在使用 `addText()` 函数设置固定高度时很有用。

### startArrowHead, endArrowHead

字符串类型。有效值为 "arrow"（箭头）、"bar"（线段）、"dot"（圆点）和 "none"（无）。用于指定箭头的起始和结束样式。

这在使用 `addArrow()` 和 `connectObjects()` 函数时很有用。



================================================
FILE: docs/zh-cn/docs/API/introduction.md
================================================
[Binary file]


================================================
FILE: docs/zh-cn/docs/API/objects.md
================================================
# [◀ Excalidraw 自动化使用指南](../readme.md)

## 添加对象

这些函数将向你的绘图中添加对象。画布是无限的，可以接受负数和正数的 X 和 Y 值。X 值从左到右递增，Y 值从上到下递增。

![坐标系](https://user-images.githubusercontent.com/14358394/116825632-6569b980-ab90-11eb-827b-ada598e91e46.png)

### addRect(), addDiamond(), addEllipse()

```typescript
addRect(topX:number, topY:number, width:number, height:number):string
addDiamond(topX:number, topY:number, width:number, height:number):string
addEllipse(topX:number, topY:number, width:number, height:number):string
```

返回对象的 `id`。当使用线条连接对象时需要用到这个 `id`，详见后文。

### addText()

```typescript
addText( 
  topX:number, 
  topY:number, 
  text:string, 
  formatting?:{
    wrapAt?:number, 
    width?:number, 
    height?:number,
    textAlign?:string, 
    box?: "box"|"blob"|"ellipse"|"diamond", 
    boxPadding?:number
  },
  id?:string
):string
```

向绘图中添加文本。

格式化参数是可选的：
- 如果未指定 `width` 和 `height`，函数将根据字体系列（fontFamily）、字体大小（fontSize）和提供的文本来计算宽度和高度。
- 如果你想要将文本相对于绘图中的其他元素居中对齐，你可以提供固定的高度和宽度，并且可以像上面描述的那样指定 `textAlign` 和 `verticalAlign`。例如：`{width:500, textAlign:"center"}`
- 如果你想在文本周围添加一个框，设置 `{box:"box"|"blob"|"ellipse"|"diamond"}`（分别对应矩形框、气泡框、椭圆框、菱形框）

返回对象的 `id`。当使用线条连接对象时需要用到这个 `id`，详见后文。如果设置了 `{box:}`，则返回包围框对象的 id。

### addLine()

```typescript
addLine(points: [[x:number,y:number]]):string
```

根据提供的点添加一条线。必须包含至少两个点 `points.length >= 2`。如果提供了超过 2 个点，中间点将被添加为断点。当 `strokeSharpness` 设置为 "sharp" 时，线条会以角度方式折断；设置为 "round" 时，线条会呈现曲线。

返回对象的 `id`。

### addArrow()

```typescript
addArrow(points: [[x:number,y:number]],formatting?:{startArrowHead?:string,endArrowHead?:string,startObjectId?:string,endObjectId?:string}):string ;
```

根据提供的点添加一个箭头。必须包含至少两个点 `points.length >= 2`。如果提供了超过 2 个点，中间点将被添加为断点。当元素的 `style.strokeSharpness` 设置为 "sharp" 时，线条会以角度方式折断；设置为 "round" 时，线条会呈现曲线。

`startArrowHead` 和 `endArrowHead` 指定要使用的箭头类型，如上所述。有效值包括 "none"（无）、"arrow"（箭头）、"dot"（圆点）和 "bar"（线条）。例如：`{startArrowHead: "dot", endArrowHead: "arrow"}`

`startObjectId` 和 `endObjectId` 是连接对象的 ID。如果是为了连接对象，建议使用 `connectObjects` 而不是调用 addArrow()。

返回对象的 `id`。

### connectObjects()

```typescript
declare type ConnectionPoint = "top"|"bottom"|"left"|"right";
connectObjects(objectA: string, connectionA: ConnectionPoint, objectB: string, connectionB: ConnectionPoint, formatting?:{numberOfPoints: number,startArrowHead:string,endArrowHead:string, padding: number}):void
```

使用箭头连接两个对象。如果两个元素中的任何一个是 `line`（线条）、`arrow`（箭头）或 `freedraw`（自由绘制）类型，则不会执行任何操作。

`objectA` 和 `objectB` 是字符串类型，表示要连接的对象的 ID。这些 ID 是在创建对象时由 addRect()、addDiamond()、addEllipse() 和 addText() 函数返回的。

`connectionA` 和 `connectionB` 指定在对象上的连接位置。有效值包括："top"（顶部）、"bottom"（底部）、"left"（左侧）和 "right"（右侧）。

`numberOfPoints` 设置线条的中间断点数量。默认值为零，表示箭头的起点和终点之间没有断点。当在绘图上移动对象时，这些断点会影响 Excalidraw 重新路由线条的方式。

`startArrowHead` 和 `endArrowHead` 的工作方式如上文 `addArrow()` 中所述。

### addToGroup()

```typescript
addToGroup(objectIds:[]):string
```

将 `objectIds` 中列出的对象组合成一个组。返回该组的 `id`。


================================================
FILE: docs/zh-cn/docs/API/utility.md
================================================
# [◀ Excalidraw Automate How To](../readme.md)

## 实用工具函数

### isExcalidrawFile()
```typescript
isExcalidrawFile(f:TFile): boolean
```
如果提供的文件是有效的 Excalidraw 文件（可以是传统的 `*.excalidraw` 文件或在 front-matter 中包含 excalidraw 键的 markdown 文件），则返回 true。

### clear()
`clear()` 将清除缓存中的对象，但会保留元素样式设置。

### reset()
`reset()` 会先调用 `clear()`，然后将元素样式重置为默认值。

### toClipboard()
```typescript
async toClipboard(templatePath?:string)
```
将生成的绘图放置到剪贴板中。当你不想创建新的绘图，而是想将额外的元素粘贴到现有绘图上时，这个功能很有用。

### getElements()
```typescript
getElements():ExcalidrawElement[];
```
以数组形式返回 ExcalidrawAutomate 中的 ExcalidrawElement 元素。这种格式在使用 ExcalidrawRef 时特别有用。

### getElement()
```typescript
getElement(id:string):ExcalidrawElement;
```
返回与指定 id 匹配的元素对象。如果元素不存在，则返回 null。

### create()
```typescript
async create(params?:{filename: string, foldername:string, templatePath:string, onNewPane: boolean})
```
创建并打开绘图。返回创建文件的完整路径。

`filename` 是要创建的绘图文件名（不包含扩展名）。如果为 `null`，Excalidraw 将自动生成文件名。

`foldername` 是文件创建的目标文件夹。如果为 `null`，则会根据 Excalidraw 设置使用默认的新建绘图文件夹。

`templatePath` 是模板文件的完整路径（包含文件名和扩展名）。该模板文件将作为基础图层，所有通过 ExcalidrawAutomate 添加的对象都会显示在模板元素的上层。如果为 `null`，则不使用模板，即使用空白画布作为添加对象的基础。

`onNewPane` 定义新绘图的创建位置。`false` 将在当前活动页签中打开绘图。`true` 将通过垂直分割当前页签来打开绘图。

`frontmatterKeys` 是要应用到文档的 frontmatter 键值集合
  {
    excalidraw-plugin?: "raw"|"parsed",
    excalidraw-link-prefix?: string,
    excalidraw-link-brackets?: boolean,
    excalidraw-url-prefix?: string
  }

示例：
```javascript
create (
  {
    filename:"my drawing", 
    foldername:"myfolder/subfolder/", 
    templatePath: "Excalidraw/template.excalidraw", 
    onNewPane: true, 
    frontmatterKeys: {
      "excalidraw-plugin": "parsed",
      "excalidraw-link-prefix": "",
      "excalidraw-link-brackets": true,
      "excalidraw-url-prefix": "🌐",
    }
  }
);
```

### createSVG()
```typescript
async createSVG(templatePath?:string)
```
返回包含生成绘图的 HTML SVGSVGElement 元素。

### createPNG()
```typescript
async createPNG(templatePath?:string, scale:number=1)
```
返回包含生成绘图的 PNG 图像 blob 对象。

### wrapText()
```typescript
wrapText(text:string, lineLen:number):string
```
返回一个按照指定最大行长度换行的字符串。

### 访问打开的 Excalidraw 视图
在使用任何视图操作函数之前，你需要先初始化 targetView。

#### targetView
```typescript
targetView: ExcalidrawView
```
已打开的 Excalidraw 视图，被配置为视图操作的目标。使用 `setView` 进行初始化。

#### setView()
```typescript
setView(view:ExcalidrawView|"first"|"active"):ExcalidrawView
```
设置将作为视图操作目标的 ExcalidrawView。有效的 `view` 输入值包括：
- ExcalidrawView 的对象实例
- "first"：如果打开了多个 Excalidraw 视图，则选择 `app.workspace.getLeavesOfType("Excalidraw")` 返回的第一个视图
- "active"：表示当前活动的视图

#### getExcalidrawAPI()
```typescript
getExcalidrawAPI():any
```
返回在 `targetView` 中指定的当前活动绘图的原生 Excalidraw API（ref.current）。
查看 Excalidraw 文档请访问：https://www.npmjs.com/package/@excalidraw/excalidraw#ref

#### getViewElements()
```typescript
getViewElements():ExcalidrawElement[] 
```
返回视图中的所有元素。

#### deleteViewElements()
```typescript
deleteViewElements(elToDelete: ExcalidrawElement[]):boolean 
```
从视图中删除与输入参数中提供的元素相匹配的元素。

示例：从视图中删除选中的元素：
```typescript
ea = ExcalidrawAutomate;
ea.setView("active");
el = ea.getViewSelectedElements();
ea.deleteViewElements();
```

#### getViewSelectedElement()
```typescript
getViewSelectedElement():ExcalidrawElement
```
首先需要调用 `setView()` 来设置视图。

如果在目标视图 (targetView) 中选中了一个元素，该函数将返回被选中的元素。如果选中了多个元素（通过 <kbd>SHIFT+点击</kbd> 选择多个元素，或者选择一个组），将返回第一个元素。如果你想从一个组中指定要选择的元素，请双击该组中想要的元素。

当你想要添加一个与绘图中现有元素相关的新元素时，这个函数会很有帮助。

#### getViewSelectedElements()
```typescript
getViewSelectedElements():ExcalidrawElement[]
```
首先需要调用 `setView()` 来设置视图。

获取场景中选中元素的数组。如果没有选中任何元素，则返回 []。

注意：你可以调用 `getExcalidrawAPI().getSceneElements()` 来获取场景中的所有元素。

#### viewToggleFullScreen()
```typescript
viewToggleFullScreen(forceViewMode?:boolean):void;
```
在目标视图 (targetView) 中切换全屏模式和普通模式。通过将 forceViewMode 设置为 `true` 可以将 Excalidraw 切换到查看模式。默认值为 `false`。

此功能在 Obsidian 移动端上不生效。

#### connectObjectWithViewSelectedElement()
```typescript 
connectObjectWithViewSelectedElement(objectA:string,connectionA: ConnectionPoint, connectionB: ConnectionPoint, formatting?:{numberOfPoints?: number,startArrowHead?:string,endArrowHead?:string, padding?: number}):boolean
```
与 `connectObjects()` 功能相同，但 ObjectB 是目标 ExcalidrawView 中当前选中的元素。该函数有助于在新创建的对象和目标 ExcalidrawView 中选中的元素之间放置一个箭头。

#### addElementsToView()
```typescript
async addElementsToView(repositionToCursor:boolean=false, save:boolean=false):Promise<boolean>
```
将使用 ExcalidrawAutomate 创建的元素添加到目标 ExcalidrawView 中。

`repositionToCursor` 默认值为 false
- true：元素将被移动，使其中心点与 ExcalidrawView 上当前指针的位置对齐。你可以使用此开关将元素指向并放置到绘图中的所需位置。
- false：元素将按照每个元素的 x&y 坐标定义的位置进行放置。

`save` 默认值为 false
- true：元素添加后绘图将被保存。
- false：绘图将在下一个自动保存周期时保存。当连续添加多个元素时使用 false。否则，最好使用 true 以最小化数据丢失的风险。

### onDropHook
```typescript
onDropHook (data: {
  ea: ExcalidrawAutomate, 
  event: React.DragEvent<HTMLDivElement>,
  draggable: any, //Obsidian draggable object
  type: "file"|"text"|"unknown",
  payload: {
    files: TFile[], //TFile[] array of dropped files
    text: string, //string 
  },
  excalidrawFile: TFile, //the file receiving the drop event
  view: ExcalidrawView, //the excalidraw view receiving the drop
  pointerPosition: {x:number, y:number} //the pointer position on canvas at the time of drop
}):boolean;
```
当可拖拽项被拖放到 Excalidraw 上时触发的回调函数。

该函数应返回一个布尔值。如果拖放由钩子函数处理且应停止进一步的原生处理，则返回 true；如果应让 Excalidraw 继续处理拖放操作，则返回 false。

拖放类型可以是以下之一：
- "file"：当从 Obsidian 文件浏览器中拖放文件到 Excalidraw 时。在这种情况下，payload.files 将包含被拖放文件的列表。
- "text"：当拖放链接（如 URL 或 wiki 链接）或其他文本时。在这种情况下，payload.text 将包含接收到的字符串。
- "unknown"：当 Excalidraw 插件无法识别拖放对象的类型时。在这种情况下，你可以使用 React.DragEvent 来分析拖放的对象。

使用 Templater 启动模板或类似方法来设置钩子函数。

```typescript
ea = ExcalidrawAutomate;
ea.onDropHook = (data) => {
  console.log(data); 
  return false;
}
```



================================================
FILE: docs/zh-cn/docs/Examples/apply_template.md
================================================
# [◀ Excalidraw 自动化使用指南](../readme.md)

## 将 Excalidraw 模板应用到新绘图

这个示例与介绍中的类似，只是将图形旋转了90度，并且使用了模板，同时指定了保存绘图的文件名和文件夹，还会在新窗格中打开这个新绘图。

*使用 <kbd>CTRL+Shift+V</kbd> 将代码粘贴到 Obsidian 中！*

```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.style.angle = Math.PI/2; 
  ea.style.strokeWidth = 3.5;
  ea.addRect(-150,-50,450,300);
  ea.addText(-100,70,"Left to right");
  ea.addArrow([[-100,100],[100,100]]);

  ea.style.strokeColor = "red";
  await ea.addText(100,-30,"top to bottom",{width:200,textAlign:"center"});
  ea.addArrow([[200,0],[200,200]]);
  await ea.create({
    filename    :"My Drawing",
    foldername  :"myfolder/fordemo/",
    templatePath:"Excalidraw/Template2.excalidraw",
    onNewPane   :true});
%>
```


================================================
FILE: docs/zh-cn/docs/Examples/connect_objects.md
================================================
# [◀ Excalidraw Automate 使用指南](../readme.md)

## 连接对象

这个 [Templater](https://github.com/SilentVoid13/Templater) 模板演示了如何使用 ExcalidrawAutomate 连接两个对象。

*使用 <kbd>CTRL+Shift+V</kbd> 将代码粘贴到 Obsidian 中！*

```javascript
<%*
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.addText(-130,-100,"Connecting two objects");
  const a = ea.addRect(-100,-100,100,100);
  const b = ea.addEllipse(200,200,100,100);
  ea.connectObjects(a,"bottom",b,"left",{numberOfPoints: 2}); //see how the line breaks differently when moving objects around
  ea.style.strokeColor = "red";
  ea.connectObjects(a,"right",b,"top",1);
  await ea.create();
%>
```



================================================
FILE: docs/zh-cn/docs/Examples/dataviewjs_familytree.md
================================================
# [◀ Excalidraw Automate 使用指南](../readme.md)

## 使用 dataviewjs 生成家谱树

这个示例与使用 dataviewjs 生成思维导图的脚本类似，但输出结果是垂直呈现的。

### 输出效果

![image](https://user-images.githubusercontent.com/14358394/117549637-d3ecc280-b03b-11eb-952a-840a9a75b6ca.png)

### 输入文件

任务列表格式如下：

```markdown
- [ ] OBSIDIAN
    - [ ] Silver
        - [ ] PawPaw Silv
        - [ ] MawMaw Silv
    - [ ] Licat
        - [ ] PeePaw Li
        - [ ] MeeMaw Li
```

### dataviewjs 脚本

渲染 Excalidraw 图形的代码如下：

```javascript
function crawl(subtasks) {
  let size = subtasks.length > 0 ? 0 : 1; //if no children then a leaf with size 1
  for (let task of subtasks) {
    task["size"] = crawl(task.subtasks);
    size += task.size;
  }
  return size;
}

const tasks = dv.page("FamilyTree.md").file.tasks[0];
tasks["size"] = crawl(tasks.subtasks);

const width = 300;
const height = 150;
const ea = ExcalidrawAutomate;
ea.reset();

function buildMindmap(subtasks, depth, offset, parentObjectID) {
  if (subtasks.length == 0) return;
  let task;
  
  for (let i = 0; i < subtasks.length; i++) {
  task = subtasks[i]
  if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
    task["objectID"] = ea.addText((task.size/2+offset)*width,depth*height,task.text,{box:true})
    ea.connectObjects(parentObjectID,"top",task.objectID,"bottom",{startArrowHead: 'arrow', endArrowHead: 'dot'});
    if (i >= 1) {
            ea.connectObjects(subtasks[i-1]['objectID'],"right",task.objectID,"left", {endArrowHead: 'none'});
    }

    buildMindmap(task.subtasks, depth-1,offset,task.objectID);
    offset += task.size/1.5;
  }
 
}

tasks["objectID"] = ea.addText(width*1.5,height*(tasks.size-1),tasks.text,{box:true, textAlign:"center"});
buildMindmap(tasks.subtasks, 2, 0, tasks.objectID);

ea.createSVG().then((svg)=>dv.span(svg.outerHTML));
```


================================================
FILE: docs/zh-cn/docs/Examples/dataviewjs_mindmap.md
================================================
# [◀ Excalidraw Automate 使用指南](../readme.md)

## 使用 dataviewjs 从任务列表生成思维导图

这个方法与使用 templater 生成思维导图的脚本类似，但由于 dataview 已经以树形结构返回任务，所以实现起来稍微简单一些

### 输出效果

![image](https://user-images.githubusercontent.com/14358394/117548665-71dd8e80-b036-11eb-8a45-4169fdd7cc05.png)

### 输入文件

输入文件是 `Demo.md`，其内容如下：

```markdown
- [ ] Root task
    - [ ] task 1.1
    - [ ] task 1.2
        - [ ] task 1.2.1
        - [ ] task 1.2.2
    - [ ] task 1.3
        - [ ] task 1.3.1
```

### dataviewjs 脚本

`dataviewjs` 脚本如下所示：

*使用 <kbd>CTRL+Shift+V</kbd> 将代码粘贴到 Obsidian 中！*

```javascript
function crawl(subtasks) {
  let size = subtasks.length > 0 ? 0 : 1; //if no children then a leaf with size 1
  for (let task of subtasks) {
    task["size"] = crawl(task.subtasks);
    size += task.size;
  }
  return size;
}

const tasks = dv.page("Demo.md").file.tasks[0];
tasks["size"] = crawl(tasks.subtasks);

const width = 300;
const height = 100;
const ea = ExcalidrawAutomate;
ea.reset();

function buildMindmap(subtasks, depth, offset, parentObjectID) {
  if (subtasks.length == 0) return;
  for (let task of subtasks) {
    if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
    task["objectID"] = ea.addText(depth*width,(task.size/2+offset)*height,task.text,{box:true})
    ea.connectObjects(parentObjectID,"right",task.objectID,"left",{startArrowHead: 'dot'});
    buildMindmap(task.subtasks, depth+1,offset,task.objectID);
    offset += task.size;
  }
}

tasks["objectID"] = ea.addText(0,(tasks.size/2)*height,tasks.text,{box:true});    
buildMindmap(tasks.subtasks, 1, 0, tasks.objectID);

ea.createSVG().then((svg)=>dv.span(svg.outerHTML));
```


================================================
FILE: docs/zh-cn/docs/Examples/insert_new_drawing.md
================================================
# [◀ Excalidraw 自动化使用指南](../readme.md)

## 在当前编辑的文档中插入新绘图

这个 [Templater](https://github.com/SilentVoid13/Templater) 模板会提示你输入绘图的标题。它将使用提供的标题创建一个新的绘图，并将其保存在你正在编辑的文档所在的文件夹中。然后，它会在光标位置嵌入新绘图，并通过拆分当前页面的方式在新的工作区中打开这个绘图。

*使用 <kbd>CTRL+Shift+V</kbd> 将代码粘贴到 Obsidian 中！*

```javascript
<%*
  const defaultTitle = tp.date.now("HHmm")+' '+tp.file.title;
  const title = await tp.system.prompt("Title of the drawing?", defaultTitle);
  const folder = tp.file.folder(true);
  const transcludePath = (folder== '/' ? '' : folder + '/') + title + '.excalidraw';
  tR = '![['+transcludePath+']]';
  const ea = ExcalidrawAutomate;
  ea.reset();
  ea.setTheme(1); //set Theme to dark
  await ea.create({
    filename : title,
    foldername : folder,
    //templatePath: 'Excalidraw/Template.excalidraw', //uncomment if you want to use a template
    onNewPane : true
  });
%>
```


================================================
FILE: docs/zh-cn/docs/Examples/templater_mindmap.md
================================================
# [◀ Excalidraw Automate 使用指南](../readme.md)

## 从文本大纲生成简单思维导图

这是一个稍微复杂一点的示例。它将从制表符缩进的大纲生成思维导图。

### 输出效果

![Drawing 2021-05-05 20 52 34](https://user-images.githubusercontent.com/14358394/117194124-00a69d00-ade4-11eb-8b75-5e18a9cbc3cd.png)

### 输入文件

示例输入：
```
- Test 1
	- Test 1.1
- Test 2
	- Test 2.1
	- Test 2.2 
		- Test 2.2.1
		- Test 2.2.2
		- Test 2.2.3
			- Test 2.2.3.1
- Test 3
	- Test 3.1
```

### Templater 脚本

*使用 <kbd>CTRL+Shift+V</kbd> 将代码粘贴到 Obsidian 中！*

```javascript
<%*
const IDX = Object.freeze({"depth":0, "text":1, "parent":2, "size":3, "children": 4, "objectId":5});

//check if an editor is the active view
const editor = this.app.workspace.activeLeaf?.view?.editor;
if(!editor) return;

//initialize the tree with the title of the document as the first element
let tree = [[0,this.app.workspace.activeLeaf?.view?.getDisplayText(),-1,0,[],0]];
const linecount = editor.lineCount();

//helper function, use regex to calculate indentation depth, and to get line text
function getLineProps (i) {
  props = editor.getLine(i).match(/^(\t*)-\s+(.*)/);
  return [props[1].length+1, props[2]];
}

//a vector that will hold last valid parent for each depth
let parents = [0];

//load outline into tree
for(i=0;i<linecount;i++) {
  [depth,text] = getLineProps(i);
  if(depth>parents.length) parents.push(i+1);
  else parents[depth] = i+1;
  tree.push([depth,text,parents[depth-1],1,[]]);
  tree[parents[depth-1]][IDX.children].push(i+1);
}

//recursive function to crawl the tree and identify height aka. size of each node
function crawlTree(i) {
  if(i>linecount) return 0;
  size = 0;
  if((i+1<=linecount && tree[i+1][IDX.depth] <= tree[i][IDX.depth])|| i == linecount) { //I am a leaf
    tree[i][IDX.size] = 1; 
    return 1; 
  }
  tree[i][IDX.children].forEach((node)=>{ 
    size += crawlTree(node);
  });
  tree[i][IDX.size] = size; 
  return size;   
}

crawlTree(0);

//Build the mindmap in Excalidraw
const width = 300;
const height = 100;
const ea = ExcalidrawAutomate;
ea.reset();

//stores position offset of branch/leaf in height units
offsets = [0];

for(i=0;i<=linecount;i++) {
  depth = tree[i][IDX.depth];
  if (depth == 1) ea.style.strokeColor = '#'+(Math.random()*0xFFFFFF<<0).toString(16).padStart(6,"0");
  tree[i][IDX.objectId] = ea.addText(depth*width,((tree[i][IDX.size]/2)+offsets[depth])*height,tree[i][IDX.text],{box:true});  
  //set child offset equal to parent offset
  if((depth+1)>offsets.length) offsets.push(offsets[depth]);
  else offsets[depth+1] = offsets[depth];
  offsets[depth] += tree[i][IDX.size];
  if(tree[i][IDX.parent]!=-1) {
    ea.connectObjects(tree[tree[i][IDX.parent]][IDX.objectId],"right",tree[i][IDX.objectId],"left",{startArrowHead: 'dot'});
  }
}

await ea.create({onNewPane: true});
%>
```



================================================
FILE: docs/zh-cn/ea-scripts/README.md
================================================
[Binary file]


================================================
FILE: ea-scripts/README.md
================================================
# Excalidraw Script Engine scripts library

【English | [简体中文](../docs/zh-cn/ea-scripts/README.md)】

Click to watch the intro video:

[![Script Engine](https://user-images.githubusercontent.com/14358394/145684531-8d9c2992-59ac-4ebc-804a-4cce1777ded2.jpg)](https://youtu.be/hePJcObHIso)

> **Warning**
> There is an easier way to install/manage scripts than what is shown in this video

See the [Excalidraw Script Engine](https://zsviczian.github.io/obsidian-excalidraw-plugin/ExcalidrawScriptsEngine.html) documentation for more details.

## How to install scripts into your Obsidian Vault
To install one of the built-in scripts:
- Open up an excalidraw drawing in Obsidian
- In the pane dropdown menu select "Install or update Excalidraw Scripts"
- Click on one of the available scripts
- Click on "Install this script" (note if the script is already installed you will instead see an option to update it)
- Restart Obsidian so the script will be picked up

Note: By default this will install the script into your vault in the `Excalidraw/Scripts/Downloaded` folder

<details><summary>Manual installation of scripts</summary>

Open the script you are interested in and save it to your Obsidian Vault including the first line `/*`, or open it in "Raw" and copy the entire contents to Obsidian.

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-download-raw.jpg)

</details>

## List of available scripts
|Title|Description|Icon|Contributor|
|----|----|----|----|
|[Add Connector Point](Add%20Connector%20Point.md)|This script will add a small circle to the top left of each text element in the selection and add the text and the "bullet point" into a group.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-bullet-point.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Add Link to Existing File and Open](Add%20Link%20to%20Existing%20File%20and%20Open.md)|Prompts for a file from the vault. Adds a link to the selected element pointing to the selected file. You can control in settings to open the file in the current active pane or an adjacent pane.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-link-and-open.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Add Link to New Page and Open](Add%20Link%20and%20Open%20Page.md)|Prompts for filename. Offers option to create and open a new Markdown or Excalidraw document. Adds link pointing to the new file, to the selected objects in the drawing. You can control in settings to open the file in the current active pane or an adjacent pane.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-link-to-new-page-and-pen.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Add Next Step in Process](Add%20Link%20to%20New%20Page%20and%20Open.md)|This script will prompt you for the title of the process step, then will create a stick note with the text. If an element is selected then the script will connect this new step with an arrow to the previous step (the selected element). If no element is selected, then the script assumes this is the first step in the process and will only output the sticky note with the text that was entered.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-process-step.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Split Ellipse](Boolean%20Operations.md)|With This Script it is possible to make boolean Operations on Shapes.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-boolean-operations-showcase.png)|[@GColoy](https://github.com/GColoy)|
|[Box Each Selected Groups](Box%20Each%20Selected%20Groups.md)|This script will add encapsulating boxes around each of the currently selected groups in Excalidraw.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-box-each-selected-groups.png)|[@1-2-3](https://github.com/1-2-3)|
|[Box Selected Elements](Box%20Selected%20Elements.md)|This script will add an encapsulating box around the currently selected elements in Excalidraw.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-box-elements.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Change shape of selected elements](Change%20shape%20of%20selected%20elements.md)|The script allows you to change the shape of selected Rectangles, Diamonds and Ellipses|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-change-shape.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Connect elements](Connect%20elements.md)|This script will connect two objects with an arrow. If either of the objects are a set of grouped elements (e.g. a text element grouped with an encapsulating rectangle), the script will identify these groups, and connect the arrow to the largest object in the group (assuming you want to connect the arrow to the box around the text element).|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-connect-elements.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Convert freedraw to line](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/ea-scripts/Convert%20freedraw%20to%20line.md)|Convert selected freedraw objects into editable lines. This will allow you to adjust your drawings by dragging line points and will also allow you to select shape fill in case of enclosed lines. You can adjust conversion point density in settings|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-convert-freedraw-to-line.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Convert selected text elements to sticky notes](Convert%20selected%20text%20elements%20to%20sticky%20notes.md)|Converts selected plain text elements to sticky notes with transparent background and transparent stroke color. Essentially converts text element into a wrappable format.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-textelement-to-transparent-stickynote.png)|[@zsviczian](https://github.com/zsviczian)|
|[Convert text to link with folder and alias](Convert%20text%20to%20link%20with%20folder%20and%20alias.md)|Converts text elements to links pointing to a file in a selected folder and with the alias set as the original text. The script will prompt the user to select an existing folder from the vault.|`original text` => `[[selected folder/original text\|original text]]`|[@zsviczian](https://github.com/zsviczian)|
|[Copy Selected Element Styles to Global](Copy%20Selected%20Element%20Styles%20to%20Global)|This script will copy styles of any selected element into Excalidraw's global styles.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-copy-selected-element-styles-to-global.png)|[@1-2-3](https://github.com/1-2-3)|
|[Create new markdown file and embed into active drawing](Create%20new%20markdown%20file%20and%20embed%20into%20active%20drawing.md)|The script will prompt you for a filename, then create a new markdown document with the file name provided, open the new markdown document in an adjacent pane, and embed the markdown document into the active Excalidraw drawing.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-create-and-embed-new-markdown-file.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Darken background color](Darken%20background%20color.md)|This script darkens the background color of the selected element by 2% at a time. You can use this script several times until you are satisfied. It is recommended to set a shortcut key for this script so that you can quickly try to DARKEN and LIGHTEN the color effect. In contrast to the `Modify background color opacity` script, the advantage is that the background color of the element is not affected by the canvas color, and the color value does not appear in a strange rgba() form.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/darken-lighten-background-color.png)|[@1-2-3](https://github.com/1-2-3)|
|[Elbow connectors](Elbow%20connectors.md)|This script converts the selected connectors to elbows.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/elbow-connectors.png)|[@1-2-3](https://github.com/1-2-3)|
|[Expand rectangles horizontally keep text centered](Expand%20rectangles%20horizontally%20keep%20text20%centered.md)|This script expands the width of the selected rectangles until they are all the same width and keep the text centered.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-expand-rectangles.gif)|[@1-2-3](https://github.com/1-2-3)|
|[Expand rectangles horizontally](Expand%20rectangles%20horizontally.md)|This script expands the width of the selected rectangles until they are all the same width.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-expand-rectangles.gif)|[@1-2-3](https://github.com/1-2-3)|
|[Expand rectangles vertically keep text centered](Expand%20rectangles%20vertically%20keep%20text%20centered.md)|This script expands the height of the selected rectangles until they are all the same height and keep the text centered.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-expand-rectangles.gif)|[@1-2-3](https://github.com/1-2-3)|
|[Expand rectangles vertically](Expand%20rectangles%20vertically.md)|This script expands the height of the selected rectangles until they are all the same height.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-expand-rectangles.gif)|[@1-2-3](https://github.com/1-2-3)|
|[Fixed horizontal distance between centers](Fixed%20horizontal%20distance%20between%20centers.md)|This script arranges the selected elements horizontally with a fixed center spacing.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-fixed-horizontal-distance-between-centers.png)|[@1-2-3](https://github.com/1-2-3)|
|[Fixed inner distance](Fixed%20inner%20distance.md)|This script arranges selected elements and groups with a fixed inner distance.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-fixed-inner-distance.png)|[@1-2-3](https://github.com/1-2-3)|
|[Fixed spacing](Fixed%20spacing.md)|The script arranges the selected elements horizontally with a fixed spacing. When we create an architecture diagram or mind map, we often need to arrange a large number of elements in a fixed spacing. `Fixed spacing` and `Fixed vertical Distance` scripts can save us a lot of time.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-fix-space-demo.png)|[@1-2-3](https://github.com/1-2-3)|
|[Fixed vertical distance between centers](Fixed%20vertical%20distance%20between%20centers.md)|This script arranges the selected elements vertically with a fixed center spacing.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-fixed-vertical-distance-between-centers.png)|[@1-2-3](https://github.com/1-2-3)|
|[Fixed vertical distance](Fixed%20vertical%20distance.md)|The script arranges the selected elements vertically with a fixed spacing. When we create an architecture diagram or mind map, we often need to arrange a large number of elements in a fixed spacing. `Fixed spacing` and `Fixed vertical Distance` scripts can save us a lot of time.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-fixed-vertical-distance.png)|[@1-2-3](https://github.com/1-2-3)|
|[Lighten background color](Lighten%20background%20color.md)|This script lightens the background color of the selected element by 2% at a time. You can use this script several times until you are satisfied. It is recommended to set a shortcut key for this script so that you can quickly try to DARKEN and LIGHTEN the color effect.In contrast to the `Modify background color opacity` script, the advantage is that the background color of the element is not affected by the canvas color, and the color value does not appear in a strange rgba() form.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/darken-lighten-background-color.png)|[@1-2-3](https://github.com/1-2-3)|
|[Mindmap connector](Mindmap%20connector.md)|This script creates mindmap like lines (only right side and down available currently) for selected elements. The line will start according to the creation time of the elements. So you should create the header element first.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/mindmap%20connector.png)|[@xllowl](https://github.com/xllowl)|
|[Modify background color opacity](Modify%20background%20color%20opacity.md)|This script changes the opacity of the background color of the selected boxes. The default background color in Excalidraw is so dark that the text is hard to read. You can lighten the color a bit by setting transparency. And you can tweak the transparency over and over again until you're happy with it. Although excalidraw has the opacity option in its native property Settings, it also changes the transparency of the border. Use this script to change only the opacity of the background color without affecting the border.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-modify-background-color-opacity.png)|[@1-2-3](https://github.com/1-2-3)|
|[Normalize Selected Arrows](Normalize%20Selected%20Arrows.md)|This script will reset the start and end positions of the selected arrows. The arrow will point to the center of the connected box and will have a gap of 8px from the box.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-normalize-selected-arrows.png)|[@1-2-3](https://github.com/1-2-3)|
|[OCR - Optical Character Recognition](OCR%20-%20Optical%20Character%20Recognition.md)|The script will  1) send the selected image file to [taskbone.com](https://taskbone.com) to extract the text from the image, and 2) will add the text to your drawing as a text element.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-ocr.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Organic Line](Organic%20Line.md)|Converts selected freedraw lines such that pencil pressure will decrease from maximum to minimum from the beginning of the line to its end. The resulting line is placed at the back of the layers, under all other items. Helpful when drawing organic mindmaps.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-organic-line.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Repeat Elements](Repeat%20Elements.md)|This script will detect the difference between 2 selected elements, including position, size, angle, stroke and background color, and create several elements that repeat these differences based on the number of repetitions entered by the user.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-repeat-elements.png)|[@1-2-3](https://github.com/1-2-3)|
|[Reset LaTeX Size](Reset%20LaTeX%20Size.md)|Reset the sizes of embedded LaTeX equations to the default sizes or a multiple of the default sizes.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-reset-latex.jpg)|[@firai](https://github.com/firai)|
|[Reverse arrows](Reverse%20arrows.md)|Reverse the direction of **arrows** within the scope of selected elements.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-reverse-arrow.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Scribble Helper](Scribble%20Helper.md)|iOS scribble helper for better handwriting experience with text elements. If no elements are selected then the creates a text element at pointer position and you can use the edit box to modify the text with scribble. If a text element is selected then opens the input prompt where you can modify this text with scribble.|![]('https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-scribble-helper.jpg')|[@zsviczian](https://github.com/zsviczian)|
|[Select Elements of Type](Select%20Elements%20of%20Type.md)|Prompts you with a list of the different element types in the active image. Only elements of the selected type will be selected on the canvas. If nothing is selected when running the script, then the script will process all the elements on the canvas. If some elements are selected when the script is executed, then the script will only process the selected elements.<br>The script is useful when, for example, you want to bring to front all the arrows, or want to change the color of all the text elements, etc.|![]('https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-select-element-of-type.jpg')|[@zsviczian](https://github.com/zsviczian)|
|[Set background color of unclosed line object by adding a shadow clone](Set%20background%20color%20of%20unclosed%20line%20object%20by%20adding%20a%20shadow%20clone.md)|Use this script to set the background color of unclosed (i.e. open) line objects by creating a clone of the object. The script will set the stroke color of the clone to transparent and will add a straight line to close the object. Use settings to define the default background color, the fill style, and the strokeWidth of the clone. By default the clone will be grouped with the original object, you can disable this also in settings.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-dimensions.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set Dimensions](Set%20Dimensions.md)|Currently there is no way to specify the exact location and size of objects in Excalidraw. You can bridge this gap with the following simple script.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-dimensions.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set Font Family](Set%20Font%20Family.md)|Sets font family of the text block (Virgil, Helvetica, Cascadia). Useful if you want to set a keyboard shortcut for selecting font family.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-font-family.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set Grid](Set%20Grid.md)|The default grid size in Excalidraw is 20. Currently there is no way to change the grid size via the user interface. This script offers a way to bridge this gap.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-grid.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set Link Alias](Set20%Link20%Alias.md)|Iterates all of the links in the selected TextElements and prompts the user to set or modify the alias for each link found.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-set-link-alias.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set stroke width of selected elements](Set%20Stroke%20Width%20of%20Selected%20Elements.md)|This script will set the stroke width of selected elements. This is helpful, for example, when you scale freedraw sketches and want to reduce or increase their line width.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-stroke-width.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Split text by lines](Split%20text%20by%20lines.md)|Split lines of text into separate text elements for easier reorganization|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-split-lines.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Set Text Alignment](Set%20Text%20Alignment.md)|Sets text alignment of text block (cetner, right, left). Useful if you want to set a keyboard shortcut for selecting text alignment.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-text-align.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Split Ellipse](Split%20Ellipse.md)|This script splits an ellipse at any point where a line intersects it.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-splitEllipse-demo1.png)|[@GColoy](https://github.com/GColoy)|
|[TheBrain-navigation](TheBrain-navigation.md)|An Excalidraw based graph user interface for your Vault. Requires the [Dataview plugin](https://github.com/blacksmithgu/obsidian-dataview). Generates a graph view similar to that of [TheBrain](https://TheBrain.com) plex. Watch introduction to this script on [YouTube](https://youtu.be/plYobK-VufM).|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/TheBrain.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Toggle Fullscreen on Mobile](Toggle%20Fullscreen%20on%20Mobile.md)|Hides Obsidian workspace leaf padding and header (based on option in settings, default is "hide header" = false) which will take Excalidraw to full screen. ⚠ Note that if the header is not visible, it will be very difficult to invoke the command palette to end full screen. Only hide the header if you have a keyboard or you've practiced opening command palette!|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/ea-toggle-fullscreen.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Toggle Grid](Toggle%20Grid.md)|Toggles the grid.||[@GColoy](https://github.com/GColoy)|
|[Transfer TextElements to Excalidraw markdown metadata](Transfer%20TextElements%20to%20Excalidraw%20markdown%20metadata.md)|The script will delete the selected text elements from the canvas and will copy the text from these text elements into the Excalidraw markdown file as metadata. This means, that the text will no longer be visible in the drawing, however you will be able to search for the text in Obsidian and find the drawing containing this image.|![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-text-to-metadata.jpg)|[@zsviczian](https://github.com/zsviczian)|
|[Zoom to Fit Selected Elements](Zoom%20to%20Fit%20Selected%20Elements.md)|Similar to Excalidraw standard <kbd>SHIFT+2</kbd> feature: Zoom to fit selected elements, but with the ability to zoom to 1000%. Inspiration: [#272](https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/272)||[@zsviczian](https://github.com/zsviczian)|
|[Hardware Eraser Suppoer](Hardware%20Eraser%20Support.md)|Allows the use of pen inversion/hardware erasers on supported pens.|[@threethan](https://github.com/threethan)|
|[Hardware Eraser Suppoer](Auto%20Draw%20for%20Pen.md)|Automatically switched from the Select tool to the Draw tool when a pen is hovered, and then back.|[@threethan](https://github.com/threethan)|


================================================
FILE: ea-scripts/Add Connector Point.md
================================================
/*
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-bullet-point.jpg)

This script will add a small circle to the top left of each text element in the selection and add the text and the "bullet point" into a group.

See documentation for more details:
https://zsviczian.github.io/obsidian-excalidraw-plugin/ExcalidrawScriptsEngine.html

```javascript
*/
elements = ea.getViewSelectedElements().filter((el)=>el.type==="text");
ea.copyViewElementsToEAforEditing(elements);
const padding = 10;
elements.forEach((el)=>{
  ea.style.strokeColor = el.strokeColor;
  const size = el.fontSize/2;
  const ellipseId = ea.addEllipse(
    el.x-padding-size,
    el.y+size/2,
    size,
    size
  );
  ea.addToGroup([el.id,ellipseId]);
});
await ea.addElementsToView(false,false,true);



================================================
FILE: ea-scripts/Add Link to Existing File and Open.md
================================================
/*
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-link-and-open.jpg)

Prompts for a file from the vault. Adds a link to the selected element pointing to the selected file. You can control in settings to open the file in the current active pane or an adjacent pane.

```javascript
*/

if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.21")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();

if(!settings["Open link in active pane"]) {
  settings = {
    "Open link in active pane": {
      value: false,
      description: "Open the link in the current active pane (on) or a new pane (off)."
	},
    ...settings
  };
  ea.setScriptSettings(settings);
}

const openInCurrentPane = settings["Open link in active pane"].value;

elements = ea.getViewSelectedElements();
if(elements.length === 0) {
  new Notice("No selected elements");
  return;
}

const files = app.vault.getFiles()
const filePaths = files.map((f)=>f.path);
file = await utils.suggester(filePaths,files,"Select a file");

if(!file) return;

const link = `[[${app.metadataCache.fileToLinktext(file,ea.targetView.file.path,true)}]]`;

ea.style.backgroundColor = "transparent";
ea.style.strokeColor = "rgba(70,130,180,0.05)"
ea.style.strokeWidth = 2;
ea.style.roughness = 0;

if(elements.length===1 && elements[0].type !== "text") {
  ea.copyViewElementsToEAforEditing(elements);
	ea.getElements()[0].link = link;
} else {
  const b = ea.getBoundingBox(elements);
  const id = ea.addEllipse(b.topX+b.width-5, b.topY, 5, 5);
  ea.getElement(id).link = link;
  ea.copyViewElementsToEAforEditing(elements);
  ea.addToGroup(elements.map((e)=>e.id).concat([id]));
}
await ea.addElementsToView(false,true,true);
ea.selectElementsInView(ea.getElements());

if(openInCurrentPane) {
	app.workspace.openLinkText(file.path,ea.targetView.file.path,false);
  return;
}
ea.openFileInNewOrAdjacentLeaf(file);



================================================
FILE: ea-scripts/Add Link to New Page and Open.md
================================================
/*
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-link-to-new-page-and-pen.jpg)

Prompts for filename. Offers option to create and open a new Markdown or Excalidraw document. Adds link pointing to the new file, to the selected objects in the drawing. You can control in settings to open the file in the current active pane or an adjacent pane.

```javascript
*/

if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.6.1")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();

if(!settings["Open link in active pane"]) {
  settings = {
    "Open link in active pane": {
      value: false,
      description: "Open the link in the current active pane (on) or a new pane (off)."
	},
    ...settings
  };
  ea.setScriptSettings(settings);
}

const openInCurrentPane = settings["Open link in active pane"].value;

elements = ea.getViewSelectedElements();
if(elements.length === 0) {
  new Notice("No selected elements");
  return;
}

const activeFile = ea.targetView.file;
const prefix = activeFile.basename;
const timestamp = moment(Date.now()).format(ea.plugin.settings.drawingFilenameDateTime);

let fileType = "";
const filename = await utils.inputPrompt (
  "Filename for new document",
  "",
  `${prefix} - ${timestamp}`,
  [
    {
      caption: "Markdown",
      action: ()=>{fileType="md";return;}
		},
    {
      caption: "Excalidraw",
      action: ()=>{fileType="ex";return;}
    }
  ]
);

if(!filename || filename === "") return;
const filepath = activeFile.path.replace(activeFile.name,`${filename}.md`);

const file = await app.fileManager.createNewMarkdownFileFromLinktext(filepath);
if(file && fileType==="ex") {
  const blank = await app.plugins.plugins["obsidian-excalidraw-plugin"].getBlankDrawing();
  await app.vault.modify(file,blank);
  await new Promise(r => setTimeout(r, 100)); //wait for metadata cache to update, so file opens as excalidraw
}

const link = `[[${app.metadataCache.fileToLinktext(file,ea.targetView.file.path,true)}]]`;

ea.style.backgroundColor = "transparent";
ea.style.strokeColor = "rgba(70,130,180,0.05)"
ea.style.strokeWidth = 2;
ea.style.roughness = 0;

if(elements.length===1 && elements[0].type !== "text") {
  ea.copyViewElementsToEAforEditing(elements);
	ea.getElements()[0].link = link;
} else {
  const b = ea.getBoundingBox(elements);
  const id = ea.addEllipse(b.topX+b.width-5, b.topY, 5, 5);
  ea.getElement(id).link = link;
  ea.copyViewElementsToEAforEditing(elements);
  ea.addToGroup(elements.map((e)=>e.id).concat([id]));
}
await ea.addElementsToView(false,true,true);
ea.selectElementsInView(ea.getElements());

if(openInCurrentPane) {
	app.workspace.openLinkText(file.path,ea.targetView.file.path,false);
  return;
}
ea.openFileInNewOrAdjacentLeaf(file);



================================================
FILE: ea-scripts/Add Next Step in Process.md
================================================
/*
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-add-process-step.jpg)

This script will prompt you for the title of the process step, then will create a stick note with the text. If an element is selected then the script will connect this new step with an arrow to the previous step (the selected element). If no element is selected, then the script assumes this is the first step in the process and will only output the sticky note with the text that was entered.

```javascript
*/

if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.5.24")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}

settings = ea.getScriptSettings();
//set default values on first run
if(!settings["Starting arrowhead"]) {
	settings = {
	  "Starting arrowhead" : {
			value: "none",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Ending arrowhead" : {
			value: "triangle",
      valueset: ["none","arrow","triangle","bar","dot"]
		},
		"Line points" : {
			value: 0,
      description: "Number of line points between start and end"
		},
		"Gap between elements": {
			value: 100
		},
		"Wrap text at (number of characters)": {
			value: 25,
		},
		"Fix width": {
			value: true,
			description: "The object around the text should have fix width to fit the wrapped text"
		}
	};
	ea.setScriptSettings(settings);
}

const arrowStart = settings["Starting arrowhead"].value === "none" ? null : settings["Starting arrowhead"].value;
const arrowEnd = settings["Ending arrowhead"].value === "none" ? null : settings["Ending arrowhead"].value;

// workaround until https://github.com/zsviczian/obsidian-excalidraw-plugin/issues/388 is fixed
if (!arrowEnd) ea.style.endArrowHead = null;
if (!arrowStart) ea.style.startArrowHead = null;

const linePoints = Math.floor(settings["Line points"].value);
const gapBetweenElements = Math.floor(settings["Gap between elements"].value);
const wrapLineLen = Math.floor(settings["Wrap text at (number of characters)"].value);
const fixWidth = settings["Fix width"];

const textPadding = 10;
const text = await utils.inputPrompt("Text?");
const elements = ea.getViewSelectedElements();
const isFirst = (!elements || elements.length === 0);

const width = ea.measureText("w".repeat(wrapLineLen)).width;

let id = "";

if(!isFirst) {
  const fromElement = ea.getLargestElement(elements);
  ea.copyViewElementsToEAforEditing([fromElement]);

  const previousTextElements = elements.filter((el)=>el.type==="text");
  const previousRectElements = elements.filter((el)=> ['ellipse', 'rectangle', 'diamond'].includes(el.type));
  if(previousTextElements.length>0) {
    const el = previousTextElements[0];
    ea.style.strokeColor = el.strokeColor;
    ea.style.fontSize    = el.fontSize;
    ea.style.fontFamily  = el.fontFamily;
  }

	textWidth = ea.measureText(text).width;

  id = ea.addText(
    fixWidth
    ? fromElement.x+fromElement.width/2-width/2
    : fromElement.x+fromElement.width/2-textWidth/2-textPadding,
    fromElement.y+fromElement.height+gapBetweenElements,
    text,
    {
      wrapAt: wrapLineLen,
      textAlign: "center",
      textVerticalAlign: "middle",
      box: previousRectElements.length > 0 ? previousRectElements[0].type : false,
      ...fixWidth
      ? {width: width, boxPadding:0}
      : {boxPadding: textPadding}
    }
  );

  ea.connectObjects(
    fromElement.id,
    null,
    id,
    null,
    {
	  endArrowHead: arrowEnd,
	  startArrowHead: arrowStart,
	  numberOfPoints: linePoints
    }
  );

  if (previousRectElements.length>0) {
    const rect = ea.getElement(id);
    rect.strokeColor = fromElement.strokeColor;
    rect.strokeWidth = fromElement.strokeWidth;
    rect.strokeStyle = fromElement.strokeStyle;
    rect.roughness = fromElement.roughness;
    rect.roundness = fromElement.roundness;
    rect.strokeSharpness = fromElement.strokeSharpness;
    rect.backgroundColor = fromElement.backgroundColor;
    rect.fillStyle = fromElement.fillStyle;
    rect.width = fromElement.width;
    rect.height = fromElement.height;
  }

  await ea.addElementsToView(false,false);
} else {
  id = ea.addText(
    0,
    0,
    text,
    {
      wrapAt: wrapLineLen,
      textAlign: "center",
      textVerticalAlign: "middle",
      box: "rectangle",
      boxPadding: textPadding,
		  ...fixWidth?{width: width}:null
    }
  );
  await ea.addElementsToView(true,false);
}

ea.selectElementsInView([ea.getElement(id)]);


================================================
FILE: ea-scripts/Auto Layout.md
================================================
/*

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-download-raw.jpg)

Download this file and save to your Obsidian Vault including the first line, or open it in "Raw" and copy the entire contents to Obsidian.

![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-auto-layout.png)

This script performs automatic layout for the selected top-level grouping objects. It is powered by [elkjs](https://github.com/kieler/elkjs) and needs to be connected to the Internet.


See documentation for more details:
https://zsviczian.github.io/obsidian-excalidraw-plugin/ExcalidrawScriptsEngine.html

```javascript
*/

if (
  !ea.verifyMinimumPluginVersion ||
  !ea.verifyMinimumPluginVersion("1.5.21")
) {
  new Notice(
    "This script requires a newer version of Excalidraw. Please install the latest version."
  );
  return;
}

settings = ea.getScriptSettings();
//set default values on first run
if (!settings["Layout Options JSON"]) {
  settings = {
    "Layout Options JSON": {
      height: "450px",
      value: `{\n      "org.eclipse.elk.layered.crossingMinimization.semiInteractive": "true",\n      "org.eclipse.elk.layered.considerModelOrder.components": "FORCE_MODEL_ORDER"\n}`,
      description: `You can use layout options to configure the layout algorithm. A list of all options and further details of their exact effects is available in <a href="http://www.eclipse.org/elk/reference.html" rel="nofollow">ELK's documentation</a>.`,
    },
  };
  ea.setScriptSettings(settings);
} 

if (typeof ELK === "undefined") {
  loadELK(doAutoLayout);
} else {
  doAutoLayout();
}

async function doAutoLayout() {
  const selectedElements = ea.getViewSelectedElements();
  const groups = ea
    .getMaximumGroups(selectedElements)
    .map((g) => g.filter((el) => el.containerId == null)) // ignore text in stickynote
    .filter((els) => els.length > 0);

  const stickynotesMap = selectedElements
    .filter((el) => el.containerId != null)
    .reduce((result, el) => {
      result.set(el.containerId, el);
      return result;
    }, new Map());

  const elk = new ELK();
  const knownLayoutAlgorithms = await elk.knownLayoutAlgorithms();
  const layoutAlgorithms = knownLayoutAlgorithms
    .map((knownLayoutAlgorithm) => ({
      id: knownLayoutAlgorithm.id,
      displayText:
        knownLayoutAlgorithm.id === "org.eclipse.elk.layered" ||
        knownLayoutAlgorithm.id === "org.eclipse.elk.radial" ||
        knownLayoutAlgorithm.id === "org.eclipse.elk.mrtree"
          ? "* " +
            knownLayoutAlgorithm.name +
            ": " +
            knownLayoutAlgorithm.description
          : knownLayoutAlgorithm.name + ": " + knownLayoutAlgorithm.description,
    }))
    .sort((lha, rha) => lha.displayText.localeCompare(rha.displayText));

  const layoutAlgorithmsSimple = knownLayoutAlgorithms
    .map((knownLayoutAlgorithm) => ({
      id: knownLayoutAlgorithm.id,
      displayText:
        knownLayoutAlgorithm.id === "org.eclipse.elk.layered" ||
        knownLayoutAlgorithm.id === "org.eclipse.elk.radial" ||
        knownLayoutAlgorithm.id === "org.eclipse.elk.mrtree"
          ? "* " + knownLayoutAlgorithm.name
          : knownLayoutAlgorithm.name,
    }))
    .sort((lha, rha) => lha.displayText.localeCompare(rha.displayText));

  // const knownOptions = knownLayoutAlgorithms
  //   .reduce(
  //     (result, knownLayoutAlgorithm) => [
  //       ...result,
  //       ...knownLayoutAlgorithm.knownOptions,
  //     ],
  //     []
  //   )
  //   .filter((value, index, self) => self.indexOf(value) === index) // remove duplicates
  //   .sort((lha, rha) => lha.localeCompare(rha));
  // console.log("knownOptions", knownOptions);

  const selectedAlgorithm = await utils.suggester(
    layoutAlgorithms.map((algorithmInfo) => algorithmInfo.displayText),
    layoutAlgorithms.map((algorithmInfo) => algorithmInfo.id),
    "Layout algorithm"
  );

  const knownNodePlacementStrategy = [
    "SIMPLE",
    "INTERACTIVE",
    "LINEAR_SEGMENTS",
    "BRANDES_KOEPF",
    "NETWORK_SIMPLEX",
  ];

  const knownDirections = [
    "UNDEFINED",
    "RIGHT",
    "LEFT",
    "DOWN",
    "UP"
  ];

  let nodePlacementStrategy = "BRANDES_KOEPF";
  let componentComponentSpacing = "10";
  let nodeNodeSpacing = "100";
  let nodeNodeBetweenLayersSpacing = "100";
  let discoComponentLayoutAlgorithm = "org.eclipse.elk.layered";
  let direction = "UNDEFINED";

  if (selectedAlgorithm === "org.eclipse.elk.layered") {
    nodePlacementStrategy = await utils.suggester(
      knownNodePlacementStrategy,
      knownNodePlacementStrategy,
      "Node placement strategy"
    );

    selectedDirection = await utils.suggester(
      knownDirections,
      knownDirections,
      "Direction"
    );
    direction = selectedDirection??"UNDEFINED";
  } else if (selectedAlgorithm === "org.eclipse.elk.disco") {
    const componentLayoutAlgorithms = layoutAlgorithmsSimple.filter(al => al.id !== "org.eclipse.elk.disco");
    const selectedDiscoComponentLayoutAlgorithm = await utils.suggester(
      componentLayoutAlgorithms.map((algorithmInfo) => algorithmInfo.displayText),
      componentLayoutAlgorithms.map((algorithmInfo) => algorithmInfo.id),
      "Disco Connected Components Layout Algorithm"
    );
    discoComponentLayoutAlgorithm = selectedDiscoComponentLayoutAlgorithm??"org.eclipse.elk.layered";
  }

  if (
    selectedAlgorithm === "org.eclipse.elk.box" ||
    selectedAlgorithm === "org.eclipse.elk.rectpacking"
  ) {
    nodeNodeSpacing = await utils.inputPrompt("Node Spacing", "number", "10");
  } else {
    let userSpacingStr = await utils.inputPrompt(
      "Components Spacing, Node Spacing, Node Node Between Layers Spacing",
      "number, number, number",
      "10, 100, 100"
    );
    let userSpacingArr = (userSpacingStr??"").split(",");
    componentComponentSpacing = userSpacingArr[0] ?? "10";
    nodeNodeSpacing = userSpacingArr[1] ?? "100";
    nodeNodeBetweenLayersSpacing = userSpacingArr[2] ?? "100";
  }

  let layoutOptionsJson = {};
  try {
    layoutOptionsJson = JSON.parse(settings["Layout Options JSON"].value);
  } catch (e) {
    new Notice(
      "Error reading Layout Options JSON, see developer console for more information",
      4000
    );
    console.log(e);
  }

  layoutOptionsJson["elk.algorithm"] = selectedAlgorithm;
  layoutOptionsJson["org.eclipse.elk.spacing.componentComponent"] =
    componentComponentSpacing;
  layoutOptionsJson["org.eclipse.elk.spacing.nodeNode"] = nodeNodeSpacing;
  layoutOptionsJson["org.eclipse.elk.layered.spacing.nodeNodeBetweenLayers"] =
    nodeNodeBetweenLayersSpacing;
  layoutOptionsJson["org.eclipse.elk.layered.nodePlacement.strategy"] =
    nodePlacementStrategy;
  layoutOptionsJson["org.eclipse.elk.disco.componentCompaction.componentLayoutAlgorithm"] = 
    discoComponentLayoutAlgorithm;
  layoutOptionsJson["org.eclipse.elk.direction"] = direction;

  const graph = {
    id: "root",
    layoutOptions: layoutOptionsJson,
    children: [],
    edges: [],
  };

  let groupMap = new Map();
  let targetElkMap = new Map();
  let arrowEls = [];

  for (let i = 0; i < groups.length; i++) {
    const elements = groups[i];
    if (
      elements.length === 1 &&
      (elements[0].type === "arrow" || elements[0].type === "line")
    ) {
      if (
        elements[0].type === "arrow" &&
        elements[0].startBinding &&
        elements[0].endBinding
      ) {
        arrowEls.push(elements[0]);
      }
    } else {
      let elkId = "g" + i;
      elements.reduce((result, el) => {
        result.set(el.id, elkId);
        return result;
      }, targetElkMap);

      const box = ea.getBoundingBox(elements);
      groupMap.set(elkId, {
        elements: elements,
        boundingBox: box,
      });

      graph.children.push({
        id: elkId,
        width: box.width,
        height: box.height,
        x: box.topX,
        y: box.topY,
      });
    }
  }

  for (let i = 0; i < arrowEls.length; i++) {
    const arrowEl = arrowEls[i];
    const startElkId = targetElkMap.get(arrowEl.startBinding.elementId);
    const endElkId = targetElkMap.get(arrowEl.endBinding.elementId);

    graph.edges.push({
      id: "e" + i,
      sources: [startElkId],
      targets: [endElkId],
    });
  }

  const initTopX =
    Math.min(...Array.from(groupMap.values()).map((v) => v.boundingBox.topX)) -
    12;
  const initTopY =
    Math.min(...Array.from(groupMap.values()).map((v) => v.boundingBox.topY)) -
    12;

  elk
    .layout(graph)
    .then((resultGraph) => {
      for (const elkEl of resultGraph.children) {
        const group = groupMap.get(elkEl.id);
        for (const groupEl of group.elements) {
          const originalDistancX = groupEl.x - group.boundingBox.topX;
          const originalDistancY = groupEl.y - group.boundingBox.topY;
          const groupElDistanceX =
            elkEl.x + initTopX + originalDistancX - groupEl.x;
          const groupElDistanceY =
            elkEl.y + initTopY + originalDistancY - groupEl.y;

          groupEl.x = groupEl.x + groupElDistanceX;
          groupEl.y = groupEl.y + groupElDistanceY;

          if (stickynotesMap.has(groupEl.id)) {
            const stickynote = stickynotesMap.get(groupEl.id);
            stickynote.x = stickynote.x + groupElDistanceX;
            stickynote.y = stickynote.y + groupElDistanceY;
          }
        }
      }

      ea.copyViewElementsToEAforEditing(selectedElements);
      ea.addElementsToView(false, false);

      normalizeSelectedArrows();
    })
    .catch(console.error);
}

function loadELK(doAfterLoaded) {
  let script = document.createElement("script");
  script.onload = function () {
    if (typeof ELK !== "undefined") {
      doAfterLoaded();
    }
  };
  script.src =
    "https://cdn.jsdelivr.net/npm/elkjs@0.8.2/lib/elk.bundled.min.js";
  document.head.appendChild(script);
}

/*
 * Normalize Selected Arrows
 */

function normalizeSelectedArrows() {
  let gapValue = 2;

  const selectedIndividualArrows = ea.getMaximumGroups(ea.getViewSelectedElements())
    .reduce((result, g) => [...result, ...g.filter(el => el.type === 'arrow')], []);

  const allElements = ea.getViewElements();
  for (const arrow of selectedIndividualArrows) {
    const startBindingEl = allElements.filter(
      (el) => el.id === (arrow.startBinding || {}).elementId
    )[0];
    const endBindingEl = allElements.filter(
      (el) => el.id === (arrow.endBinding || {}).elementId
    )[0];

    if (startBindingEl) {
      recalculateStartPointOfLine(
        arrow,
        startBindingEl,
        endBindingEl,
        gapValue
      );
    }
    if (endBindingEl) {
      recalculateEndPointOfLine(arrow, endBindingEl, startBindingEl, gapValue);
    }
  }

  ea.copyViewElementsToEAforEditing(selectedIndividualArrows);
  ea.addElementsToView(false, false);
}

function recalculateStartPointOfLine(line, el, elB, gapValue) {
  const aX = el.x + el.width / 2;
  const bX =
    line.points.length <= 2 && elB
      ? elB.x + elB.width / 2
      : line.x + line.points[1][0];
  const aY = el.y + el.height / 2;
  const bY =
    line.points.length <= 2 && elB
      ? elB.y + elB.height / 2
      : line.y + line.points[1][1];

  line.startBinding.gap = gapValue;
  line.startBinding.focus = 0;
  const intersectA = ea.intersectElementWithLine(
    el,
    [bX, bY],
    [aX, aY],
    line.startBinding.gap
  );

  if (intersectA.length > 0) {
    line.points[0] = [0, 0];
    for (let i = 1; i < line.points.length; i++) {
      line.points[i][0] -= intersectA[0][0] - line.x;
      line.points[i][1] -= intersectA[0][1] - line.y;
    }
    line.x = intersectA[0][0];
    line.y = intersectA[0][1];
  }
}

function recalculateEndPointOfLine(line, el, elB, gapValue) {
  const aX = el.x + el.width / 2;
  const bX =
    line.points.length <= 2 && elB
      ? elB.x + elB.width / 2
      : line.x + line.points[line.points.length - 2][0];
  const aY = el.y + el.height / 2;
  const bY =
    line.points.length <= 2 && elB
      ? elB.y + elB.height / 2
      : line.y + line.points[line.points.length - 2][1];

  line.endBinding.gap = gapValue;
  line.endBinding.focus = 0;
  const intersectA = ea.intersectElementWithLine(
    el,
    [bX, bY],
    [aX, aY],
    line.endBinding.gap
  );

  if (intersectA.length > 0) {
    line.points[line.points.length - 1] = [
      intersectA[0][0] - line.x,
      intersectA[0][1] - line.y,
    ];
  }
}


================================================
FILE: ea-scripts/Boolean Operations.md
================================================
/*
With This Script it is possible to make boolean Operations on Shapes. 
The style of the resulting shape will be the style of the highest ranking Element that was used. 
The ranking of the elements is based on their background. The "denser" the background, the higher the ranking (the order of backgroundstyles is shown below). If they have the same background the opacity will decide. If thats also the same its decided by the order they were created.
The ranking is also important for the difference operation, so a transparent object for example will cut a hole into a solid object.
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-boolean-operations-showcase.png)
![](https://raw.githubusercontent.com/zsviczian/obsidian-excalidraw-plugin/master/images/scripts-boolean-operations-element-ranking.png)


See documentation for more details:
https://zsviczian.github.io/obsidian-excalidraw-plugin/ExcalidrawScriptsEngine.html

```javascript
*/
if(!ea.verifyMinimumPluginVersion || !ea.verifyMinimumPluginVersion("1.9.20")) {
  new Notice("This script requires a newer version of Excalidraw. Please install the latest version.");
  return;
}
const ShadowGroupMarker = "ShadowCloneOf-";

const elements = ea.getViewSelectedElements().filter(
  el=>["ellipse", "rectangle", "diamond"].includes(el.type) ||
    el.groupIds.some(id => id.startsWith(ShadowGroupMarker)) ||
    (["line", "arrow"].includes(el.type) && el.roundness === null)
);
if(elements.length < 2) {
  new Notice ("Select ellipses, rectangles, diamonds; or lines and arrows with sharp edges");
  return;
}

const PolyBool = ea.getPolyBool();
const polyboolAction = await utils.suggester(["union (a + b)", "intersect (a && b)", "difference (a - b)", "reversed difference (b - a)", "xor"], [
  PolyBool.union, PolyBool.intersect, PolyBool.difference, PolyBool.differenceRev, PolyBool.xor
], "What would you like todo with the object");

const shadowClones = elements.filter(element => element.groupIds.some(id => id.startsWith(ShadowGroupMarker)));
shadowClones.forEach(shadowClone => {
  let parentId = shadowClone.groupIds
    .filter(id => id.startsWith(ShadowGroupMarker))[0]
    .slice(ShadowGroupMarker.length);
  const shadowCloneIndex = elements.findIndex(element => element.id == parentId);
  if (shadowCloneIndex == -1) return;
  elements[shadowCloneIndex].backgroundColor = shadowClone.backgroundColor;
  elements[shadowCloneIndex].fillStyle = shadowClone.fillStyle;
})
const borderElements = elements.filter(element => !element.groupIds.some(id => id.startsWith(ShadowGroupMarker)));
groups = ea.getMaximumGroups(borderElements);
groups = groups.map((group) => group.sort((a, b) => RankElement(b) - RankElement(a)));
groups.sort((a, b) => RankElement(b[0]) - RankElement(a[0]));

ea.style.strokeColor = groups[0][0].strokeColor;
ea.style.backgroundColor = groups[0][0].backgroundColor;
ea.style.fillStyle = groups[0][0].fillStyle;
ea.style.strokeWidth = groups[0][0].strokeWidth;
ea.style.strokeStyle = groups[0][0].strokeStyle;
ea.style.roughness = groups[0][0].roughness;
ea.style.opacity = groups[0][0].opacity;

const basePolygons = groups.shift().map(element => traceElement(element));
const toolPolygons = groups.flatMap(group => group.map(element => traceElement(element)));

const result = polyboolAction({
  regions: basePolygons,
  inverted: false
}, {
  regions: toolPolygons,
  inverted: false
});
const polygonHierachy = subordinateInnerPolygons(result.regions);
drawPolygonHierachy(polygonHierachy);
ea.deleteViewElements(elements);
setPolygonTrue();
ea.addElementsToView(false,false,true);
return;

function setPolygonTrue() {
  ea.getElements().filter(el=>el.type==="line").forEach(el => {
    el.polygon = true;
  });
}

function traceElement(element) {
  const diamondPath = (diamond) => [
      SxVEC(1/2, [0, diamond.height]),
      SxVEC(1/2, [diamond.width, 0]),
      addVec([SxVEC(1/2, [0, diamond.height]), ([diamond.width, 0])]),
      addVec([SxVEC(1/2, [diamond.width, 0]), ([0, diamond.height])]),
      SxVEC(1/2, [0, diamond.height])
    ];
  const rectanglePath = (rectangle) => [
    [0,0],
    [0, rectangle.height],
    [rectangle.width, rectangle.height],
    [rectangle.width, 0],
    [0, 0]
  ]
  const ellipsePath = (ellipse) => {
    const angle = ellipse.angle;
    const width = ellipse.width;
    const height = ellipse.height;
    const ellipseAtPoint = (t) => {
      const spanningVector = [width/2*Math.cos(t), height/2*Math.sin(t)];
      const baseVector = [width/2, height/2];
      return addVec([spanningVector, baseVector]);
    }
    let points = [];
    step = (2*Math.PI)/64
    for (let t = 0; t < 2*Math.PI; t = t + step) {
      points.push(ellipseAtPoint(t));
    }
    return points;
  }
  let polygon;
  let correctForPolygon = [0, 0];
  switch (element.type) {
    case "diamond":
      polygon = diamondPath(element);
      break;
    case "rectangle":
      polygon = rectanglePath(element);
      break;
    case "ellipse":
      polygon = ellipsePath(element);
      break;
    case "line":
    case "arrow":
      if (element.angle != 0) {
        let smallestX = 0;
        let smallestY = 0;
        element.points.forEach(point => {
          if (point[0] < smallestX) smallestX = point[0];
          if (point[1] < smallestY) smallestY = point[1];
        });
        polygon = element.points.map(point => {
          return [
            point[0] -= smallestX,
            point[1] -= smallestY
          ];
        });
        correctForPolygon = [smallestX, smallestY];
        break;
      }
      if (element.roundness) {
        new Notice("This script does not work with curved lines or arrows yet!");
        return [];
      }
      polygon = element.points; 
      default:
          break;
    }
  if (element.angle == 0) return polygon.map(v => addVec([v, [element.x, element.y]]));
  
  polygon = polygon.map(v => addVec([v, SxVEC(-1/2, [element.width, element.height])]));
  polygon = rotateVectorsByAngle(polygon, element.angle);
  return polygon.map(v => addVec([v, [element.x, element.y], SxVEC(1/2, [element.width, element.height]), correctForPolygon]));
}

function RankElement(element) {
  let score = 0;
  const backgroundRank = [
    "dashed",
    "none",
    "hachure",
    "zigzag",
    "zigzag-line",
    "cross-hatch",
    "solid"
  ]
  score += (backgroundRank.findIndex((fillStyle) => fillStyle == element.fillStyle) + 1) * 10;
  if (element.backgroundColor == "transparent") score -= 100;
  if (element.points && getVectorLength(element.points[element.points.length - 1]) > 8) score -= 100; 
  if (score < 0) score = 0;
  score += element.opacity / 100;
  return score;
}

function drawPolygonHierachy(polygonHierachy) {
  const backgroundColor = ea.style.backgroundColor;
  const strokeColor = ea.style.strokeColor;
  const setInnerStyle = () => {
    ea.style.backgroundColor = backgroundColor;
    ea.style.strokeColor = "transparent";
  }
  const setBorderStyle = () => {
    ea.style.backgroundColor = "transparent";
    ea.style.strokeColor = strokeColor;
  }
  const setFilledStyle = () => {
    ea.style.backgroundColor = backgroundColor;
    ea.style.strokeColor = strokeColor;
  }
  
  polygonHierachy.forEach(polygon => {
    setFilledStyle();
    let path = polygon.path;
    path.push(polygon.path[0]);
    if (polygon.innerPolygons.length === 0) {
      ea.addLine(path);
      return;
    }
    const outerBorder = path;
    const innerPolygons = addInnerPolygons(polygon.innerPolygons);
    path = path.concat(innerPolygons.backgroundPath);
    path.push(polygon.path[0]);
    setInnerStyle();
    const backgroundId = ea.addLine(path);
    setBorderStyle();
    const outerBorderId = ea.addLine(outerBorder)
    const innerBorderIds = innerPolygons.borderPaths.map(path => ea.addLine(path));
    const allIds = [innerBorderIds, outerBorderId, backgroundId].flat();
    ea.addToGroup(allIds);
    const background = ea.getElement(backgroundId);
    background.groupIds.push(ShadowGroupMarker + outerBorderId);
  });
}

function addInnerPolygons(polygonHierachy) {
  let firstPath = [];
  let secondPath = [];
  let borderPaths = [];
  polygonHierachy.forEach(polygon => {
    let path = polygon.path;
    path.push(polygon.path[0]);
    borderPaths.push(path);
    firstPath = firstPath.concat(path);
    secondPath.push(polygon.path[0]);
    drawPolygonHierachy(polygon.innerPolygons);
  });
  return {
    backgroundPath: firstPath.concat(secondPath.reverse()), 
    borderPaths: borderPaths
  };
}

function subordinateInnerPolygons(polygons) {
  const polygonObjectPrototype = (polygon) => {
    return {
      path: polygon,
      innerPolygons: []
    };
  }

  const insertPolygonIntoHierachy = (polygon, hierarchy) => {
    for (let i = 0; i < hierarchy.length; i++) {
      const polygonObject = hierarchy[i];
      let inside = null;
      let pointIndex = 0;
      do {
        inside = pointInPolygon(polygon[pointIndex], polygonObject.path);
        pointIndex++
      } while (inside === null);
      if (inside) {
        hierarchy[i].innerPolygons = insertPolygonIntoHierachy(polygon, hierarchy[i].innerPolygons);
        return hierarchy;
      }
    }
    polygon = polygonObjectPrototype(polygon);
    for (let i = 0; i < hierarchy.length; i++) {
      const polygonObject = hierarchy[i];
      let inside = null;
      let pointIndex = 0;
      do {
        inside = pointInPolygon(polygonObject.path[pointIndex], polygon.path);
        pointIndex++
      } while (inside === null);
      if (inside) {
        polygon.innerPolygons.push(hierarchy.splice(i, 1)[0]);
        i--;
      }
    }
    hierarchy.push(polygon);
    return hierarchy;
  }

  let polygonHierachy = [];
  polygons.forEach(polygon => {
    polygonHierachy = insertPolygonIntoHierachy(polygon, polygonHierachy);
  })

  return polygonHierachy;
}

/**
 * Checks if the given point lays in the polygon
 * @param point array [x, y]
 * @param polygon array [[x, y], ...]
 * @returns true if inside, false if not, null if the point is on one of the polygons vertecies
 */
function pointInPolygon(point, polygon) {
  const x = point[0];
  const y = point[1];
  let inside = false;

  // odd even test if point is in polyg