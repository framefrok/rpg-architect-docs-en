# Battle Table

*Источник: https://docs.rpg-architect.com/11-battles/03-battle-programs/battle-table/*

---

# Battle Table

## **Battle Table**[¶](#battle-table "Permanent link")

Battle Table elements select from multiple actions by chance.

> **Note**: For example, you may want to set up an enemy that has a 50% chance of attacking, or a 50% chance of running away.
> 
> **Note**: Chance values are defined as percentages.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Evaluation Method

The evaluation method to use for the battle program table.

[Chance Evaluation Method](#chance-evaluation-method)

Failure Chance

The chance of failure.

Number

Rows

The table rows eligible for random selection. Each row has a chance value that determines its likelihood of being chosen.

BattleProgramElement

#### **[Chance Evaluation Method](#chance-evaluation-method)**[¶](#chance-evaluation-method "Permanent link")

Name

Explanation

Singular

Only one item will result. Calculates the total sum of all chances and picks a single result from the weighted range.

Cumulative

Each roll is evaluated against the total of all rows. Can generate every result, using a single random number against the cumulative sum.

Reroll

Each row is independently re-evaluated with its own random roll against the maximum chance. Can generate every result.