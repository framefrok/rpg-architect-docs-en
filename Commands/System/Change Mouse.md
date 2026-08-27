# Change Mouse

*Источник: https://docs.rpg-architect.com/07-commands/20-system/20-change-mouse/*

---

# Change Mouse

## **Change Mouse**[¶](#change-mouse "Permanent link")

Controls whether the mouse position can be changed by the player.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Can Position Change

Whether the mouse position can be changed by the player.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Lock Mouse Position**[¶](#lock-mouse-position "Permanent link")

Prevents the player from changing the mouse position.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_mouse(false);`

`[](#__codelineno-1-1){"Data":{"IsMousePositionChangeable":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeMouseCommand"}`

#### **Unlock Mouse Position**[¶](#unlock-mouse-position "Permanent link")

Allows the player to change the mouse position freely.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_mouse(true);`

`[](#__codelineno-3-1){"Data":{"IsMousePositionChangeable":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeMouseCommand"}`

#### **Control Mouse Position with a Global Switch**[¶](#control-mouse-position-with-a-global-switch "Permanent link")

Sets whether the mouse position can change based on the value of global switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_mouse($gs[0]);`

`[](#__codelineno-5-1){"Data":{"IsMousePositionChangeable":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeMouseCommand"}`