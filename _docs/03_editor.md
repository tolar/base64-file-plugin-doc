---
title: Editor
layout: single
collection: docs
weight: 3
---

## Encode & Insert File

User can insert Base64 encoded file to caret position by invoking appropriate action from context menu.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_insert_action.png" %}

### Encode & Insert File Action

| Action              | Decription                                                                                                                                                                                     |   |
|---------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|
| Insert Encoded File | Invokes file selection dialog where use select a file from within current project. The selected file is Base64 encoded (using MIME scheme as default) and inserted at caret position in editor |   |

## Encoded File Representation

The inserted encoded file is visually marked in the editor with highlighting and a label displaying a name of the
encoded file.

There is also encoded file's relative file path displayed in a status bar below, when a caret is placed withing the
encoded file.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_gui_elements.png" %}

## Encoded File Manipulation

When user invokes context menu with caret at the encoded value several actions for manipulating with encoded value is
available.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_encoded_actions.png" %}

### Encoded File Actions

| Action                                                        | Decription                                                                                                                            |   |
|---------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|---|
| Remove Link to Encoded File at Caret (Keeping Encoded Value)  | Remove link between encoded file value at caret and its source file. The encoded value in the editor remains untouched.               |   |
| Remove Link to Encoded File at Caret (Deleting Encoded Value) | Remove link between encoded file value at caret and its source file. Also the encoded value will be removed from file open in editor. |   |
| Navigate to Encoded File at Caret                             | The file encoded at caret position will be selected in project view.                                                                  |   |
| Convert Encoding Scheme                                       | Convert current encoding scheme from/to MIME/BASIC                                                                                    |   |




