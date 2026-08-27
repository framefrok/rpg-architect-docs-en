# Adjust Fog

*Источник: https://docs.rpg-architect.com/07-commands/11-map/115-adjust-fog/*

---

# Adjust Fog

## **Adjust Fog**[¶](#adjust-fog "Permanent link")

Modifies the scene's fog color, distances, height falloff, on/off state, and render distance over a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Enabled

Whether the fog color adjustment is applied.

Toggle

Duration

The duration in milliseconds over which the fog adjustment ramps. A value of zero applies the change instantly.

[Variable or Value](../../../05-reference/variable-or-value/)

End Enabled

Whether the fog end adjustment is applied.

Toggle

Fog Color

The color of the fog. When ramped, the color interpolates from its current value.

Color

Fog End

The distance at which the fog fully obscures the scene, relative to the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Fog Start

The distance at which the fog begins, relative to the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Fog Visibility

Whether the fog is visible. This is applied instantly and is not ramped.

[Switch or Value](../../../05-reference/switch-or-value/)

Height Falloff

The rate at which the fog falls off with height.

[Variable or Value](../../../05-reference/variable-or-value/)

Height Falloff Enabled

Whether the fog height falloff adjustment is applied.

Toggle

Height Start

The height at which the fog begins.

[Variable or Value](../../../05-reference/variable-or-value/)

Height Start Enabled

Whether the fog height start adjustment is applied.

Toggle

Render Distance

The distance at which geometry stops rendering, relative to the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Render Distance Enabled

Whether the render distance adjustment is applied.

Toggle

Reset to Default

When enabled, resets all fog values to the map and core parameter defaults, overriding the individual property adjustments. Still honors the duration to ramp toward the defaults.

Toggle

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting for the ramp to finish.

Toggle

Start Enabled

Whether the fog start adjustment is applied.

Toggle

Use As Delta Values

When enabled, adjusts the numeric fog values by the specified amount relative to their current values rather than setting them to absolute values. Does not apply to color or visibility.

Toggle

Visibility Enabled

Whether the fog visibility adjustment is applied.

Toggle