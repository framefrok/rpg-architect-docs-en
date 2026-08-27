# Change Battle Speed

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/200-change-battle-speed/*

---

# Change Battle Speed

## **Change Battle Speed**[¶](#change-battle-speed "Permanent link")

Adjusts the speed multiplier at which the battle updates.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Speed Multiplier

The speed multiplier to apply to the battle update rate. A value of 1.0 is normal speed.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Battle Speed to Double**[¶](#set-battle-speed-to-double "Permanent link")

This sets the battle speed multiplier to 2, making the battle update twice as fast.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_battle_speed(2);`

`[](#__codelineno-1-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattleSpeedCommand"}`

#### **Reset Battle Speed to Normal**[¶](#reset-battle-speed-to-normal "Permanent link")

This resets the battle speed multiplier to 1, restoring normal battle speed.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_battle_speed(1);`

`[](#__codelineno-3-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattleSpeedCommand"}`

#### **Set Battle Speed from a Variable**[¶](#set-battle-speed-from-a-variable "Permanent link")

This sets the battle speed multiplier to the value stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_battle_speed($gv[0]);`

`[](#__codelineno-5-1){"Data":{"Multiplier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattleSpeedCommand"}`