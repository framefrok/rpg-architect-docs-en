# Schedule Battle Command

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/100-schedule-battle-command/*

---

# Schedule Battle Command

## **Schedule Battle Command**[¶](#schedule-battle-command "Permanent link")

Schedules a battle command to be executed on a target battler during combat.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battle Command Unique ID

The unique ID of the battle command to schedule.

[Variable or Value](../../../05-reference/variable-or-value/)

Select All

When enabled, all available targets will be selected for the battle command.

[Switch or Value](../../../05-reference/switch-or-value/)

Select Random

When enabled, a random target will be selected for the battle command.

[Switch or Value](../../../05-reference/switch-or-value/)

Target Unique ID

The unique ID of the specific battler to target with the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Schedule a Battle Command on a Specific Target**[¶](#schedule-a-battle-command-on-a-specific-target "Permanent link")

This schedules the battle command identified by Global Variable 0 on the battler identified by Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)schedule_battle_command($gv[0], $gv[1]);`

`[](#__codelineno-1-1){"Data":{"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SelectAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SelectRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ScheduleBattleCommandCommand"}`

#### **Schedule a Battle Command Selecting All Targets**[¶](#schedule-a-battle-command-selecting-all-targets "Permanent link")

This schedules a battle command and selects all available targets.

Code ScriptVisual Script

`[](#__codelineno-2-1)schedule_battle_command($gv[0], $gv[1], select_all: true);`

`[](#__codelineno-3-1){"Data":{"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SelectAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"SelectRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ScheduleBattleCommandCommand"}`

#### **Schedule a Battle Command with Random Target Selection**[¶](#schedule-a-battle-command-with-random-target-selection "Permanent link")

This schedules a battle command and selects a random target from the available targets.

Code ScriptVisual Script

`[](#__codelineno-4-1)schedule_battle_command($gv[0], $gv[1], select_random: true);`

`[](#__codelineno-5-1){"Data":{"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SelectAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SelectRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ScheduleBattleCommandCommand"}`