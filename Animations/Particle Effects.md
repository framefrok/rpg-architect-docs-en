# Particle Effects

*Источник: https://docs.rpg-architect.com/09-animations/particle-effect/*

---

# Particle Effects

## **Particle Effects**[¶](#particle-effects "Permanent link")

Particle Effects are effects that can be applied to [Particle Emitters](../animation-element/particle-emitter/) and alter how particles visualize and interact.

* * *

#### **Particle Effects**[¶](#particle-effects_1 "Permanent link")

*   [Acceleration](#acceleration)
*   [Color](#color)
*   [Hue Shift](#hue-shift)
*   [Opacity](#opacity)
*   [Radial Translation](#radial-translation)
*   [Radial Velocity](#radial-velocity)
*   [Scale](#scale)
*   [Translation](#translation)
*   [Velocity](#velocity)

* * *

## **Acceleration**[¶](#acceleration "Permanent link")

Acceleration effects randomly adjust a particle's velocity over time.

> **Note**: For example, gravity, wind, or turbulence.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

Frequency

The frequency interval for acceleration updates in milliseconds. Zero applies every frame.

Number

#### **X Acceleration**[¶](#x-acceleration "Permanent link")

Name

Explanation

Type

Maximum

The maximum random acceleration on the X axis per update.

Number

Minimum

The minimum random acceleration on the X axis per update.

Number

#### **Y Acceleration**[¶](#y-acceleration "Permanent link")

Name

Explanation

Type

Maximum

The maximum random acceleration on the Y axis per update.

Number

Minimum

The minimum random acceleration on the Y axis per update.

Number

#### **Z Acceleration**[¶](#z-acceleration "Permanent link")

Name

Explanation

Type

Maximum

The maximum random acceleration on the Z axis per update.

Number

Minimum

The minimum random acceleration on the Z axis per update.

Number

* * *

## **Color**[¶](#color "Permanent link")

Color effects interpolate a particle's color from a start value to an end value over the effect duration.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **Color**[¶](#color_1 "Permanent link")

Name

Explanation

Type

End Color

The color the particle transitions to by the end of the effect duration.

Color

Start Color

The initial color applied to the particle when the effect begins.

Color

* * *

## **Hue Shift**[¶](#hue-shift "Permanent link")

Hue Shift effects interpolate a particle's hue from a start value to an end value over the effect duration.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **Hue Shift**[¶](#hue-shift_1 "Permanent link")

Name

Explanation

Type

End Hue Shift

The hue-shift value the particle transitions to by the end of the effect duration.

Number

Start Hue Shift

The initial hue-shift value applied to the particle when the effect begins.

Number

* * *

## **Opacity**[¶](#opacity "Permanent link")

Opacity effects interpolate a particle's transparency from a start value to an end value over the effect duration.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **Opacity**[¶](#opacity_1 "Permanent link")

Name

Explanation

Type

End

The opacity value the particle transitions to by the end of the effect duration. Range: 0 (transparent) to 1 (opaque).

Number

Start

The initial opacity when the effect begins. Range: 0 (transparent) to 1 (opaque).

Number

* * *

## **Radial Translation**[¶](#radial-translation "Permanent link")

Radial Translation effects position a particle at a random angle and radius from the origin.

> **Note**: Use to create ring or sphere spawn patterns.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **Radius**[¶](#radius "Permanent link")

Name

Explanation

Type

Maximum

The maximum distance from the origin a particle can spawn.

Number

Minimum

The minimum distance from the origin a particle can spawn.

Number

#### **X Rotation (Pitch)**[¶](#x-rotation-pitch "Permanent link")

Name

Explanation

Type

Maximum

The maximum X rotation (pitch) angle in degrees for radial positioning.

Number

Minimum

The minimum X rotation (pitch) angle in degrees for radial positioning.

Number

#### **Y Rotation (Yaw)**[¶](#y-rotation-yaw "Permanent link")

Name

Explanation

Type

Maximum

The maximum Y rotation (yaw) angle in degrees for radial positioning.

Number

Minimum

The minimum Y rotation (yaw) angle in degrees for radial positioning.

Number

#### **Z Rotation (Roll)**[¶](#z-rotation-roll "Permanent link")

Name

Explanation

Type

Maximum

The maximum Z rotation (roll) angle in degrees for radial positioning.

Number

Minimum

The minimum Z rotation (roll) angle in degrees for radial positioning.

Number

* * *

## **Radial Velocity**[¶](#radial-velocity "Permanent link")

Radial Velocity effects set a particle's angular velocity, causing it to rotate around its origin over time.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **X Rotation (Pitch) per Second**[¶](#x-rotation-pitch-per-second "Permanent link")

Name

Explanation

Type

Maximum

The maximum X rotation (pitch) velocity in degrees per second.

Number

Minimum

The minimum X rotation (pitch) velocity in degrees per second.

Number

#### **Y Rotation (Yaw) per Second**[¶](#y-rotation-yaw-per-second "Permanent link")

Name

Explanation

Type

Maximum

The maximum Y rotation (yaw) velocity in degrees per second.

Number

Minimum

The minimum Y rotation (yaw) velocity in degrees per second.

Number

#### **Z Rotation (Roll) per Second**[¶](#z-rotation-roll-per-second "Permanent link")

Name

Explanation

Type

Maximum

The maximum Z rotation (roll) velocity in degrees per second.

Number

Minimum

The minimum Z rotation (roll) velocity in degrees per second.

Number

* * *

## **Scale**[¶](#scale "Permanent link")

Scale effects interpolate a particle's size from start values to end values over the effect duration.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **X Scale**[¶](#x-scale "Permanent link")

Name

Explanation

Type

End

The horizontal scale multiplier the particle transitions to by the end of the effect duration.

Number

Start

The initial horizontal scale multiplier when the effect begins.

Number

#### **Y Scale**[¶](#y-scale "Permanent link")

Name

Explanation

Type

End

The vertical scale multiplier the particle transitions to by the end of the effect duration.

Number

Start

The initial vertical scale multiplier when the effect begins.

Number

* * *

## **Translation**[¶](#translation "Permanent link")

Translation effects offset a particle's position by a random amount within the configured range.

> **Note**: For example, spreading spawn positions across an area.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds. Controls how long the effect is applied to each particle.

Number

#### **X Translation**[¶](#x-translation "Permanent link")

Name

Explanation

Type

Maximum

The maximum random offset on the X axis.

Number

Minimum

The minimum random offset on the X axis.

Number

#### **Y Translation**[¶](#y-translation "Permanent link")

Name

Explanation

Type

Maximum

The maximum random offset on the Y axis.

Number

Minimum

The minimum random offset on the Y axis.

Number

#### **Z Translation**[¶](#z-translation "Permanent link")

Name

Explanation

Type

Maximum

The maximum random offset on the Z axis.

Number

Minimum

The minimum random offset on the Z axis.

Number

* * *

## **Velocity**[¶](#velocity "Permanent link")

Velocity effects set a particle's linear velocity, controlling its movement direction and speed through space.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Frequency

The frequency interval for velocity updates in milliseconds. Zero applies every frame.

Number

Is Continuous

Whether the velocity is re-randomized every frame. When disabled, velocity is set once at spawn.

Toggle

#### **X Velocity**[¶](#x-velocity "Permanent link")

Name

Explanation

Type

Maximum

The maximum random velocity on the X axis.

Number

Minimum

The minimum random velocity on the X axis.

Number

#### **Y Velocity**[¶](#y-velocity "Permanent link")

Name

Explanation

Type

Maximum

The maximum random velocity on the Y axis.

Number

Minimum

The minimum random velocity on the Y axis.

Number

#### **Z Velocity**[¶](#z-velocity "Permanent link")

Name

Explanation

Type

Maximum

The maximum random velocity on the Z axis.

Number

Minimum

The minimum random velocity on the Z axis.

Number