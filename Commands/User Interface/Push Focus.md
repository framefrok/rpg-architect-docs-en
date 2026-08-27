# Push Focus

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/10-push-focus/*

---

# Push Focus

## **Push Focus**[¶](#push-focus "Permanent link")

Moves focus to a specific element inside a user interface.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Element

The unique ID of the user interface element to focus on.

[Variable or Value](../../../05-reference/variable-or-value/)

Select All

Whether to select all items in the focused element.

[Switch or Value](../../../05-reference/switch-or-value/)

Select Random

Whether to randomly select an item in the focused element.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Push Focus to a Specific Element**[¶](#push-focus-to-a-specific-element "Permanent link")

This moves focus to the user interface element whose unique ID is stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)push_focus($gv[0]);`

`[](#__codelineno-1-1){"Data":{"AreAllSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"AreRandomSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushFocusCommand"}`

#### **Push Focus and Select All Items**[¶](#push-focus-and-select-all-items "Permanent link")

This moves focus to the element whose unique ID is stored in Global Variable 0 and selects all items in that element.

Code ScriptVisual Script

`[](#__codelineno-2-1)push_focus($gv[0], all: true);`

`[](#__codelineno-3-1){"Data":{"AreAllSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"AreRandomSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushFocusCommand"}`

#### **Push Focus and Randomly Select an Item**[¶](#push-focus-and-randomly-select-an-item "Permanent link")

This moves focus to the element whose unique ID is stored in Global Variable 0 and randomly selects an item.

Code ScriptVisual Script

`[](#__codelineno-4-1)push_focus($gv[0], random: true);`

`[](#__codelineno-5-1){"Data":{"AreAllSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"AreRandomSelected":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushFocusCommand"}`