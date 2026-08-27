# Target Effect

*Источник: https://docs.rpg-architect.com/09-animations/animation-element/target-effect/*

---

# Target Effect

## **Target Effect**[¶](#target-effect "Permanent link")

Target Effect elements apply color masks and flash effects to the animation target or the entire screen during playback.

> **Note**: This element supports tweening to generate frames.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Name

The name of this animation element. Used for identification in the timeline.

String

#### **Appearance**[¶](#appearance "Permanent link")

Name

Explanation

Type

Color

The color mask applied to the target or screen. Use to tint or darken during the animation frame.

Color

Flash

The flash color overlaid on the target. Use for hit flashes or impact highlights.

Color

Is Screen Effect

Whether to apply the effect to the entire screen instead of the animation target.

Toggle

Is User Interface Included

Whether the screen effect also applies to interface elements. Only relevant when **Is Screen Effect** is enabled.

Toggle