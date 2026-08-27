# Setup Sequences

*Источник: https://docs.rpg-architect.com/11-battles/05-setup-sequences/*

---

# Setup Sequences

## **Setup Sequences**[¶](#setup-sequences "Permanent link")

Setup Sequences define how battlers are visually arranged before and after battle. A Setup Sequence is a list of Setup Elements that execute in order — for example, moving heroes into their starting positions, playing an entrance animation, or scaling enemies into view. Each element type controls a different aspect of the setup.

* * *

#### **Setup Elements**[¶](#setup-elements "Permanent link")

*   [Animation](#animation)
*   [Battle Pose](#battle-pose)
*   [Color Mask](#color-mask)
*   [Move](#move)
*   [Scale](#scale)
*   [Sound Effect](#sound-effect)
*   [Teleport](#teleport)
*   [Wait](#wait)

* * *

## **Animation**[¶](#animation "Permanent link")

Animation elements play a visual animation on a battler or the screen.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Animation**[¶](#animation_1 "Permanent link")

Name

Explanation

Type

Animation

The animation to use in the sequence.

[Animation](../../06-database/08-animations/00-animations/)

Targets Battler

Whether the animation targets the battler.

Toggle

Targets Screen

Whether the animation targets the screen.

Toggle

* * *

## **Battle Pose**[¶](#battle-pose "Permanent link")

Battle Pose elements change the visual pose of a battler.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Battle Pose**[¶](#battle-pose_1 "Permanent link")

Name

Explanation

Type

Battle Pose

The battle pose to set on the target.

[Battle Pose](../../06-database/07-battles/10-battle-poses/)

Is Reset

Whether the battle pose should be reset.

Toggle

* * *

## **Color Mask**[¶](#color-mask "Permanent link")

Color Mask elements apply or transition a color tint on a battler.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Color Mask**[¶](#color-mask_1 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

End

The ending color mask on the target.

Color

Is Instant

Whether the sequence is instantaneous and ignores duration.

Toggle

Start

The starting color mask on the target.

Color

* * *

## **Move**[¶](#move "Permanent link")

Move elements animate a battler's movement to a destination.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Position**[¶](#position "Permanent link")

Name

Explanation

Type

Is Relative

Whether the destination should be treated as an offset to the position.

Toggle

Use Pathfinding

Whether to use pathfinding to reach the destination.

Toggle

Use Slot Position

Whether to use the position specified by the battle slot.

Toggle

X

The x coordinate to move to.

[Variable or Value](../../05-reference/variable-or-value/)

Y

The y coordinate to move to.

[Variable or Value](../../05-reference/variable-or-value/)

Z

The z coordinate to move to.

[Variable or Value](../../05-reference/variable-or-value/)

* * *

## **Scale**[¶](#scale "Permanent link")

Scale elements resize a battler's visual representation.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Scale**[¶](#scale_1 "Permanent link")

Name

Explanation

Type

Easing Function

The easing curve applied between the start and end scale values.

[Easing Function](../../05-reference/easing-function/)

End

The ending scale value. Applied as a multiplier of the battler's current scale when **Is Relative** is enabled, otherwise as an absolute scale.

[Variable or Value](../../05-reference/variable-or-value/)

End X

The ending scale along the X axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

End Y

The ending scale along the Y axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

End Z

The ending scale along the Z axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

Is Component Based

Whether the start and end scale are specified per axis. When disabled, a single uniform scale value is applied to all axes.

Toggle

Is Instant

Whether the element occurs instantly, snapping to the end scale without animating.

Toggle

Is Relative

Whether the start and end values are interpreted as multipliers of the battler's current scale. When disabled, they are absolute scale values.

Toggle

Return to Original

Whether the battler's scale is restored to its original value when the element finishes.

Toggle

Start

The starting scale value. Applied as a multiplier of the battler's current scale when **Is Relative** is enabled, otherwise as an absolute scale.

[Variable or Value](../../05-reference/variable-or-value/)

Start X

The starting scale along the X axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

Start Y

The starting scale along the Y axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

Start Z

The starting scale along the Z axis. Used when **Is Component Based** is enabled.

[Variable or Value](../../05-reference/variable-or-value/)

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Sound Effect**[¶](#sound-effect "Permanent link")

Sound Effect elements play an audio sound effect.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Sound Effect

The sound effect to play.

[Sound Effect](../../05-reference/sound-effect/)

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

* * *

## **Teleport**[¶](#teleport "Permanent link")

Teleport elements instantly move a battler to a new position.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Position**[¶](#position_1 "Permanent link")

Name

Explanation

Type

Is Relative

Whether the destination should be treated as an offset to the position.

Toggle

Use Slot Position

Whether to use the position specified by the battle slot.

Toggle

X

The x coordinate of the teleport.

[Variable or Value](../../05-reference/variable-or-value/)

Y

The y coordinate of the teleport.

[Variable or Value](../../05-reference/variable-or-value/)

Z

The z coordinate of the teleport.

[Variable or Value](../../05-reference/variable-or-value/)

* * *

## **Wait**[¶](#wait "Permanent link")

Wait elements pause the battler setup sequence for a specified duration before continuing.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Start Time (milliseconds)

The time to start the setup element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle