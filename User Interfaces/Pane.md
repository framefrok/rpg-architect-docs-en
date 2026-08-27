# Pane

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/pane/*

---

# Pane

## **Pane**[¶](#pane "Permanent link")

Pane elements render a border or window background into a fixed area, using a skinning strategy such as stretch or 9-slice compositing.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Background

The image to display as a background in the element.

[Image](../../../05-reference/image/)

Color Mask

The color mask to apply to the element.

Color

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Hue Shift

The hue shift to apply to the element.

Number

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

Strategy

The strategy used to compose the background.

[Skin Strategy](#skin-strategy)

Template Type

The data type expected when this element is used with templated data binding.

String

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

Use Template Background Image

Whether or not to use a template for the background image.

Toggle

#### **[Skin Strategy](#skin-strategy)**[¶](#skin-strategy "Permanent link")

Name

Explanation

Component

Splits the skin into a 3x3 grid of corners, borders, and a center piece that scale independently.

Stretch

Stretches the entire skin image to fit the element dimensions.