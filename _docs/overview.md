---
layout: single
collection: docs
weight: 1
---

Base64 File plugin supports work with Base64 encoded files in IntellijIDEA.

### Install Plugin

1. Launch your IntellijIDEA
2. Choose <kbd>Preferences</kbd> &rarr; <kbd>Plugins</kbd> &rarr; <kbd>Marketplace</kbd>
3. Enter "Base64 File" into the search input
4. Click <kbd>Install</kbd> next to the "Base64 File"

### Functionw Overview

The plugin enriches IntellijIDEA with several actions in different parts of IDE. The plugin's actions are clearly
recognisable as they always part of action group __`Base64 File`__.

![](/assets/images/screenshot/action_group.svg){: style="width: auto; height: 50px;" }

The action group `Base64 File` is part of following menus:

* Editor popup menu
* Project tree popup menu
* Main edit menu

#### Editor

There is an action for inserting encoded file to file currently open in editor.

![](/assets/images/screenshot/editor/action_insert_encoded_file.svg){: style="width: auto; height: 40px;" }

There are actions for managing encoded files.

![](/assets/images/screenshot/editor/actions_encoded_file.svg){: style="width: auto; height: 90px;" }

And there is an action for decoding selected text to file.

![](/assets/images/screenshot/editor/action_decode_selection_to_file.svg){: style="width: auto; height: 40px;" }

Encoded files are visually marked in the editor with highlighting, and a label displaying the name of the encoded file.

![](/assets/images/screenshot/editor/encoded_file_visual_representation.svg){: style="width: auto; height: auto;" }

#### Project Tree

The plugin automatically creates a link between the encoded file value and its source file. These links are also
visually displayed in the project tree.

![](/assets/images/screenshot/project_tree/project_tree_links.svg){: style="width: auto; height: auto;" }





