# Slider

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/slider/*

---

# Slider

## **Slider**[¶](#slider "Permanent link")

Slider elements are interactable [Gauges](../gauge/) whose value can be increased or decreased based on input.

> **Note**: For example, volume sliders for sound effects or music.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animate When Unfocused

Whether or not to animate the cursor and fill when unfocused.

Toggle

Change

The amount the slider value changes per input step.

[Variable or Value](../../../05-reference/variable-or-value/)

Color Mask

The color mask to apply to the element.

Color

Confirm Sound Effect

The sound to play when confirmation occurs.

[Sound Effect](../../../05-reference/sound-effect/)

Current Value

The variable or value that tracks the current position of the slider.

[Variable or Value](../../../05-reference/variable-or-value/)

Cursor Offset

The amount in pixels to offset the cursor on the element.

Point

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Execute Script

The script to execute when the confirm button is pressed.

[Script](../../../05-reference/script/)

Fill

The sprite to use for the filled area between the start and end of the slider.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Fill Strategy

The method used to render the fill sprite between the start and end of the slider.

[Fill Strategy](#fill-strategy)

Focus Script

The script to execute when the item gets focus.

[Script](../../../05-reference/script/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Hide Cursor When Unfocused

Whether or not to hide the cursor when the element is unfocused.

Toggle

Invert Direction

Whether or not to invert the direction of the slider.

Toggle

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

Maximum Value

The variable or value that defines the upper bound of the slider range.

[Variable or Value](../../../05-reference/variable-or-value/)

Minimum Value

The variable or value that defines the lower bound of the slider range.

[Variable or Value](../../../05-reference/variable-or-value/)

Movement Sound Effect

The sound to play when a cursor moves.

[Sound Effect](../../../05-reference/sound-effect/)

Name

The name of the element.

String

Orientation

The orientation of the slider.

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

Sprite

The sprite to use for the current position of the slider.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Template Type

The data type expected when this element is used with templated data binding.

String

Unfocus Script

The script to execute when the item loses focus.

[Script](../../../05-reference/script/)

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Default Sounds

Whether or not to use the default system sound effects.

Toggle

Use Floating Points

Whether or not to use floating points when evaluating the values.

Toggle

Use Integers

Whether or not to use integers when evaluating the values.

Toggle

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

Value Changed Script

The script to execute when the value changes.

[Script](../../../05-reference/script/)

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