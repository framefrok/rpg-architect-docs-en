# Templated List

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/templated-list/*

---

# Templated List

## **Templated List**[¶](#templated-list "Permanent link")

Templated List elements render a variable list of items from a [Context](../../../05-reference/context/), compositing child [User Interface Elements](../) that use templated values to display each item.

> **Note**: For example, party member lists, inventory screens, or skill lists where the number of items changes at runtime.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animate Cursor When Unfocused

Whether or not to animate the cursor when the element is unfocused.

Toggle

Buzzer Sound Effect

The sound to play when an invalid action occurs.

[Sound Effect](../../../05-reference/sound-effect/)

Color Mask

The color mask to apply to the cursor on the element.

Color

Confirm Sound Effect

The sound to play when confirmation occurs.

[Sound Effect](../../../05-reference/sound-effect/)

Cursor Mask Margin

The margin to apply to the cursor on the element.

Number

Cursor Mask Strategy

The strategy used to compose the masked cursor on the element.

[Skin Strategy](#skin-strategy)

Cursor Offset

The amount in pixels to offset the cursor on the element.

Point

Custom Context

The custom context property to use on the element.

String

Custom Context Template Type

The data type the custom context is read from. The custom context names a collection on this type, and each item in that collection uses the element's template type.

String

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Enable Looping

Whether or not the items in the element loop to the beginning after reaching the end and vice versa.

Toggle

Execute Script

The script to execute when a list item is confirmed.

[Script](../../../05-reference/script/)

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

Item Components

The item components in a templated item.

[User Interface Element](../)

Item Focus Script

The script to execute when an individual item gains focus.

[Script](../../../05-reference/script/)

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

The height relative to the templated list of the item.

Number

Item Relative Width

The width relative to the templated list of the item.

Number

Item Unfocus Script

The script to execute when an individual item loses focus.

[Script](../../../05-reference/script/)

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

The direction items are arranged in, either vertically or horizontally.

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

Selected Effects

The visual effects applied when this element is selected.

[User Interface Element Effect](../../user-interface-element-effect/)

Sprite

The sprite to use for the cursor on the element.

[Sprite or Model](../../../05-reference/sprite-or-model/)

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

Use Custom Context

Whether or not to use a custom context property on the element.

Toggle

Use Default Sounds

Whether or not to use the default system sound effects.

Toggle

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

#### **[Cursor Type](#cursor-type)**[¶](#cursor-type "Permanent link")

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

#### **[Orientation](#orientation)**[¶](#orientation "Permanent link")

Name

Explanation

Horizontal

Items are arranged in a horizontal row.

Vertical

Items are arranged in a vertical column.

#### **[Skin Strategy](#skin-strategy)**[¶](#skin-strategy "Permanent link")

Name

Explanation

Component

Splits the skin into a 3x3 grid of corners, borders, and a center piece that scale independently.

Stretch

Stretches the entire skin image to fit the element dimensions.