# Adjust Background Effect

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/12-adjust-background-effect/*

---

# Adjust Background Effect

## **Adjust Background Effect**[¶](#adjust-background-effect "Permanent link")

Adjusts the volume, pan, pitch, or looping of one or all running background effects, optionally ramping over a duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Adjust All

When enabled, all active background effects are adjusted.

Toggle

Duration (milliseconds)

The duration in milliseconds over which the adjustment ramps. A value of zero applies the change instantly.

[Variable or Value](../../../05-reference/variable-or-value/)

Looping

Whether the adjusted background effects loop continuously.

[Switch or Value](../../../05-reference/switch-or-value/)

Looping Enabled

Whether the looping adjustment is applied.

Toggle

Pan

The stereo panning value to adjust to. Ranges from -1 (left) to 1 (right).

[Variable or Value](../../../05-reference/variable-or-value/)

Pan Enabled

Whether the pan adjustment is applied.

Toggle

Pitch

The pitch value to adjust to. Ranges from -1 to 1.

[Variable or Value](../../../05-reference/variable-or-value/)

Pitch Enabled

Whether the pitch adjustment is applied.

Toggle

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting for the ramp to finish.

Toggle

Unique ID

The unique ID of the specific background effect instance to adjust.

[Variable or Value](../../../05-reference/variable-or-value/)

Use As Delta Values

When enabled, adjusts each property by the specified amount relative to its current value rather than setting it to an absolute value.

Toggle

Volume

The volume to adjust to. Ranges from 0 (silent) to 1 (full volume).

[Variable or Value](../../../05-reference/variable-or-value/)

Volume Enabled

Whether the volume adjustment is applied.

Toggle