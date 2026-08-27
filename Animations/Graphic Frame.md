# Graphic Frame

*Источник: https://docs.rpg-architect.com/09-animations/animation-element/graphic-frame/*

---

# Graphic Frame

## **Graphic Frame**[¶](#graphic-frame "Permanent link")

Graphic Frame elements display a single image in an animation, with support for color, rotation, scale, and position adjustments.

> **Note**: This element supports tweening to generate frames.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Name

The name of this animation element. Used for identification in the timeline.

String

#### **Appearance**[¶](#appearance "Permanent link")

Name

Explanation

Type

Color Mask

The color mask applied to the graphic. Use to tint or fade the image.

Color

Hue Shift

The hue-shift applied to the graphic. Use to recolor the image without changing the source file.

Number

Rotation

The rotation of the graphic in degrees. Use to angle the image within the frame.

Number

Texture Region

The region of the source texture to display. Use to select a portion of a sprite sheet.

Rectangle

Texture Source

The file path of the source texture image.

[Image](../../../05-reference/image/)

#### **Scale**[¶](#scale "Permanent link")

Name

Explanation

Type

Scale

The scale of the graphic as an X/Y multiplier. Values above 1 enlarge, below 1 shrink.

Vector

#### **Translation**[¶](#translation "Permanent link")

Name

Explanation

Type

Translation

The position offset of the graphic relative to the animation target.

Vector