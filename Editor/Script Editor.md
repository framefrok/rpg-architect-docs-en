# Script Editor

*Источник: https://docs.rpg-architect.com/04-editor/script-editor/*

---

# Script Editor

## **Script Editor**[¶](#script-editor "Permanent link")

The Script Editor is where every script in the project is written: a stack of commands run in order, each configured through its own dialog.

Scripts are authored visually by default. The Visual / Code toggle presents the same script as text instead, changing how it is written and stored rather than what it does.

What the individual commands do is documented under [Commands](../../07-commands/).

![The Script Editor in Visual format, showing a script as a stack of commands](../media/img_29_script-editor.png)

### ![1](../media/img_17_marker-01.png) Visual and Code[¶](#visual-and-code "Permanent link")

Switches between the command stack and the same script written as text. Visual is the default.

![The same script in Code format](../media/img_30_script-editor.code.png)

### ![2](../media/img_18_marker-02.png) Copy[¶](#copy "Permanent link")

Copies the entire script to the clipboard.

### ![3](../media/img_20_marker-03.png) Paste[¶](#paste "Permanent link")

Replaces the script with one from the clipboard.

### ![4](../media/img_22_marker-04.png) Undo[¶](#undo "Permanent link")

Steps back through edits made to this script.

### ![5](../media/img_23_marker-05.png) Redo[¶](#redo "Permanent link")

Steps forward again.

### ![6](../media/img_28_marker-06.png) Collapse All[¶](#collapse-all "Permanent link")

Folds every command down to a single line.

### ![7](../media/img_31_marker-07.png) Expand All[¶](#expand-all "Permanent link")

Opens every command out again.

### ![8](../media/img_32_marker-08.png) Pop Out[¶](#pop-out "Permanent link")

Opens the script in its own window, which is worth doing on a long script — the embedded panel is only as tall as the section hosting it.

> **Note**: In Code view, undo and redo are handled by the text editor itself rather than the script editor, so Ctrl+Z and Ctrl+Y behave as they would in any text box.