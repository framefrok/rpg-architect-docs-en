# Folder

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element/folder/*

---

# Folder

## **Folder**[¶](#folder "Permanent link")

Folder elements organize child [User Interface Elements](../) hierarchically without rendering or interaction in the engine.

> **Note**: Folders do not create an actual element in the engine and are only used for organization inside the editor.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Children

The child elements inside the folder.

[User Interface Element](../)

Disabled Effects

The visual effects applied when this element is disabled.

[User Interface Element Effect](../../user-interface-element-effect/)

Focused Effects

The visual effects applied when this element has focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Is Expanded

Whether or not the folder is expanded.

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

Template Type

The data type expected when this element is used with templated data binding.

String

Unfocused Effects

The visual effects applied when this element loses focus.

[User Interface Element Effect](../../user-interface-element-effect/)

Use Relative Positioning

Whether to use screen-relative coordinates (0.0 to 1.0) instead of pixel coordinates for positioning and sizing.

Toggle