# Scale

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-element/scale/*

---

# Scale

## **Scale**[¶](#scale "Permanent link")

Scale elements animate the size of the user or target battler over a duration. Start and end values can be applied as multipliers of the battler's current scale (relative) or as absolute scale values.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Start Time (milliseconds)

The time to start the sequence element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Scale**[¶](#scale_1 "Permanent link")

Name

Explanation

Type

Apply to All

Whether the element applies to the entire group of Users or Targets.

Toggle

Apply to Target

Whether the scale applies to the target.

Toggle

Apply to User

Whether the scale applies to the user.

Toggle

Easing Function

The easing curve applied between the start and end scale values.

[Easing Function](../../../../05-reference/easing-function/)

End

The ending scale value. Applied as a multiplier of the battler's current scale when **Is Relative** is enabled, otherwise as an absolute scale.

Number

End X

The ending scale along the X axis. Used when **Is Component Based** is enabled.

Number

End Y

The ending scale along the Y axis. Used when **Is Component Based** is enabled.

Number

End Z

The ending scale along the Z axis. Used when **Is Component Based** is enabled.

Number

Is Component Based

Whether the start and end scale are specified per axis. When disabled, a single uniform scale value is applied to all axes.

Toggle

Is Instant

Whether the action occurs instantly, snapping to the end scale without animating.

Toggle

Is Relative

Whether the start and end values are interpreted as multipliers of the battler's current scale. When disabled, they are absolute scale values.

Toggle

Return to Original

Whether the battler's scale is restored to its original value when the element finishes.

Toggle

Start

The starting scale value. Applied as a multiplier of the battler's current scale when **Is Relative** is enabled, otherwise as an absolute scale.

Number

Start X

The starting scale along the X axis. Used when **Is Component Based** is enabled.

Number

Start Y

The starting scale along the Y axis. Used when **Is Component Based** is enabled.

Number

Start Z

The starting scale along the Z axis. Used when **Is Component Based** is enabled.

Number

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../../../04-editor/easing-function-editor/)