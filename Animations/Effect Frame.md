# Effect Frame

*Источник: https://docs.rpg-architect.com/09-animations/animation-element/effect-frame/*

---

# Effect Frame

## **Effect Frame**[¶](#effect-frame "Permanent link")

Effect Frame elements display damage numbers, healing, and other battle results on specific animation frames.

> **Note**: Works in tandem with Action Sequences to determine when and where results appear.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Is Target Result

Whether the result frame displays effects on the target of the action.

Toggle

Is User Result

Whether the result frame displays effects on the user performing the action.

Toggle

Name

The name of this animation element. Used for identification in the timeline.

String

#### **Appearance**[¶](#appearance "Permanent link")

Name

Explanation

Type

Color Mask

The color mask applied to the result text. Use to tint damage numbers or healing values.

Color

Font Family

The font family used to render result text. Only applies when **Use Custom Font Family** is enabled.

[Font](../../../05-reference/font/)

Font Size

The font size for result text. Leave empty to use the default size.

Number

Use Custom Font Family

Whether to use a custom font family for result text instead of the default.

Toggle