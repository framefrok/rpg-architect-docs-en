# Battle Rewards

*Источник: https://docs.rpg-architect.com/11-battles/04-battle-rewards/*

---

# Battle Rewards

## **Battle Rewards**[¶](#battle-rewards "Permanent link")

Battle Rewards are given at the end of a battle, when a [Status Effect](../../06-database/05-statistics/03-status-effects/) is applied to an enemy (for example, "KO"). They are toggled on by **Grant Rewards** and can be prevented by toggling **Prevent Rewards** when setting up the Enemy Formation.

* * *

#### **Battle Rewards**[¶](#battle-rewards_1 "Permanent link")

*   [Equipment](#equipment)
*   [Global Switch](#global-switch)
*   [Global Variable](#global-variable)
*   [Item](#item)
*   [Loot Table](#loot-table)
*   [Money](#money)
*   [Statistic](#statistic)

* * *

## **Equipment**[¶](#equipment "Permanent link")

Equipment rewards grant the player an equipment item.

> **Note**: For example, an enemy might give the player a rusty sword as a reward.
> 
> **Note**: An item must have the Is Equipment flag set on it before it can be an Equipment Battle Reward.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Equipment

The equipment to award.

[Equipment](../../06-database/02-items/02-equipment/)

Is Instanced

Whether the equipment is instanced.

Toggle

Quantity

The quantity to add.

Number

Rank

The rank of the equipment.

Number

* * *

## **Global Switch**[¶](#global-switch "Permanent link")

Global Switch rewards set a global switch value.

> **Note**: For example, a boss might give different rewards based on which Switches are on and off. Switches are often used to govern world states - so you might have a boss drop something different depending on the choices the player has made in your game.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Random

Whether to assign a random value.

Toggle

Switch

The switch to update.

[Switch](../../05-reference/switch/)

Value

The value to assign to the switch.

Toggle

* * *

## **Global Variable**[¶](#global-variable "Permanent link")

Global Variable rewards perform an operation on a global variable.

> **Note**: You can use this to randomize what an enemy drops with relative ease. For example, a quick dice roll of 1-6, and if the Global Variable is 6, the enemy drops an item. For more complex randomization, you may want to use a Loot Table.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Operation

The operation to perform on the variable.

Operator

Random

Whether to assign a random value.

Toggle

Random End

The end of the random value to assign to the variable.

Number

Random Start

The start of the random value to assign to the variable.

Number

Value

The value to assign to the variable.

String

Variable

The variable to update.

[Variable](../../05-reference/variable/)

* * *

## **Item**[¶](#item "Permanent link")

Item rewards grant the player an item.

> **Note**: For example, rewarding the player with a potion.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Is Instanced

Whether the items are instanced.

Toggle

Item

The item to award.

[Item](../../06-database/02-items/01-items/)

Quantity

The quantity to add.

Number

* * *

## **Loot Table**[¶](#loot-table "Permanent link")

Loot Table rewards select items from a pre-defined loot table.

> **Note**: This makes it easier to randomize loot en masse. For example, multiple Enemy Formations can have the same loot table assigned.
> 
> **Note**: Loot tables are defined in the Loot Table in the database.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Evaluation Method

The chance evaluation method for rewards.

Evaluation Method

Loot Table

The loot table to utilize.

[Loot Table](../../06-database/02-items/03-loot-tables/)

Maximum Attempts

The maximum number of attempts to occur on the table.

[Variable or Value](../../05-reference/variable-or-value/)

Minimum Attempts

The minimum number of attempts to occur on the table.

[Variable or Value](../../05-reference/variable-or-value/)

* * *

## **Money**[¶](#money "Permanent link")

Money rewards add or subtract from the player's money.

> **Note**: For example, an enemy could drop a hundred gold pieces - or take them away.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Amount

The amount to reward, if not random.

Number

Is Random

Whether the amount is random.

Toggle

Maximum Amount

The maximum amount to reward, if random.

Number

Minimum Amount

The minimum amount to reward, if random.

Number

* * *

## **Statistic**[¶](#statistic "Permanent link")

Statistic rewards alter a character's statistic by a formula or fixed value.

> **Note**: For example, you might want an enemy to reward Experience Points, if you are using a Statistic to represent those.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Formula

The amount to reward, expressed as a formula, if not random.

[Formula](../../05-reference/formulas/)

Formula Name

The formula name of the statistic to adjust.

[Statistic](../../06-database/05-statistics/01-statistics/)

Include Active Members

Whether to include active party members in the rewards.

Toggle

Include Inactive Members

Whether to include inactive party members in the rewards.

Toggle

Is Random

Whether the amount is random.

Toggle

Maximum Amount

The maximum amount to reward, if random.

Number

Minimum Amount

The minimum amount to reward, if random.

Number