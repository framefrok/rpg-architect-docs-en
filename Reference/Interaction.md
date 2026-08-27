# Interaction

*Источник: https://docs.rpg-architect.com/05-reference/interaction/*

---

# Interaction

## **Interaction**[¶](#interaction "Permanent link")

RPG Architect supports many interactable events for [Entities](../entity/). These events include things like collisions, key presses, and so forth.

> **Note**: All interactions must evaluate to true for a script to execute.

* * *

#### **Interactions**[¶](#interactions "Permanent link")

*   [Any Interaction](#any-interaction)
*   [Automatic Interaction](#automatic-interaction)
*   [Entity Entity Collision Interaction](#entity-entity-collision-interaction)
*   [Entity Entity No Collision Interaction](#entity-entity-no-collision-interaction)
*   [Player Entity Collision Interaction](#player-entity-collision-interaction)
*   [Player Entity No Collision Interaction](#player-entity-no-collision-interaction)
*   [Player Key Collision Interaction](#player-key-collision-interaction)
*   [Projection Interaction](#projection-interaction)
*   [Virtual Key Interaction](#virtual-key-interaction)
*   [World Collision Interaction](#world-collision-interaction)

* * *

## **Any Interaction**[¶](#any-interaction "Permanent link")

Any interactions trigger when any of the contained interactions evaluate to true.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Interactions

The interactions to poll from.

[Interaction](./)

* * *

## **Automatic Interaction**[¶](#automatic-interaction "Permanent link")

Automatic interactions trigger whenever the script is present.

* * *

## **Entity Entity Collision Interaction**[¶](#entity-entity-collision-interaction "Permanent link")

Entity Entity Collision interactions trigger when an entity collides with another entity.

* * *

## **Entity Entity No Collision Interaction**[¶](#entity-entity-no-collision-interaction "Permanent link")

Entity Entity No Collision interactions trigger when an entity is not colliding with another entity.

> **Note**: For example, a door entity may close when it is not touching or colliding with the player or another entity.

* * *

## **Player Entity Collision Interaction**[¶](#player-entity-collision-interaction "Permanent link")

Player Entity Collision interactions trigger when the player collides with an entity.

* * *

## **Player Entity No Collision Interaction**[¶](#player-entity-no-collision-interaction "Permanent link")

Player Entity No Collision interactions trigger when the player is not colliding with an entity.

* * *

## **Player Key Collision Interaction**[¶](#player-key-collision-interaction "Permanent link")

Player Key Collision interactions trigger when a player presses the action key and collides with an entity.

> **Note**: For example, this is the most common kind of interaction, generally used for talking or interacting with entities.

* * *

## **Projection Interaction**[¶](#projection-interaction "Permanent link")

Projection interactions trigger when a projection collides with the entity.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Projection

The type of projection that is required.

[Projection](../../06-database/03-maps/07-projections/)

* * *

## **Virtual Key Interaction**[¶](#virtual-key-interaction "Permanent link")

Virtual Key interactions trigger when a virtual key is being pressed.

> **Note**: For example, this interaction allows for non-action key presses.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Is Ignoring Cooldown

Whether the check ignores cooldowns.

Toggle

Is Registering Cooldown

Whether to register the input cooldown when triggered.

Toggle

Virtual Key

The virtual key to evaluate.

[Virtual Key](../../06-database/10-system/50-virtual-keys/)

* * *

## **World Collision Interaction**[¶](#world-collision-interaction "Permanent link")

World Collision interactions trigger when an entity collides with world geometry, outside of other entities.

> **Note**: For example, this can detect when an entity walks into a wall or terrain boundary.