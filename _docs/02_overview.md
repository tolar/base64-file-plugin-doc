---
title: Overview
layout: single
collection: docs
weight: 2
permalink: /documentation
---

Base64 File plugin supports work with Base64 encoded files in JetBrains IDEs like [Android Studio](https://developer.android.com/studio), 
[PyCharm](https://www.jetbrains.com/pycharm/), [IntellijIDEA](https://www.jetbrains.com/idea/), [PhpStorm](https://www.jetbrains.com/phpstorm/), 
[WebStorm](https://www.jetbrains.com/webstorm/) and others.

## Function Overview

The plugin enriches IntellijIDEA with several actions in different parts of IDE. The plugin's actions are clearly
recognisable as they always part of action group __`Base64 File`__.

![]({{ site.baseurl }}/assets/images/screenshot/action_group.svg){: style="width: auto; height: 50px;" }

The action group `Base64 File` is part of following menus:

* Editor popup menu
* Project tree popup menu
* Main edit menu

## Editor

There are two actions for inserting encoded file to file currently open in editor.

![]({{ site.baseurl }}/assets/images/screenshot/editor/actions_insert_encoded_file.svg)

There are actions for managing encoded files.

![]({{ site.baseurl }}/assets/images/screenshot/editor/actions_encoded_file.svg)

And there is an action for decoding selected text to file.

![]({{ site.baseurl }}/assets/images/screenshot/editor/action_decode_selection_to_file.svg){: style="width: auto; height: 40px;" }

Encoded files are visually marked in the editor with highlighting, and a label displaying the name of the encoded file.

![]({{ site.baseurl }}/assets/images/screenshot/editor/encoded_file_visual_representation.svg)

Learn more about [Editor Functions](/editor)

## Project Tree

The plugin automatically creates a link between the encoded file value and its source file. These links are also
visually displayed in the project tree.

![]({{ site.baseurl }}/assets/images/screenshot/project_tree/project_tree_links.svg){: style="width: auto; height: auto;" }

There are two actions to encode and insert the selected file from the tree into the file currently open in editor at the caret position.

![]({{ site.baseurl }}/assets/images/screenshot/project_tree/action_encode_file_and_insert_at_caret.svg){: style="width: auto; height: auto;" }

Learn more about [Project Tree Functions](/project_tree)

## Main Menu

There is an action for removing all links between the encoded files and its source files.

![]({{ site.baseurl }}/assets/images/screenshot/menu/action_remove_all.svg){: style="width: auto; height: auto;" }

Learn more about [Main Menu Functions](/main_menu)





