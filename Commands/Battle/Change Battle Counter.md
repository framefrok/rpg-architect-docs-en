# Change Battle Counter

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/50-change-battle-counter/*

---

# Change Battle Counter

## **Change Battle Counter**[¶](#change-battle-counter "Permanent link")

Adjusts or sets the battle counter value of a specific battler during combat.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battler Unique ID

The unique ID of the battler whose counter will be changed.

[Variable or Value](../../../05-reference/variable-or-value/)

Counter

The amount to adjust the counter by or set the counter to.

[Variable or Value](../../../05-reference/variable-or-value/)

Use As Delta Value

When enabled, the counter is adjusted by the specified amount. When disabled, the counter is set to the specified amount.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Increase a Battler Counter by a Delta Value**[¶](#increase-a-battler-counter-by-a-delta-value "Permanent link")

This increases the battle counter of the battler identified by Global Variable 0 by the amount stored in Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_battle_counter($gv[0], $gv[1]);`

`[](#__codelineno-1-1){"Data":{"BattlerUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Counter":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"IsDeltaOperation":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattleCounterCommand"}`

#### **Set a Battler Counter to an Absolute Value**[¶](#set-a-battler-counter-to-an-absolute-value "Permanent link")

This sets the battle counter of the specified battler to exactly 100, replacing the current value.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_battle_counter($gv[0], 100, set);`

`[](#__codelineno-3-1){"Data":{"BattlerUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Counter":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsDeltaOperation":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattleCounterCommand"}`