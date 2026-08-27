# Text

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/text/*

---

# Text

## **Text**[¶](#text "Permanent link")

Text elements render text in a user interface.

> **Note**: Also supports [Text Escape Codes](../../../05-reference/text-escape-codes/) for dynamic content.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Character Delay

The number of milliseconds to wait before displaying the next character in the text.

Number

Character Sound

The sound effect to play when each character displays in the text.

[Sound Effect](../../../05-reference/sound-effect/)

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Font

The font used to render the text in this element.

[Font](../../../05-reference/font/)

Horizontal Alignment

The horizontal alignment of the text in the element.

[Alignment](#alignment)

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

Template

The template property name that provides the text content at runtime.

String

Template Type

The data type expected when this element is used with templated data binding.

String

Text

The text to display in the element.

String

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle

Use Template Text

Whether or not to use a template for the text.

String

Use Word Wrapping

Whether or not to wrap text to fit cleanly on multiple lines.

Toggle

Vertical Alignment

The vertical alignment of the text in the element.

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