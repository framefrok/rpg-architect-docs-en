# Projection Element Modifiers

*Источник: https://docs.rpg-architect.com/05-reference/projection-element-modifier/*

---

# Projection Element Modifiers

## **Projection Element Modifiers**[¶](#projection-element-modifiers "Permanent link")

Projection Elements Modifiers alter how a [Projection Element](../projection-element/) interacts with the world.

* * *

#### **Projection Element Modifiers**[¶](#projection-element-modifiers_1 "Permanent link")

*   [Origin Alignment](#origin-alignment)
*   [Rotation](#rotation)
*   [Rotational Velocity](#rotational-velocity)
*   [Scale](#scale)
*   [Translation](#translation)
*   [Velocity](#velocity)

* * *

## **Origin Alignment**[¶](#origin-alignment "Permanent link")

Origin Alignment modifiers offset the projection away from its source in the direction the source is facing.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Distance

The fixed distance from the source's origin, in world-space units. Ignored when **Use Bounding Box** is enabled.

Number

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Origin Overlap

The percentage of overlap with the source, from 0 (full distance away) to 100 (centered on the source).

Number

Use Bounding Box

Whether to derive the offset distance from the source's bounding box dimensions instead of the fixed **Distance** value.

Toggle

* * *

## **Rotation**[¶](#rotation "Permanent link")

Rotation modifiers apply a fixed angular offset to the projection each frame. Supports variable-driven values.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Pitch (X Rotation)

The amount in degrees to spin around the x axis.

[Variable or Value](../variable-or-value/)

Roll (Z Rotation)

The amount in degrees to spin around the z axis.

[Variable or Value](../variable-or-value/)

Yaw (Y Rotation)

The amount in degrees to spin around the y axis.

[Variable or Value](../variable-or-value/)

* * *

## **Rotational Velocity**[¶](#rotational-velocity "Permanent link")

Rotational Velocity modifiers spin the projection continuously around one or more axes at a given speed.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Velocity

The rotational velocity in degrees per second for each axis.

Vector

* * *

## **Scale**[¶](#scale "Permanent link")

Scale modifiers multiply the size of the projection along each axis each frame.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Scale

The scale multiplier for each axis. A value of 1 is the original size.

Vector

* * *

## **Translation**[¶](#translation "Permanent link")

Translation modifiers apply a fixed positional offset to the projection each frame.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Translation

The positional offset to apply, in world-space units.

Vector

* * *

## **Velocity**[¶](#velocity "Permanent link")

Velocity modifiers move the projection continuously in a direction at a given speed each frame.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Duration

The duration of the modifier in milliseconds. When empty, the modifier runs for the element's full duration.

Number

Offset

The delay before the modifier begins, in milliseconds from the element's start.

Number

Velocity

The velocity vector in world-space units per second.

Vector