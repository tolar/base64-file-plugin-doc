---
title: Editor
layout: single
collection: docs
weight: 3
---

## Encode File

The user can insert a Base64 encoded file at the caret position by invoking the appropriate action from the context
menu.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_insert_action.png" %}

### Insert Encoded File Action

| Action              | Decription                                                                                                                                                                                                                            |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Insert Encoded File | The action invokes a file selection dialog where the user can select a file from within the current project. The selected file is Base64 encoded (using the MIME scheme by default) and inserted at the caret position in the editor. |

## Encoded File Representation

The inserted encoded file is visually marked in the editor with highlighting and a label displaying the name of the
encoded file.

The relative file path of the encoded file is also displayed in the status bar below when the caret is placed within the
encoded file.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_gui_elements.png" %}

## Encoded File Manipulation

When the user invokes the context menu with the caret at the encoded value, several actions for manipulating the encoded
value are available.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_encoded_actions.png" %}

### Encoded File Actions

| Action                                                        | Decription                                                                                                                                                             |
|---------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Remove Link to Encoded File at Caret (Keeping Encoded Value)  | The action removes the link between the encoded file value at the caret and its source file. The encoded value in the editor remains unchanged.                        |
| Remove Link to Encoded File at Caret (Deleting Encoded Value) | This action removes the link between the encoded file value at the caret and its source file. The encoded value will also be removed from the file open in the editor. |
| Navigate to Encoded File at Caret                             | The action causes the file encoded at the caret position to be selected in the project view.                                                                           |
| Convert Encoding Scheme                                       | The action converts the current encoding scheme from/to MIME/BASIC.                                                                                                    |

## File Change Notification

If the encoded file changes, its encoded value will be automatically updated. This change is communicated to the user
via a notification panel at the top of the editor.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_notification.png" %}

## Decode Encoded File

The user can decode the file by selecting its encoded value in the editor and triggering the appropriate action.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_decode_action.png" %}

The user specifies the name of the file into which the selected encoded value will be decoded in the dialog that
appears.

{% include figure popup=true image_path="/assets/images/screenshot/editor/editor_overview_decode_file_name.png" %}

### Decode File Action

| Action                                              | Description                                                                                                                                                                                                                           |
|-----------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Decode Selection to File and Make Link to That File | The action triggers a dialog where the user specifies the name of the file that will be created by decoding the selected text in the editor. The file will be created in the same directory as the file containing the encoded value. |




