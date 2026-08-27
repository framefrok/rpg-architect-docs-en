# Trait Effect Table

*Источник: https://docs.rpg-architect.com/05-reference/trait-effect-table/*

---

# Trait Effect Table

## **Trait Effect Table**[¶](#trait-effect-table "Permanent link")

A table that defines the effects applied by skills, items, or status effects. Effects modify statistics, apply states, interact with elementals, and can occur on recurring intervals.

## **Effect Row**[¶](#effect-row "Permanent link")

A single effect entry within an effect table, defining what is modified, by how much, and optionally on a recurring schedule.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Formula

The formula expression used to calculate this trait's value.

[Formula](../formulas/)

Formula Name

The statistic formula name this trait modifies.

String

Ignores Modifiers

Whether to bypass elemental resistance and weakness modifiers.

Toggle

Is Forced

Whether this effect is applied regardless of other conditions.

Toggle

Is Occurrence Unending

Whether the recurring effect continues indefinitely without ending.

Toggle

Occurrence End Formula

The formula that determines when the recurring effect ends.

[Formula](../formulas/)

Occurrence End Type

The unit of time used to measure when the recurring effect ends.

[Trait Effect Occurrence](#trait-effect-occurrence)

Occurrence Frequency Formula

The formula that determines how often the recurring effect triggers.

[Formula](../formulas/)

Occurrence Frequency Type

The unit of time used to measure how often the recurring effect triggers.

[Trait Effect Occurrence](#trait-effect-occurrence)

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

Uses Occurrences

Whether this effect recurs on a schedule rather than applying once.

Toggle

Value Modifier

A flat value modifier applied to the trait.

Number

## **[Trait Effect Occurrence](#trait-effect-occurrence)**[¶](#trait-effect-occurrence "Permanent link")

Name

Explanation

Step

Triggers every step the character takes on the map.

Second (Battle)

Triggers every second during battle.

Second (Non-Battle)

Triggers every second on the map (outside of battle).

Round

Triggers every round in turn-based battles.

Turn or Action (After)

Triggers after each turn (turn-based) or action (counter-based).

Turn or Action (Before)

Triggers before each turn (turn-based) or action (counter-based).

Counter

Triggers on every battle counter increment.

Battle Won

Triggers once when a battle the battler participated in ends in victory.

Battle Escaped

Triggers once when the battler escapes from a battle.

Battle Defeated

Triggers once when a battle the battler participated in ends in defeat.

Battle Ended

Triggers once when any battle the battler participated in ends, regardless of outcome.

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