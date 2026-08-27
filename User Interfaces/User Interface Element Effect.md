# User Interface Element Effect

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-element-effect/*

---

# User Interface Element Effect

## **User Interface Element Effect**[¶](#user-interface-element-effect "Permanent link")

Effects define conditional visual or value changes on interface elements, such as color shifts, scaling, or visibility toggling based on switches or templates.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Character Model Value Modifier

The character model or image to use as the value modifier for this effect.

[Sprite or Model](../../05-reference/sprite-or-model/)

Color Mask

The color mask to apply to the element.

Color

Easing Function

The easing function that controls how the effect animates over time.

[Easing Function](../../05-reference/easing-function/)

Grayscale

Whether the element renders in grayscale when this effect is active. Overrides the color mask.

Toggle

Hue Shift

The hue shift in degrees to apply to the element when this effect is active.

Number

Invert Condition Value

Whether to invert the condition result, so the effect activates when the condition is false.

Toggle

Is Recycling?

Whether the effect loops continuously after completing its easing function.

Toggle

Name

The name of the effect.

String

Offset

The offset to apply to the element.

Vector

Opacity

The opacity to apply to the element.

Number

Scale

The scale to apply to the element.

Vector

Switch

The switch index used to conditionally activate this effect at runtime.

[Switch](../../05-reference/switch/)

Template

The template property name used to conditionally activate this effect at runtime.

String

Template Value Modifier

The template value modifier to use for the condition.

String

Text Value Modifier

The text value modifier to use for the condition.

String

Use Color Mask

Whether the color mask is applied when this effect is active.

Toggle

Use Effect

Whether this effect is active. Disabled effects are ignored at runtime.

Toggle

Use Global Switch

Whether the switch condition references a global switch instead of a local switch.

Toggle

Use Image or Sprite

Whether or not to use a sprite or image for the value modifier.

Toggle

Use Local Switch

Whether the switch condition references a local switch instead of a global switch.

Toggle

Use Offset

Whether the offset is applied when this effect is active.

Toggle

Use Scale

Whether the scale is applied when this effect is active.

Toggle

Use Switch

Whether this effect is conditionally activated by a switch value.

Toggle

Use Template

Whether or not to use a templated value for the value modifier.

Toggle

Use Template Value

Whether this effect is conditionally activated by a template property value.

Toggle

Use Text

Whether or not to use text for the value modifier.

Toggle

Use Visibility

Whether the visibility override is applied when this effect is active.

Toggle

Visibility

Whether or not the element should be visible.

Toggle

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)