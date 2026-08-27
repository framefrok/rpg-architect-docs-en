# Trait Table

*Источник: https://docs.rpg-architect.com/05-reference/trait-table/*

---

# Trait Table

## **Trait Table**[¶](#trait-table "Permanent link")

A table that defines traits for a character, class, enemy, or equipment. Traits modify statistics, grant skills, add elemental properties, and more.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Rank Statistic

The statistic that tracks the current rank.

[Statistic](../../06-database/05-statistics/01-statistics/)

## **Trait Row**[¶](#trait-row "Permanent link")

A single trait entry within a trait table, defining the type, target, and modifiers for one trait at a specific rank.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Formula

The formula expression used to calculate this trait's value.

[Formula](../formulas/)

Formula Name

The statistic formula name this trait modifies.

String

Rank

The rank at which this trait becomes active.

Number

Scale Modifier

A percentage-based modifier applied to the trait's value.

Number

Statistics

The statistics and their values to apply when the trait type is a state.

[Statistics Table](../statistics-table/)

Trait Index

The database index of the trait target (e.g. which elemental, equipment slot, or skill).

Number

Trait Type

The category of trait, such as Statistic, Skill, Elemental, Equipment Slot, or State.

[Trait Type](#trait-type)

Value Modifier

A flat value modifier applied to the trait.

Number

## **[Trait Type](#trait-type)**[¶](#trait-type "Permanent link")

Name

Explanation

Statistic

Modifies a statistic value by a flat amount or scale factor.

Skill

Grants or removes a skill.

State

Applies or removes a status effect, optionally with statistic modifications.

Formula

Evaluates a formula to determine the trait's value.

Equipment Slot

Grants or removes access to an equipment slot.

Item Type

Grants or restricts the ability to use an item type.

Skill Type

Grants or restricts the ability to use a skill type.

Physical Property

Modifies a physical property such as movement speed or collision.

Tile Tag

Grants or removes the ability to traverse a tile tag.

Global Switch

Sets a global switch to on or off.

Global Variable

Modifies a global variable by a flat amount.

Elemental

Adds or modifies elemental affinity for resistance, weakness, or attack.

Battle Counter

Modifies the battle counter value used for turn ordering.

Global Variable Evaluator

Evaluates a formula and stores the result in a global variable.

Global Switch Evaluator

Evaluates a formula and stores the result as a global switch (non-zero = true).