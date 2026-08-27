# Absolute Movement

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-element/absolute-movement/*

---

# Absolute Movement

## **Absolute Movement**[¶](#absolute-movement "Permanent link")

Absolute Movement elements control battler movement to a fixed position using X, Y, Z coordinates, with optional parabolic pathing.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the element in milliseconds.

Number

Is Relative

Whether the movement is relative to the current position.

Toggle

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

#### **Absolute Movement**[¶](#absolute-movement_1 "Permanent link")

Name

Explanation

Type

Easing Function

The easing curve applied to the movement's progress over the duration.

[Easing Function](../../../../05-reference/easing-function/)

Is Parabolic

Whether the movement should follow a semi-parabolic path.

Toggle

Return to Start

Whether the movement returns the target to their starting position.

Toggle

X

The x component of movement.

Number

Y

The y component of movement.

Number

Z

The z component of movement.

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