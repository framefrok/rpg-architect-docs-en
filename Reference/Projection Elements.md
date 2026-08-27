# Projection Elements

*Источник: https://docs.rpg-architect.com/05-reference/projection-element/*

---

# Projection Elements

## **Projection Elements**[¶](#projection-elements "Permanent link")

Projection Elements make up the body of a [Projection](../../06-database/03-maps/07-projections/) and how that Projection interact or visualize in a game scene.

* * *

#### **Projection Elements**[¶](#projection-elements_1 "Permanent link")

*   [Entity Projection Element](#entity-projection-element)
*   [Line](#line)
*   [Sphere](#sphere)
*   [Volume](#volume)

* * *

## **Entity Projection Element**[¶](#entity-projection-element "Permanent link")

Entity projections spawn an [Entity](../../06-database/03-maps/04-entity-definitions/) into the scene.

> **Note**: The spawned **Entity Definition** has a special internal link that allows it to be picked up by the [Projection Interaction](../interaction/#projection-interaction).

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration of the element in milliseconds.

Number

Entity Definition

The entity definition to spawn.

[Entity Definition](../../06-database/03-maps/04-entity-definitions/)

Ignore Source

Whether to ignore the creator of the projectile when checking collisions. Prevents the source from hitting itself.

Toggle

Is Player Collidable

Whether the projectile can collide with a player character.

Toggle

Is Rotational Alignment Enabled

Whether to use the rotation as a rotational alignment.

Toggle

Modifiers

The modifiers applied to this element, such as translation, rotation, velocity, or scale adjustments.

[Projection Element Modifier](../projection-element-modifier/)

* * *

## **Line**[¶](#line "Permanent link")

Line projections cast a ray in the source's facing direction, detecting objects along the path.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Distance

The distance of the line in the source's facing direction, in world-space units.

Number

Duration

The duration of the element in milliseconds.

Number

Ignore Source

Whether to ignore the creator of the projectile when checking collisions. Prevents the source from hitting itself.

Toggle

Is Player Collidable

Whether the projectile can collide with a player character.

Toggle

Modifiers

The modifiers applied to this element, such as translation, rotation, velocity, or scale adjustments.

[Projection Element Modifier](../projection-element-modifier/)

* * *

## **Sphere**[¶](#sphere "Permanent link")

Sphere projections detect objects within a spherical area around the source.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Diameter

The diameter of the sphere in world-space units.

Number

Duration

The duration of the element in milliseconds.

Number

Ignore Source

Whether to ignore the creator of the projectile when checking collisions. Prevents the source from hitting itself.

Toggle

Is Player Collidable

Whether the projectile can collide with a player character.

Toggle

Modifiers

The modifiers applied to this element, such as translation, rotation, velocity, or scale adjustments.

[Projection Element Modifier](../projection-element-modifier/)

* * *

## **Volume**[¶](#volume "Permanent link")

Volume projections detect objects within a rectangular box area, with configurable width, height, and depth.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Depth

The depth of the volume on the Z axis, in world-space units.

Number

Duration

The duration of the element in milliseconds.

Number

Height

The height of the volume on the Y axis, in world-space units.

Number

Ignore Source

Whether to ignore the creator of the projectile when checking collisions. Prevents the source from hitting itself.

Toggle

Is Player Collidable

Whether the projectile can collide with a player character.

Toggle

Modifiers

The modifiers applied to this element, such as translation, rotation, velocity, or scale adjustments.

[Projection Element Modifier](../projection-element-modifier/)

Width

The width of the volume on the X axis, in world-space units.

Number