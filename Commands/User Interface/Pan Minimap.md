# Pan Minimap

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/45-pan-minimap/*

---

# Pan Minimap

## **Pan Minimap**[¶](#pan-minimap "Permanent link")

Pans the minimap away from the followed position over a specified duration, or resets it back to the player. Offsets are in tiles.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration to pan the minimap in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Minimap

The minimap user interface to target. Leave as Default to use the first minimap user interface, or provide a unique ID through a variable.

[Variable or Value](../../../05-reference/variable-or-value/)

Reset

Whether to pan the minimap back to the followed position, clearing any offset.

Toggle

Run Asynchronously

Whether the pan runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Use As Delta Values

When enabled, pans by the specified amount relative to the current offset rather than setting it to an absolute value.

Toggle

X

The horizontal pan offset in tiles.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

Whether the X offset is applied.

Toggle

Y

The vertical pan offset in tiles.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

Whether the Y offset is applied.

Toggle