# Show Battle Command Targets

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/101-show-battle-command-targets/*

---

# Show Battle Command Targets

## **Show Battle Command Targets**[¶](#show-battle-command-targets "Permanent link")

Displays targeting indicators on battlers for the specified battle command.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battle Command Unique ID

The unique ID of the battle command whose targets will be shown.

[Variable or Value](../../../05-reference/variable-or-value/)

Select All

When enabled, targeting indicators will be shown on all available targets.

[Switch or Value](../../../05-reference/switch-or-value/)

Select Random

When enabled, a targeting indicator will be shown on a random target.

[Switch or Value](../../../05-reference/switch-or-value/)

Target Unique ID

The unique ID of the specific battler to show a targeting indicator on.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Show Targeting Indicator on a Specific Battler**[¶](#show-targeting-indicator-on-a-specific-battler "Permanent link")

This displays a targeting indicator on the battler identified by Global Variable 1 for the battle command identified by Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)show_battle_command_targets($gv[0], $gv[1]);`

`[](#__codelineno-1-1){"Data":{"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SelectAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SelectRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ShowBattleCommandTargetsCommand"}`

#### **Show Targeting Indicators on All Available Targets**[¶](#show-targeting-indicators-on-all-available-targets "Permanent link")

This displays targeting indicators on all available targets for the specified battle command.

Code ScriptVisual Script

`[](#__codelineno-2-1)show_battle_command_targets($gv[0], $gv[1], select_all: true);`

`[](#__codelineno-3-1){"Data":{"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SelectAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"SelectRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ShowBattleCommandTargetsCommand"}`