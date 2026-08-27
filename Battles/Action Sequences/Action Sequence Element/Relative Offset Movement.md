# Relative Offset Movement

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-element/relative-offset-movement/*

---

# Relative Offset Movement

## **Relative Offset Movement**[¶](#relative-offset-movement "Permanent link")

Relative Offset Movement elements move a battler to a position offset from the opposing battler, with optional parabolic pathing.

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

#### **Offset from Target**[¶](#offset-from-target "Permanent link")

Name

Explanation

Type

Easing Function

The easing curve applied to the movement's progress over the duration.

[Easing Function](../../../../05-reference/easing-function/)

From Center of Targets

Whether to include the center of the target, rather than just the space around.

Toggle

Is Parabolic Movement

Whether the movement should follow a semi-parabolic path.

Toggle

Offset from Target X

The distance to move along X.

Number

Offset from Target Y

The distance to move along Y.

Number

Offset from Target Z

The distance to move along Z.

Number

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

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../../../04-editor/easing-function-editor/)