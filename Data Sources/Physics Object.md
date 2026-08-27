# Physics Object

*Источник: https://docs.rpg-architect.com/08-data-sources/physics-object/*

---

# Physics Object

## **Physics Object**[¶](#physics-object "Permanent link")

Physics Object data sources get information about a physics object.

## **Properties**[¶](#properties "Permanent link")

#### **Properties**[¶](#properties_1 "Permanent link")

Name

Explanation

Type

Position (Ground) - X

The constrained position's x coordinate.

Number

Position (Ground) - Y

The constrained position's y coordinate.

Number

Position (Ground) - Z

The constrained position's z coordinate.

Number

Unclamped Position (Ground) - X

The unrestrained position's x coordinate.

Number

Unclamped Position (Ground) - Y

The unrestrained position's y coordinate.

Number

Unclamped Position (Ground) - Z

The unrestrained position's z coordinate.

Number

Velocity - X

The velocity's x component.

Number

Velocity - Y

The velocity's y component.

Number

Velocity - Z

The velocity's z component.

Number

Applied Velocity - X

The applied velocity's x component.

Number

Applied Velocity - Y

The applied velocity's y component.

Number

Applied Velocity - Z

The applied velocity's z component.

Number

Speed - X

The speed's x component.

Number

Speed - Y

The speed's y component.

Number

Speed - Z

The speed's z component.

Number

Size - X

The size's x component.

Number

Size - Y

The size's y component.

Number

Size - Z

The size's z component.

Number

Bounding Box - Minimum X

The bounding box's minimum x component.

Number

Bounding Box - Maximum X

The bounding box's maximum x component.

Number

Bounding Box - Minimum Y

The bounding box's minimum y component.

Number

Bounding Box - Maximum Y

The bounding box's maximum y component.

Number

Bounding Box - Minimum Z

The bounding box's minimum z component.

Number

Bounding Box - Maximum Z

The bounding box's maximum z component.

Number

Intended Movement - X

The intended movement's x component.

Number

Intended Movement - Y

The intended movement's y component.

Number

Intended Movement - Z

The intended movement's z component.

Number

Gravity - X

The gravity's x component.

Number

Gravity - Y

The gravity's y component.

Number

Gravity - Z

The gravity's z component.

Number

Direction

The direction.

[Direction](../../05-reference/direction/)

Prior Unclamped Position (Center of Mass) - X

The unrestrained position's prior center of mass x coordinate.

Number

Prior Unclamped Position (Center of Mass) - Y

The unrestrained position's prior center of mass y coordinate.

Number

Prior Unclamped Position (Center of Mass) - Z

The unrestrained position's prior center of mass z coordinate.

Number

Collisions - Count

The collisions associated with a physics object.

Number

Collisions - Unique ID

The unique ID of a collision.

[Unique ID](../../05-reference/unique-id/)

Position (Center of Mass) - X

The constrained position's center of mass x coordinate.

Number

Position (Center of Mass) - Y

The constrained position's center of mass y coordinate.

Number

Position (Center of Mass) - Z

The constrained position's center of mass z coordinate.

Number

Collisions Array - Unique ID

The collisions in an array.

[Array](../../05-reference/array/)

Unclamped Position (Center of Mass) - X

The constrained position's center of mass x coordinate.

Number

Unclamped Position (Center of Mass) - Y

The constrained position's center of mass y coordinate.

Number

Unclamped Position (Center of Mass) - Z

The constrained position's center of mass z coordinate.

Number

Prior Unclamped Position (Feet) - X

The unrestrained position's prior x coordinate.

Number

Prior Unclamped Position (Feet) - Y

The unrestrained position's prior y coordinate.

Number

Prior Unclamped Position (Feet) - Z

The unrestrained position's prior z coordinate.

Number

Tag

The tags of the physical object.

[Tags](../../05-reference/tags/)

Tag Count

The tag count of the physical object.

Number

Tag Key at Index

The tag key at the index of the physical object.

String

Collider Name

The name of the collider of the physical object.

String

Collider Type

The type of the collider of the physical object.

Number

Collider Width or Diameter

The width or diameter of the collider of the physical object.

Number

Collider Depth

The depth of the collider of the physical object.

Number

Collider Height

The height of the collider of the physical object.

Number

Gravity Multiplier - X

The gravity multiplier's x component.

Number

Gravity Multiplier - Y

The gravity multiplier's y component.

Number

Gravity Multiplier - Z

The gravity multiplier's z component.

Number

#### **Flags**[¶](#flags "Permanent link")

Name

Explanation

Type

Is Ignoring Collision?

Whether the physics object ignores collisions with other physics objects.

Toggle

Is Ignoring Gravity?

Whether the physics object ignores gravity.

Toggle

Is Clipping?

Whether the physics object ignores user-defined collisions.

Toggle

Is Falling?

Whether the physics object is falling.

Toggle

Is Static?

Whether the physics object is static.

Toggle

Is Airborne?

Whether the physics object is airborne.

Toggle

Is Colliding With Wall?

Whether the physics object is colliding with a wall.

Toggle

Is Grounded?

Whether the physics object is connected to the ground.

Toggle

Is Movement Captured?

Whether the physics object tried to move.

Toggle