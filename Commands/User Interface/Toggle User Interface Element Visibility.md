# Toggle User Interface Element Visibility

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/20-toggle-user-interface-element-visibility/*

---

# Toggle User Interface Element Visibility

## **Toggle User Interface Element Visibility**[¶](#toggle-user-interface-element-visibility "Permanent link")

Changes whether a specific user interface element is visible or hidden.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

User Interface Element

The unique ID of the user interface element to change the visibility of.

[Variable or Value](../../../05-reference/variable-or-value/)

Visibility

Whether the user interface element should be visible.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Show a User Interface Element**[¶](#show-a-user-interface-element "Permanent link")

This makes the user interface element whose unique ID is stored in Global Variable 0 visible.

Code ScriptVisual Script

`[](#__codelineno-0-1)toggle_ui_element_visibility($gv[0], true);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.ToggleUserInterfaceElementVisibilityCommand"}`

#### **Hide a User Interface Element**[¶](#hide-a-user-interface-element "Permanent link")

This hides the user interface element whose unique ID is stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)toggle_ui_element_visibility($gv[0], false);`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.ToggleUserInterfaceElementVisibilityCommand"}`

#### **Toggle Visibility Based on a Global Switch**[¶](#toggle-visibility-based-on-a-global-switch "Permanent link")

This sets the visibility of the element to match the value of Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)toggle_ui_element_visibility($gv[0], $gs[0]);`

`[](#__codelineno-5-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.ToggleUserInterfaceElementVisibilityCommand"}`