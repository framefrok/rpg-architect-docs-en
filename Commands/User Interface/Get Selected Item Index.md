# Get Selected Item Index

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/40-get-selected-item-index/*

---

# Get Selected Item Index

## **Get Selected Item Index**[¶](#get-selected-item-index "Permanent link")

Retrieves the currently selected item index from a list-based user interface element and stores it in a variable.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Destination Variable

The variable to store the selected item index in.

[Variable or Value](../../../05-reference/variable-or-value/)

Element

The unique ID of the list-based user interface element to get the selected index from.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Get Selected Item Index into Global Variable 0**[¶](#get-selected-item-index-into-global-variable-0 "Permanent link")

This retrieves the currently selected item index from the element whose unique ID is stored in Global Variable 1, and stores the result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = get_selected_item_index($gv[1]);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.GetSelectedItemIndexCommand"}`

#### **Get Selected Item Index into Local Variable 2**[¶](#get-selected-item-index-into-local-variable-2 "Permanent link")

This retrieves the currently selected item index from the element whose unique ID is stored in Local Variable 0, and stores the result in Local Variable 2.

Code ScriptVisual Script

`[](#__codelineno-2-1)$lv[2] = get_selected_item_index($lv[0]);`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.GetSelectedItemIndexCommand"}`