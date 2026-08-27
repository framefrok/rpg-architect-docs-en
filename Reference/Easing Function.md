# Easing Function

*Источник: https://docs.rpg-architect.com/05-reference/easing-function/*

---

# Easing Function

## **Easing Function**[¶](#easing-function "Permanent link")

An easing function is a mathematical rule that describes how change occurs over time. In practice, it generally is used to control things such as opacity or positioning, such that something may slowly or rapidly fade in/out or bounce into view.

RPG Architect supports many easing functions that can be used with [Scene Transitions](../scene-transition/), user interfaces, commands, and more. These easing functions include simple linear to complex multi-parametric calculations.

> **Note**: A user interface may use a bounce easing function to fall into place with a gentle recoil on land.
> 
> **Note**: A screen transition may leverage an exponential easing function to gradually, and then sharply, adjust how quick a fade-in occurs.

* * *

#### **Easing Functions**[¶](#easing-functions "Permanent link")

*   [Bounce](#bounce)
*   [Circular](#circular)
*   [Elastic](#elastic)
*   [Exponential](#exponential)
*   [Instant](#instant)
*   [Linear](#linear)
*   [Sinusoidal](#sinusoidal)

* * *

## **Bounce**[¶](#bounce "Permanent link")

Bounce easing functions simulate a bouncing ball, controlled by gravity, elasticity, and bounce count.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Bounces

The number of bounces to perform during the easing duration.

Number

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Elasticity

The elasticity factor for each bounce, from 0 (no rebound) to 1 (full rebound).

Number

Gravity

The gravity affecting the bounce. Higher values produce sharper drops between bounces.

Number

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Circular**[¶](#circular "Permanent link")

Circular easing functions accelerate, decelerate, or both using a circular curve.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Mode

The easing mode that controls whether the function accelerates in, decelerates out, or both.

Circular Easing Mode

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Elastic**[¶](#elastic "Permanent link")

Elastic easing functions simulate a spring oscillation, controlled by amplitude and frequency.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Amplitude

The amplitude of the spring oscillation. Higher values produce larger overshoots.

Number

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Frequency

The frequency of the spring oscillation. Higher values produce more rapid bounces.

Number

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Exponential**[¶](#exponential "Permanent link")

Exponential easing functions curve the rate of change using an exponent, producing acceleration or deceleration.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Exponent

The exponent that controls the steepness of the curve. Higher values produce sharper acceleration.

Number

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Instant**[¶](#instant "Permanent link")

Instant easing functions complete immediately with no interpolation, jumping directly to the target value.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Linear**[¶](#linear "Permanent link")

Linear easing functions interpolate at a constant rate from start to finish, producing uniform motion.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Reverse

Whether to reverse the easing function.

Toggle

* * *

## **Sinusoidal**[¶](#sinusoidal "Permanent link")

Sinusoidal easing functions accelerate, decelerate, or both using a sine curve, producing smooth wave-like motion.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the easing function in milliseconds.

Number

Mode

The easing mode that controls whether the function accelerates in, decelerates out, or both.

Sine Easing Mode

Reverse

Whether to reverse the easing function.

Toggle