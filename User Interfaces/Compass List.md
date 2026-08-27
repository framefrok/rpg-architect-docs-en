# Compass List

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/compass-list/*

---

# Compass List

## **Compass List**[¶](#compass-list "Permanent link")

Compass List elements organize items in a 3x3 grid mapped to the eight [Cardinal Directions](../../../05-reference/direction/) with a default item in the center.

> **Note**: For example, main menus that navigate between inventory, statistics, and party members. For data-driven lists, use the [Templated List](../templated-list/) instead.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animate Cursor When Unfocused

Whether or not to animate the cursor when the element is unfocused.

Toggle

Background

The image to display as a background in the element.

String

Buzzer Sound Effect

The sound to play when an invalid action occurs.

[Sound Effect](../../../05-reference/sound-effect/)

Color Mask

The color mask to apply to the cursor on the element.

Color

Confirm Sound Effect

The sound to play when confirmation occurs.

[Sound Effect](../../../05-reference/sound-effect/)

Cursor Fits Contents

Whether or not the cursor is stretched to fit the currently selected item in the element.

Toggle

Cursor Mask Margin

The margin to apply to the cursor on the element.

Number

Cursor Mask Strategy

The strategy used to compose the masked cursor on the element.

[Skin Strategy](#skin-strategy)

Cursor Offset

The amount in pixels to offset the cursor on the element.

Point

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Enable Looping

Whether or not the items in the element loop to the beginning after reaching the end and vice versa.

Toggle

Focus Script

The script to execute when the item gets focus.

[Script](../../../05-reference/script/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Hide Cursor When Unfocused

Whether or not to hide the cursor when the element is unfocused.

Toggle

Hide When Unfocused

Whether or not to hide the element when it becomes unfocused.

Toggle

Is Item Relatively Positioned

Whether or not to use relative positioning and sizing for the item in the element.

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

Item Font

The font to use on the items.

[Font](../../../05-reference/font/)

Item Margin

The margin around the item in the element.

Margin

Item Pixel Height

The height in pixels of the item in the element.

Number

Item Pixel Width

The width in pixels of the item in the element.

Number

Item Relative Height

The height relative to the list of the item.

Number

Item Relative Width

The width relative to the list of the item.

Number

Item Sprite Margin

The margin around each item's sprite within the list.

Margin

Item Text Margin

The margin around each item's text within the list.

Margin

Item Use Drop Shadow

Whether to apply a drop shadow to the text on each list item.

Toggle

Items

The items in the list.

[List Item](#list-item)

Margin

The margin around the element in pixels.

Margin

Movement Sound Effect

The sound to play when a cursor moves.

[Sound Effect](../../../05-reference/sound-effect/)

Name

The name of the element.

String

Orientation

The direction of the items composition in the element.

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

Renders In Background

Whether or not the cursor renders behind the selected item.

Toggle

Require Active User Interface

Whether or not to require the user interface to be active for the cursor to be visible.

Toggle

Require Key Selection

Whether or not the appropriate key is required to maintain the selection.

Toggle

Selected Effects

The visual effects applied when this element is selected.

[User Interface Element Effect](../../user-interface-element-effect/)

Sprite

The sprite to use for the cursor on the element.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Sprite Horizontal Alignment

The horizontal alignment of the sprite or image in the element.

[Alignment](#alignment)

Sprite Vertical Alignment

The vertical alignment of the sprite or image in the element.

[Alignment](#alignment)

Strategy

The strategy used to compose the background.

[Skin Strategy](#skin-strategy)

Template Type

The data type expected when this element is used with templated data binding.

String

Type

The method of displaying the cursor on the element.

[Cursor Type](#cursor-type)

Unfocus Script

The script to execute when the item loses focus.

[Script](../../../05-reference/script/)

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Default Sounds

Whether or not to use the default system sound effects.

Toggle

Use Item Sizing

Whether or not item sizing is defined rather than automatically calculated.

Toggle

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

Use Word Wrapping

Whether or not to wrap text to fit cleanly on multiple lines.

Toggle

## **List Item**[¶](#list-item "Permanent link")

The List Item supports rendering [Text](../text/) and/or [Pictures](../picture/) inside of it.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply.

Color

Disabled Effects

The disabled effects of the element.

[User Interface Element Effect](../../user-interface-element-effect/)

Execute Script

The execution script attached to the list item.

[Script](../../../05-reference/script/)

Focus Script

The focus script attached to the list item.

[Script](../../../05-reference/script/)

Focused Effects

The focused effects of the element.

[User Interface Element Effect](../../user-interface-element-effect/)

Override Styles

Whether or not to use the local values for styling.

Toggle

Selected Effects

The selected effects of the element.

[User Interface Element Effect](../../user-interface-element-effect/)

Sprite

The **[Sprite](../../../05-reference/sprite-or-model/)** to display.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Sprite Horizontal Alignment

The horizontal alignment of the **Sprite**.

[Alignment](#alignment)

Sprite Margin

The margin around the **Sprite**.

Margin

Sprite Vertical Alignment

The vertical alignment of the **Sprite**.

[Alignment](#alignment)

Text

The text to display.

String

Text Margin

The margin around the **Text**.

Margin

Unfocus Script

The unfocus script attached to the list item.

[Script](../../../05-reference/script/)

Unfocused Effects

The unfocused effects of the element.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Space If Hidden

Whether or not to occupy the space necessary, even if hidden.

Toggle

Use Sprite Only

Whether or not to use the sprite only.

Toggle

## **[Alignment](#alignment)**[¶](#alignment "Permanent link")

Name

Explanation

Start

Aligns to the start of the area (left or top).

Middle

Aligns to the center of the area.

End

Aligns to the end of the area (right or bottom).

## **[Cursor Type](#cursor-type)**[¶](#cursor-type "Permanent link")

Name

Explanation

None

No cursor is displayed.

Mask

Highlights the entire item with a color overlay.

Pointer - Left

Displays a pointer sprite to the left of the item.

Pointer - Right

Displays a pointer sprite to the right of the item.

Pointer - Top

Displays a pointer sprite above the item.

Pointer - Bottom

Displays a pointer sprite below the item.

## **[Orientation](#orientation)**[¶](#orientation "Permanent link")

Name

Explanation

Horizontal

Items are arranged in a horizontal row.

Vertical

Items are arranged in a vertical column.

## **[Skin Strategy](#skin-strategy)**[¶](#skin-strategy "Permanent link")

Name

Explanation

Component

Splits the skin into a 3x3 grid of corners, borders, and a center piece that scale independently.

Stretch

Stretches the entire skin image to fit the element dimensions.