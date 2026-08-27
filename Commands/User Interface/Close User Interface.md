# Close User Interface

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/99-close-user-interface/*

---

# Close User Interface

## **Close User Interface**[¶](#close-user-interface "Permanent link")

Closes a currently open user interface by its unique ID, or close all open user interfaces at once.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Close All

Whether to close all open user interfaces instead of a specific one.

Toggle

User Interface ID

The unique ID of the user interface to close.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Close All Open User Interfaces**[¶](#close-all-open-user-interfaces "Permanent link")

This closes every user interface that is currently open.

Code ScriptVisual Script

`[](#__codelineno-0-1)close_user_interface(all);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAll":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.CloseUserInterfaceCommand"}`

#### **Close a Specific User Interface by Variable**[¶](#close-a-specific-user-interface-by-variable "Permanent link")

This closes the user interface whose unique ID is stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)close_user_interface($gv[0]);`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsAll":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.CloseUserInterfaceCommand"}`