# Change Statistic

*Источник: https://docs.rpg-architect.com/07-commands/06-character/00-change-statistic/*

---

# Change Statistic

## **Change Statistic**[¶](#change-statistic "Permanent link")

Adjusts a statistic on a character by a specified amount, as either a flat value or percentage scale.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Amount

The amount to adjust the statistic by.

[Variable or Value](../../../05-reference/variable-or-value/)

Is Value

When enabled, the amount is treated as a flat value. When disabled, the amount is treated as a percentage scale.

Toggle

Scale

When enabled, the amount is treated as a percentage multiplier against the current statistic value.

Toggle

Statistic

The formula name of the statistic to change.

[Statistic](../../../06-database/05-statistics/01-statistics/)

Target

The character to apply the operation to.

[Character](../../../06-database/00-characters/00-characters/)

Use As Delta Value

When enabled, the amount is added to the current statistic value. When disabled, the statistic is set to the specified amount.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Add Health Points to Party Member 0**[¶](#add-health-points-to-party-member-0 "Permanent link")

This increases the health points of the first active party member by 100.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_statistic(party(0), "hp", 100);`

`[](#__codelineno-1-1){"Data":{"Amount":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"FormulaName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"hp","VariableIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsScaleModifier":0,"IsValueModifier":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeStatisticCommand"}`

#### **Set a Statistic to an Absolute Value**[¶](#set-a-statistic-to-an-absolute-value "Permanent link")

This sets the health points of the first active party member to exactly 100.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_statistic(party(0), "hp", 100, set);`

`[](#__codelineno-3-1){"Data":{"Amount":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"FormulaName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"hp","VariableIndex":0,"Metadata":null},"IsDeltaOperation":0,"IsScaleModifier":0,"IsValueModifier":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeStatisticCommand"}`

#### **Scale a Statistic by a Percentage**[¶](#scale-a-statistic-by-a-percentage "Permanent link")

This scales the health points of hero 0 by 50 percent of the current value.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_statistic(hero(0), "hp", 0.5, scale);`

`[](#__codelineno-5-1){"Data":{"Amount":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"FormulaName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"hp","VariableIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsScaleModifier":1,"IsValueModifier":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeStatisticCommand"}`