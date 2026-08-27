# Set Selected Item Index

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/41-set-selected-item-index/*

---

# Set Selected Item Index

## **Set Selected Item Index**[¶](#set-selected-item-index "Permanent link")

Changes the currently selected item in a list-based user interface element to the specified index.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Element

The unique ID of the list-based user interface element to change the selection of.

[Variable or Value](../../../05-reference/variable-or-value/)

Index

The index of the item to select in the list.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set the Selected Item Index to a Specific Value**[¶](#set-the-selected-item-index-to-a-specific-value "Permanent link")

This sets the selected item index of the element whose unique ID is in Global Variable 0 to the value stored in Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_selected_item_index($gv[0], $gv[1]);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SetSelectedItemIndexCommand"}`

#### **Set the Selected Item Index to 3**[¶](#set-the-selected-item-index-to-3 "Permanent link")

This sets the selected item index of the element whose unique ID is in Global Variable 0 to index 3.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_selected_item_index($gv[0], 3);`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SetSelectedItemIndexCommand"}`