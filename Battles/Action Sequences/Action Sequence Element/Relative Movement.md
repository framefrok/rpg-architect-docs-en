# Relative Movement

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-element/relative-movement/*

---

# Relative Movement

## **Relative Movement**[¶](#relative-movement "Permanent link")

Relative Movement elements move a battler toward or away from the opposing battler, with optional parabolic pathing.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Is Target Movement

Whether the movement applies to the target of the battle action.

Toggle

Is User Movement

Whether the movement applies to the user of the battle action.

Toggle

Start Time (milliseconds)

The time to start the sequence element at in milliseconds.

Number

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **Parabolic Factor**[¶](#parabolic-factor "Permanent link")

Name

Explanation

Type

Parabolic Factor X

The maximum X that can be used in parabolic movement.

Number

Parabolic Factor Y

The maximum Y that can be used in parabolic movement.

Number

Parabolic Factor Z

The maximum Z that can be used in parabolic movement.

Number

#### **Relative Movement**[¶](#relative-movement_1 "Permanent link")

Name

Explanation

Type

Distance

The distance to move on all planes, if **Is Distance Oriented**.

Number

Distance X

The distance to move along X, if **Is Distance Oriented** is false.

Number

Distance Y

The distance to move along Y, if **Is Distance Oriented** is false.

Number

Distance Z

The distance to move along Z, if **Is Distance Oriented** is false.

Number

Easing Function

The easing curve applied to the movement's progress over the duration.

[Easing Function](../../../../05-reference/easing-function/)

From Center of Targets

Whether to include the center of the target, rather than just the space around.

Toggle

Is Distance Oriented

Whether the movement is done in regard to the overall distance, or components of X/Y/Z.

Toggle

Is Parabolic Movement

Whether the movement should follow a semi-parabolic path.

Toggle

Return to Start

Whether the movement returns the target to their starting position.

Toggle

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../../../04-editor/easing-function-editor/)