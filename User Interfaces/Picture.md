# Picture

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/picture/*

---

# Picture

## **Picture**[¶](#picture "Permanent link")

Picture elements render a sprite or image into an area.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the element.

Color

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Horizontal Alignment

The horizontal alignment of the element.

[Alignment](#alignment)

Hue Shift

The hue shift to apply to the element.

Number

Image

The static image to display in the element.

[Image](../../../05-reference/image/)

Is Linked to Selected Context

Whether this element's context updates to reflect the currently selected item in the interface.

Toggle

Is Linked to UI Context

Whether this element's context is linked to the parent interface's context.

Toggle

Is Visible

Whether the element is visible when the interface first loads. Can be toggled at runtime via effects or scripts.

Toggle

Margin

The margin around the element in pixels.

Margin

Name

The name of the element.

String

Pixel Height

The height in pixels of the element.

Number

Pixel Width

The width in pixels of the element.

Number

Pixel X

The x coordinate in pixels of the element.

Number

Pixel Y

The y coordinate in pixels of the element.

Number

Relative Height

The height relative to the container of the element.

Number

Relative Width

The width relative to the container of the element.

Number

Relative X

The x coordinate relative to the container of the element.

Number

Relative Y

The y coordinate relative to the container of the element.

Number

Selected Effects

The visual effects applied when this element is selected.

[User Interface Element Effect](../../user-interface-element-effect/)

Sprite

The [Sprite](../../../05-reference/sprite-or-model/) to display in the element.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Stretch to Boundaries

Whether to stretch the image or sprite to fill the element boundaries.

Toggle

Template Sprite

The template property name for the sprite.

String

Template Type

The data type expected when this element is used with templated data binding.

String

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

Use Template Image

Whether or not to use a template for the image.

Toggle

Use Template Sprite

Whether or not to use a template for the sprite.

Toggle

Vertical Alignment

The vertical alignment of the element.

[Alignment](#alignment)

#### **[Alignment](#alignment)**[¶](#alignment "Permanent link")

Name

Explanation

Start

Aligns to the start of the area (left or top).

Middle

Aligns to the center of the area.

End

Aligns to the end of the area (right or bottom).