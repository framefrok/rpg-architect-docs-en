# Light

*Источник: https://docs.rpg-architect.com/05-reference/light/*

---

# Light

## **Light**[¶](#light "Permanent link")

Lights are point light sources that illuminate the scene. They can be spherical (omni-directional) or sliced (directional cone). Omni-directional lights do not create shadows.

> **Note**: **Directional Light** is available on [Maps](../map/) and casts shadows across the scene from a distant light source. Lights defined here are local point lights on entities and doodads.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color

The color of the light.

Color

Direction

The direction of the light.

Vector

Flicker

Whether the light will flicker.

Toggle

Flicker Duration (milliseconds)

The duration between the flicker intensity in milliseconds.

Number

ID

The ID of the light.

Number

Light Type

The type of the light.

[Light Definition Type](#light-definition-type)

Maximum Intensity

The maximum intensity of the light.

Number

Maximum Radius

The maximum radius of the light.

Number

Maximum X

The maximum X constraint of the light.

Number

Maximum Y

The maximum Y constraint of the light.

Number

Maximum Z

The maximum Z constraint of the light.

Number

Minimum Intensity

The minimum intensity of the light.

Number

Minimum Radius

The minimum radius of the light.

Number

Minimum X

The minimum X constraint of the light.

Number

Minimum Y

The minimum Y constraint of the light.

Number

Minimum Z

The minimum Z constraint of the light.

Number

Position

The position of the light.

Vector

Roll

The Z rotation or roll to apply to the world positioning.

Number

Softness

The softness of the light.

Number

Texture

The texture to apply to the light.

String

#### **[Light Definition Type](#light-definition-type)**[¶](#light-definition-type "Permanent link")

Name

Explanation

Sphere

An omni-directional point light that radiates equally in all directions.

Sliced

A directional cone light that illuminates in a specific direction with configurable spread.