# Annotations

*Источник: https://docs.rpg-architect.com/05-reference/annotation/*

---

# Annotations

## **Annotations**[¶](#annotations "Permanent link")

Annotations are (generally) 2D visuals that display on top of [Actors](../actor-reference/).

> **Note**: Annotations render above the scene being drawn, but before the user interface layer.
> 
> **Note**: These are usually used when making quest markers or way-points.

* * *

#### **Annotations**[¶](#annotations_1 "Permanent link")

*   [Rectangle](#rectangle)
*   [Sprite](#sprite)
*   [Text](#text)

* * *

## **Rectangle**[¶](#rectangle "Permanent link")

Rectangle annotations render a colored rectangle based on a width and height.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color

The tint color applied to the annotation. Defaults to white (no tint).

Color

Effects

The sequence of effects applied to this annotation, such as movement, color changes, or text replacement.

[Annotation Effect](../annotation-effect/)

Height

The height of the rectangle in pixels.

Number

Is Persistent

Whether the annotation stays on screen indefinitely. When disabled, the annotation disappears after its effects complete.

Toggle

Offset

The offset of the annotation in world-space units, relative to the attached object's position.

Vector

Pixel Offset

The offset of the annotation in screen-space pixels, applied after the world-space offset.

Point

Width

The width of the rectangle in pixels.

Number

* * *

## **Sprite**[¶](#sprite "Permanent link")

Sprite annotations render a sprite or image with a provided width and height.

> **Note**: This annotation is commonly used to display quest markers, way-points, and so forth.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Color

The tint color applied to the annotation. Defaults to white (no tint).

Color

Effects

The sequence of effects applied to this annotation, such as movement, color changes, or text replacement.

[Annotation Effect](../annotation-effect/)

Height

The custom height of the image or sprite.

Number

Is Persistent

Whether the annotation stays on screen indefinitely. When disabled, the annotation disappears after its effects complete.

Toggle

Is Sprite Cycling

Whether the sprite continues to cycle through its animation frames after reaching the last frame.

Toggle

Offset

The offset of the annotation in world-space units, relative to the attached object's position.

Vector

Pixel Offset

The offset of the annotation in screen-space pixels, applied after the world-space offset.

Point

Sprite

The image or sprite used by the annotation.

[Sprite or Model](../sprite-or-model/)

Stretch To Dimensions

Whether to stretch the image to the custom Width and Height values instead of using the sprite's native frame size.

Toggle

Width

The custom width of the image or sprite.

Number

* * *

## **Text**[¶](#text "Permanent link")

Text annotations render text with the provided font.

> **Note**: This annotation is commonly used to display names above NPCs.
> 
> **Note**: Also supports [Text Escape Codes](../text-escape-codes/) for dynamic content.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Color

The tint color applied to the annotation. Defaults to white (no tint).

Color

Effects

The sequence of effects applied to this annotation, such as movement, color changes, or text replacement.

[Annotation Effect](../annotation-effect/)

Font

The font used to render the annotation's text, including family, size, and style.

[Font](../font/)

Is Persistent

Whether the annotation stays on screen indefinitely. When disabled, the annotation disappears after its effects complete.

Toggle

Offset

The offset of the annotation in world-space units, relative to the attached object's position.

Vector

Pixel Offset

The offset of the annotation in screen-space pixels, applied after the world-space offset.

Point

Text

The text content displayed by the annotation. Supports localization.

String