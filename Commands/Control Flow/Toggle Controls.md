# Toggle Controls

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/05-toggle-controls/*

---

# Toggle Controls

## **Toggle Controls**[¶](#toggle-controls "Permanent link")

Enables or disable player input controls.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Is Enabled

Whether the player controls are enabled. When set to false, the player cannot move or interact until controls are re-enabled.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Disable Player Controls**[¶](#disable-player-controls "Permanent link")

This disables all player input controls, preventing the player from moving or interacting.

Code ScriptVisual Script

`[](#__codelineno-0-1)toggle_controls(false);`

`[](#__codelineno-1-1){"Data":{"IsEnabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Flow.ToggleControlsCommand"}`

#### **Enable Player Controls**[¶](#enable-player-controls "Permanent link")

This re-enables all player input controls, allowing the player to move and interact again.

Code ScriptVisual Script

`[](#__codelineno-2-1)toggle_controls(true);`

`[](#__codelineno-3-1){"Data":{"IsEnabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Flow.ToggleControlsCommand"}`

#### **Toggle Controls Based on a Global Switch**[¶](#toggle-controls-based-on-a-global-switch "Permanent link")

This sets player controls to the value of Global Switch 0, allowing dynamic control toggling.

Code ScriptVisual Script

`[](#__codelineno-4-1)toggle_controls($gs[0]);`

`[](#__codelineno-5-1){"Data":{"IsEnabled":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Flow.ToggleControlsCommand"}`