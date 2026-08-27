# Raycast

*Источник: https://docs.rpg-architect.com/07-commands/10-physics/20-raycast/*

---

# Raycast

## **Raycast**[¶](#raycast "Permanent link")

Casts a ray from an origin in a direction and reports what it hits, writing the results to variables. The origin can be an explicit point or a source object (which is excluded from the hits). Static geometry, dynamic and kinematic objects, and clipping/ignore-collision 'ghost' objects are each disabled by default and enabled with the static, dynamic, and ghosts flags.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Depth

The maximum distance to check along the ray, in world units.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction X

The X component of the ray direction.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Y

The Y component of the ray direction.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Z

The Z component of the ray direction.

[Variable or Value](../../../05-reference/variable-or-value/)

Hit Count Variable

The variable to receive the total number of hits, including static geometry.

[Variable or Value](../../../05-reference/variable-or-value/)

Hit Dynamic Objects

When enabled, the ray hits dynamic and kinematic objects such as entities and actors.

Toggle

Hit Ghosts

When enabled, the ray also hits objects that are clipping or set to ignore collisions.

Toggle

Hit Static Geometry

When enabled, the ray hits static geometry such as walls, floors, and static doodads.

Toggle

Nearest Distance Variable

The variable to receive the distance from the origin to the nearest hit.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Normal X Variable

The variable to receive the X component of the surface normal at the nearest hit.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Normal Y Variable

The variable to receive the Y component of the surface normal at the nearest hit.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Normal Z Variable

The variable to receive the Z component of the surface normal at the nearest hit.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Point X Variable

The variable to receive the X component of the nearest hit point.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Point Y Variable

The variable to receive the Y component of the nearest hit point, which is the hit height.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Point Z Variable

The variable to receive the Z component of the nearest hit point.

[Variable or Value](../../../05-reference/variable-or-value/)

Nearest Unique ID Variable

The variable to receive the unique ID of the nearest hit object. This is empty when the nearest hit is static geometry.

[Variable or Value](../../../05-reference/variable-or-value/)

Origin X

The X component of the ray origin, used when no source object is set.

[Variable or Value](../../../05-reference/variable-or-value/)

Origin Y

The Y component of the ray origin, used when no source object is set.

[Variable or Value](../../../05-reference/variable-or-value/)

Origin Z

The Z component of the ray origin, used when no source object is set.

[Variable or Value](../../../05-reference/variable-or-value/)

Target

The physics object to target with this command.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Unique IDs Array Variable

The variable to receive a nearest-first array of the unique IDs of every hit object. Static geometry hits are not included.

[Variable or Value](../../../05-reference/variable-or-value/)

Use Source Object

When enabled, the origin is taken from a source object, which is also excluded from the hits.

Toggle