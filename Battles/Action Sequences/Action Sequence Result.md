# Action Sequence Result

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-result/*

---

# Action Sequence Result

## **Action Sequence Result**[¶](#action-sequence-result "Permanent link")

Action Sequence Results define the visual presentation of battle action results, such as damage numbers, healing values, and status messages that appear on screen during an Action Sequence.

> **Note**: Action Sequence Results control how results are rendered visually using a [Font](../../../05-reference/font/) and one or more [Annotation Effects](../../../05-reference/annotation-effect/). Annotation Effects determine the motion, fade, scale, and color behavior of the result text as it animates on screen. This is distinct from the [Battle Action Result](../battle-action-result/), which represents the underlying data of what happened (e.g. the statistic changed, the status effect applied). The Action Sequence Result is responsible for turning that data into something the player sees.

## **Properties**[¶](#properties "Permanent link")

#### **Appearance**[¶](#appearance "Permanent link")

Name

Explanation

Type

Effects

The annotation effects applied to the result text, such as movement, fading, and scaling.

[Annotation Effect](../../../05-reference/annotation-effect/)

Font

The font used to display the action result text.

[Font](../../../05-reference/font/)