---
title: Overview
layout: single
collection: docs
weight: 2
---

Base64 File plugin supports work with Base64 encoded files in IntellijIDEA.

## Function Overview

The plugin enriches IntellijIDEA with several actions in different parts of IDE. The plugin's actions are clearly
recognisable as they always part of action group __`Base64 File`__.

![]({{ site.baseurl }}/assets/images/screenshot/action_group.svg){: style="width: auto; height: 50px;" }

The action group `Base64 File` is part of following menus:

* Editor popup menu
* Project tree popup menu
* Main edit menu

## Editor

There is an action for inserting encoded file to file currently open in editor.

![]({{ site.baseurl }}/assets/images/screenshot/editor/action_insert_encoded_file.svg){: style="width: auto; height: 40px;" }

There are actions for managing encoded files.

![]({{ site.baseurl }}/assets/images/screenshot/editor/actions_encoded_file.svg){: style="width: auto; height: 90px;" }

And there is an action for decoding selected text to file.

![]({{ site.baseurl }}/assets/images/screenshot/editor/action_decode_selection_to_file.svg){: style="width: auto; height: 40px;" }

Encoded files are visually marked in the editor with highlighting, and a label displaying the name of the encoded file.

![]({{ site.baseurl }}/assets/images/screenshot/editor/encoded_file_visual_representation.svg){: style="width: auto; height: auto;" }

Learn more about [Editor Functions](/docs/03_editor/)

## Project Tree

The plugin automatically creates a link between the encoded file value and its source file. These links are also
visually displayed in the project tree.

![]({{ site.baseurl }}/assets/images/screenshot/project_tree/project_tree_links.svg){: style="width: auto; height: auto;" }

There is an action to encode and insert the selected file from the tree into the file currently open in editor at the caret position.

![]({{ site.baseurl }}/assets/images/screenshot/project_tree/action_encode_file_and_insert_at_caret.svg){: style="width: auto; height: auto;" }

Learn more about [Project Tree Functions](/docs/04_project_tree/)

## Main Menu

There is an action for removing all links between the encoded files and its source files.

![]({{ site.baseurl }}/assets/images/screenshot/menu/action_remove_all.svg){: style="width: auto; height: auto;" }

Learn more about [Main Menu Functions](/docs/05_main_menu/)





