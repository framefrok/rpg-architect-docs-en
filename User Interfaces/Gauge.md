# Gauge

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/gauge/*

---

# Gauge

## **Gauge**[¶](#gauge "Permanent link")

Gauge elements render a value in a fixed range, utilizing different fill strategies.

> **Note**: For example, health bars, experience progress bars, or magic point meters.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Alignment

The anchor that determines which edge the gauge fills from.

[Alignment](#alignment)

Color Mask

The color mask to apply to the element.

Color

Current Value

The template property name that provides the current value of the gauge at runtime.

String

Cursor Model

The cursor to use for the visual, if it is interactable.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

End

The sprite to use for the end of the gauge.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Fill

The sprite to use for the filled area between the start and end of the gauge.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Fill Strategy

The method used to render the fill sprite between the start and end of the gauge.

[Fill Strategy](#fill-strategy)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Is Linked to Selected Context

Whether this element's context updates to reflect the currently selected item in the interface.

Toggle

Is Linked to UI Context

Whether this element's context is linked to the parent interface's context.

Toggle

Is Visible

Whether the element is visible when the interface first loads. Can be toggled at runtime via effects or scripts.

Toggle

Maintain Limits

Whether to clamp the gauge so it cannot exceed the minimum or maximum values.

Toggle

Margin

The margin around the element in pixels.

Margin

Maximum Value

The template property name that provides the maximum value of the gauge at runtime.

String

Minimum Value

The template property name that provides the minimum value of the gauge at runtime.

String

Name

The name of the element.

String

Orientation

The orientation of the gauge.

[Orientation](#orientation)

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

Start

The sprite to use for the start of the gauge.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Template Type

The data type expected when this element is used with templated data binding.

String

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

#### **[Alignment](#alignment)**[¶](#alignment "Permanent link")

Name

Explanation

Start

Aligns to the start of the area (left or top).

Middle

Aligns to the center of the area.

End

Aligns to the end of the area (right or bottom).

#### **[Fill Strategy](#fill-strategy)**[¶](#fill-strategy "Permanent link")

Name

Explanation

Repeat

Tiles the image repeatedly to fill the area.

Percentage

Fills a percentage of the area based on the current value.

Stretch

Stretches the image to fill the entire area.

#### **[Orientation](#orientation)**[¶](#orientation "Permanent link")

Name

Explanation

Horizontal

Items are arranged in a horizontal row.

Vertical

Items are arranged in a vertical column.