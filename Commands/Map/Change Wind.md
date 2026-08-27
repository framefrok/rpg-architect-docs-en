# Change Wind

*Источник: https://docs.rpg-architect.com/07-commands/11-map/210-change-wind/*

---

# Change Wind

## **Change Wind**[¶](#change-wind "Permanent link")

Modifies the map's wind direction, strength, and gust parameters over a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Direction X

The X component of the wind direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction X Enabled

Whether the wind direction X adjustment is enabled.

Toggle

Direction Y

The Y component of the wind direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Y Enabled

Whether the wind direction Y adjustment is enabled.

Toggle

Direction Z

The Z component of the wind direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Z Enabled

Whether the wind direction Z adjustment is enabled.

Toggle

Duration

The duration to adjust the wind in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Gust Amplitude

The amplitude of wind gusts. 0 is steady wind, 1 is fairly choppy, 2 or more is stormy.

[Variable or Value](../../../05-reference/variable-or-value/)

Gust Amplitude Enabled

Whether the gust amplitude adjustment is enabled.

Toggle

Gust Frequency

How fast wind gusts cycle, in cycles per second.

[Variable or Value](../../../05-reference/variable-or-value/)

Gust Frequency Enabled

Whether the gust frequency adjustment is enabled.

Toggle

Is Enabled

Whether the wind toggle is updated by this command.

Toggle

Is Wind Active

Whether wind is active on the map.

Toggle

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Strength

The strength of the wind, measured in tile scales of sway at full effect.

[Variable or Value](../../../05-reference/variable-or-value/)

Strength Enabled

Whether the wind strength adjustment is enabled.

Toggle

Use As Delta Values

When enabled, adjusts the wind by the specified amount relative to its current value rather than setting it to an absolute value.

Toggle