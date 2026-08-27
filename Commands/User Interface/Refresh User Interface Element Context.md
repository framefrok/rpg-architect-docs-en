# Refresh User Interface Element Context

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/102-refresh-user-interface-element-context/*

---

# Refresh User Interface Element Context

## **Refresh User Interface Element Context**[¶](#refresh-user-interface-element-context "Permanent link")

Refreshes the context on a specific user interface element, causing it to reload its data.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

User Interface Element

The unique ID of the user interface element to refresh.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Refresh a User Interface Element by Unique ID in Global Variable 0**[¶](#refresh-a-user-interface-element-by-unique-id-in-global-variable-0 "Permanent link")

This refreshes the user interface element whose unique ID is stored in Global Variable 0, causing it to reload its data.

Code ScriptVisual Script

`[](#__codelineno-0-1)refresh_ui_element_context($gv[0]);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.RefreshUserInterfaceElementContextCommand"}`