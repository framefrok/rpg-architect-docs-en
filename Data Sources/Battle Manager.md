# Battle Manager

*Источник: https://docs.rpg-architect.com/08-data-sources/battle-manager/*

---

# Battle Manager

## **Battle Manager**[¶](#battle-manager "Permanent link")

Battle Manager data sources get information from the battle manager.

## **Properties**[¶](#properties "Permanent link")

#### **Properties**[¶](#properties_1 "Permanent link")

Name

Explanation

Type

Active Battlers - Count

The number of active battlers.

Number

Active Battler Unique ID by Index

The unique ID of an active battler by index.

[Unique ID](../../05-reference/unique-id/)

Scheduling Battler Unique ID

The scheduling battler's unique ID.

[Unique ID](../../05-reference/unique-id/)

Targeted Battlers - Count

The number of battlers that are currently being targeted by a scheduling battler.

Number

Targeted Battlers Unique ID by Index

The unique ID of a targeted battler by index.

[Unique ID](../../05-reference/unique-id/)

Heroes - Count

The number of heroes in the battle.

Number

Enemies - Count

The number of enemies in the battle.

Number

Hero Unique ID by Index

The unique ID of a hero by index.

[Unique ID](../../05-reference/unique-id/)

Enemy Unique ID by Index

The unique ID of an enemy by index.

[Unique ID](../../05-reference/unique-id/)

Turns

The turns elapsed in a battle.

Number

Rounds

The rounds elapsed in a battle.

Number

Scheduling Battler Commands - Count

The scheduling battler's command count.

Number

Scheduling Battler Command Unique ID by Index

The scheduling battler's command unique ID by index.

[Unique ID](../../05-reference/unique-id/)

Acting Battler Unique ID

The acting battler's unique ID.

[Unique ID](../../05-reference/unique-id/)

Acting Battler Action Unique ID

The acting battler's command unique ID.

[Unique ID](../../05-reference/unique-id/)

Heroes Array - Unique ID

The unique IDs of all of the heroes.

[Array](../../05-reference/array/)

Enemies Array - Unique ID

The unique IDs of all of the enemies.

[Array](../../05-reference/array/)

Targeted Battlers Array - Unique ID

The unique IDs of all of the targeted battlers.

[Array](../../05-reference/array/)

Battlers Array - Unique ID

The unique IDs of all of the battlers.

[Array](../../05-reference/array/)

Logs

The logs of the battle.

String

Logs Array - By Line

The logs of the battle, separated by line.

[Array](../../05-reference/array/)

Active Heroes - Count

The number of active hero battlers.

Number

Active Enemies - Count

The number of active enemy battlers.

Number

Active Hero Unique ID by Index

The unique ID of an active hero battler by index.

[Unique ID](../../05-reference/unique-id/)

Active Enemy Unique ID by Index

The unique ID of an active enemy battler by index.

[Unique ID](../../05-reference/unique-id/)

#### **Flags**[¶](#flags "Permanent link")

Name

Explanation

Type

Is Active

Whether a battle is currently running.

Toggle

Is Paused

Whether the battle is paused for any reason.

Toggle

Is Paused for Animation

Whether the battle is paused for an animation.

Toggle

Is Paused for Input

Whether the battle is paused for input.

Toggle

Is Paused for Script

Whether the battle is paused for script execution.

Toggle

Is Escapable?

Whether the battle is escapable.

Toggle

Phase - Introduction

Whether the battle is in the introduction phase.

Toggle

Phase - Active

Whether the battle is in the active phase.

Toggle

Phase - Victory

Whether the battle is in the victory phase.

Toggle

Phase - Defeat

Whether the battle is in the defeat phase.

Toggle