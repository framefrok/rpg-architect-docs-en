# Alter Battle Command

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/103-alter-battle-command/*

---

# Alter Battle Command

## **Alter Battle Command**[¶](#alter-battle-command "Permanent link")

Modifies the properties of a battle command during combat, such as its name, targeting behavior, and use scope.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Alter Auto Target

When enabled, the auto target property of the battle command will be altered.

Toggle

Alter Description

When enabled, the description of the battle command will be altered.

Toggle

Alter Enabled

When enabled, the enabled state of the battle command will be altered.

Toggle

Alter Icon

When enabled, the icon of the battle command will be altered.

Toggle

Alter Name

When enabled, the name of the battle command will be altered.

Toggle

Alter Targeting Animation

When enabled, the targeting animation of the battle command will be altered.

Toggle

Alter Targets All

When enabled, the targets all property of the battle command will be altered.

Toggle

Alter Targets Random

When enabled, the targets random property of the battle command will be altered.

Toggle

Alter Use Scope

When enabled, the use scope of the battle command will be altered.

Toggle

Auto Target

Whether the battle command should auto-target.

[Switch or Value](../../../05-reference/switch-or-value/)

Battle Command Unique ID

The unique ID of the battle command to alter.

[Variable or Value](../../../05-reference/variable-or-value/)

Description

The description text to assign to the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

Enabled

Whether the battle command is enabled.

[Switch or Value](../../../05-reference/switch-or-value/)

Icon

The icon index to assign to the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

Name

The display name to assign to the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

Targeting Animation

The targeting animation to assign to the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

Targets All

Whether all targets should be selected by the battle command.

[Switch or Value](../../../05-reference/switch-or-value/)

Targets Random

Whether random targets should be selected by the battle command.

[Switch or Value](../../../05-reference/switch-or-value/)

Use Scope

The use scope to assign to the battle command.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Rename a Battle Command**[¶](#rename-a-battle-command "Permanent link")

This changes the display name of the battle command identified by Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)alter_battle_command($gv[0], name: $gv[1]);`

`[](#__codelineno-1-1){"Data":{"AutoTarget":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"BattleCommandName":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Description":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Enabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Icon":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAutoTarget":0,"IsDescription":0,"IsEnabled":0,"IsIcon":0,"IsName":1,"IsTargetingAnimation":0,"IsTargetsAll":0,"IsTargetsRandom":0,"IsUseScope":0,"TargetingAnimation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"TargetsAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetsRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"UseScope":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.AlterBattleCommandCommand"}`

#### **Disable a Battle Command**[¶](#disable-a-battle-command "Permanent link")

This disables the battle command identified by Global Variable 0 so it cannot be selected.

Code ScriptVisual Script

`[](#__codelineno-2-1)alter_battle_command($gv[0], enabled: false);`

`[](#__codelineno-3-1){"Data":{"AutoTarget":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"BattleCommandName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Description":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Enabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Icon":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAutoTarget":0,"IsDescription":0,"IsEnabled":1,"IsIcon":0,"IsName":0,"IsTargetingAnimation":0,"IsTargetsAll":0,"IsTargetsRandom":0,"IsUseScope":0,"TargetingAnimation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"TargetsAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"TargetsRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"UseScope":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.AlterBattleCommandCommand"}`

#### **Set a Battle Command to Target All with Auto Targeting Disabled**[¶](#set-a-battle-command-to-target-all-with-auto-targeting-disabled "Permanent link")

This modifies the battle command to disable auto targeting and enable targeting all available battlers.

Code ScriptVisual Script

`[](#__codelineno-4-1)alter_battle_command($gv[0], auto_target: false, targets_all: true);`

`[](#__codelineno-5-1){"Data":{"AutoTarget":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"BattleCommandName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"BattleCommandUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Description":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Enabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Icon":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAutoTarget":1,"IsDescription":0,"IsEnabled":0,"IsIcon":0,"IsName":0,"IsTargetingAnimation":0,"IsTargetsAll":1,"IsTargetsRandom":0,"IsUseScope":0,"TargetingAnimation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"TargetsAll":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"TargetsRandom":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"UseScope":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.AlterBattleCommandCommand"}`