# Battle Conditions

*Источник: https://docs.rpg-architect.com/11-battles/02-battle-conditions/*

---

# Battle Conditions

## **Battle Conditions**[¶](#battle-conditions "Permanent link")

Battle Conditions are a special kind of condition that can only be accessed in Battle. They are primarily used by [Battle Rewards](../04-battle-rewards/) and [Battle Programs](../03-battle-programs/), as well as some [Action Sequence Elements](../01-action-sequences/action-sequence-element/).

* * *

#### **Battle Conditions**[¶](#battle-conditions_1 "Permanent link")

*   [Always](#always)
*   [Enemy Formation Status Effect](#enemy-formation-status-effect)
*   [Global Switch](#global-switch)
*   [Global Variable](#global-variable)
*   [My Statistic](#my-statistic)
*   [My Status Effect](#my-status-effect)
*   [Party Status Effect](#party-status-effect)
*   [Random](#random)

* * *

## **Always**[¶](#always "Permanent link")

Always conditions pass unconditionally, always evaluating to true.

> **Note**: This is useful for battle programming, forcing a battler to **always** perform a skill, such as an 'Attack.'

* * *

## **Enemy Formation Status Effect**[¶](#enemy-formation-status-effect "Permanent link")

Enemy Formation Status Effect conditions validate that all enemies have the included status effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Status Effects

All of the status effects that are required.

[Status Effect](../../06-database/05-statistics/03-status-effects/)

* * *

## **Global Switch**[¶](#global-switch "Permanent link")

Global Switch conditions evaluate a global switch and validate that its value matches the expected value.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Index

The index of the global switch.

Number

Value

The value to compare.

Toggle

* * *

## **Global Variable**[¶](#global-variable "Permanent link")

Global Variable conditions evaluate a global variable and validate that its value satisfies the specified operator.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Index

The index of the global variable.

Number

Operator

The operator to use when making comparisons in the condition.

Operator

Value

The value to compare.

String

* * *

## **My Statistic**[¶](#my-statistic "Permanent link")

My Statistic conditions validate that a battler's statistic satisfies the specified requirements.

> **Note**: This is useful for battle programming, having a certain effect or attack occur when a battler drops below a certain amount of HP, etc.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Formula Name

The formula name of the statistic to compare.

[Statistic](../../06-database/05-statistics/01-statistics/)

Is Scale Comparison

Whether the statistic comparison is based on scale.

Toggle

Is Value Comparison

Whether the statistic comparison is based on value.

Toggle

Operator

The operand for comparison.

Operator

Value

The value to compare.

Number

* * *

## **My Status Effect**[¶](#my-status-effect "Permanent link")

My Status Effect conditions validate that a battler has the included status effects.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Is Inverted

Whether to invert the condition.

Toggle

Status Effects

All of the status effects that can fulfill the condition.

[Status Effect](../../06-database/05-statistics/03-status-effects/)

* * *

## **Party Status Effect**[¶](#party-status-effect "Permanent link")

Party Status Effect conditions validate that all party members have the included status effects.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Status Effects

Any of the status effects that can fulfill the condition.

[Status Effect](../../06-database/05-statistics/03-status-effects/)

* * *

## **Random**[¶](#random "Permanent link")

Random conditions pass based on a percentage chance.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Chance

The chance of the condition occurring.

Number