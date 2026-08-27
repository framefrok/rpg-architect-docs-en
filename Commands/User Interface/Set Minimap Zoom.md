# Set Minimap Zoom

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/44-set-minimap-zoom/*

---

# Set Minimap Zoom

## **Set Minimap Zoom**[¶](#set-minimap-zoom "Permanent link")

Adjusts the minimap's zoom over a specified duration, optionally by a relative amount and asynchronously.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration to adjust the zoom in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Minimap

The minimap user interface to target. Leave as Default to use the first minimap user interface, or provide a unique ID through a variable.

[Variable or Value](../../../05-reference/variable-or-value/)

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Use As Delta Value

When enabled, adjusts the zoom by the specified amount relative to its current value rather than setting it to an absolute value.

Toggle

Zoom

The zoom factor to apply to the minimap. Higher values show a smaller, more zoomed-in area.

[Variable or Value](../../../05-reference/variable-or-value/)