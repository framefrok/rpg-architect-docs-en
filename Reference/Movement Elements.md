# Movement Elements

*Источник: https://docs.rpg-architect.com/05-reference/movement-element/*

---

# Movement Elements

## **Movement Elements**[¶](#movement-elements "Permanent link")

Movement Elements control how [Actors](../actor-reference/) move in a scene, generally configured by a path on an [Entity](../entity/) script page or via the [Move Entity](../../07-commands/12-entity-and-vehicle/10-move-entity/) command.

* * *

#### **Movement Elements**[¶](#movement-elements_1 "Permanent link")

*   [Character Model](#character-model)
*   [Character Shape](#character-shape)
*   [Color Mask](#color-mask)
*   [Face](#face)
*   [Path Find](#path-find)
*   [Relative Step](#relative-step)
*   [Rotate Model Sprite](#rotate-model-sprite)
*   [Scale](#scale)
*   [Shake](#shake)
*   [Sound Effect](#sound-effect)
*   [Step](#step)
*   [Step In Relation](#step-in-relation)
*   [Switch](#switch)
*   [Teleport](#teleport)
*   [Translation](#translation)
*   [Turn](#turn)
*   [Variable](#variable)
*   [Visibility](#visibility)
*   [Wait](#wait)

* * *

## **Character Model**[¶](#character-model "Permanent link")

Character Model elements apply a character model to the target.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Sprite / Model

The character model to apply to the target.

[Sprite or Model](../sprite-or-model/)

* * *

## **Character Shape**[¶](#character-shape "Permanent link")

Character Shape elements apply a sprite shape to the target.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Shape

The shape of the character, if a sprite.

[Sprite Shape](../sprite-format/)

* * *

## **Color Mask**[¶](#color-mask "Permanent link")

Color Mask elements apply a color mask to the target.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the target.

Color

* * *

## **Face**[¶](#face "Permanent link")

Face elements change the direction the target is facing.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Direction

The direction to face.

[Direction](../direction/)

Direction Face

Whether to face in a direction.

Toggle

Face Away From Hero

Whether the actor should face away from the hero.

Toggle

Face Backward

Whether the actor should face backwards.

Toggle

Face Random

Whether to face a random direction.

Toggle

Face Toward Hero

Whether the actor should face toward the hero.

Toggle

Face Variable Direction

Whether the actor should face a variable direction.

Toggle

Variable Direction

The variable representation of the direction.

[Variable or Value](../variable-or-value/)

* * *

## **Path Find**[¶](#path-find "Permanent link")

Path Find elements move the target to a location using pathfinding.

> **Note**: An Edit button is available to configure the X, Y, and Z coordinates.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

X

The location's X component.

[Variable or Value](../variable-or-value/)

Y

The location's Y component.

[Variable or Value](../variable-or-value/)

Z

The location's Z component.

[Variable or Value](../variable-or-value/)

* * *

## **Relative Step**[¶](#relative-step "Permanent link")

Relative Step elements move the target by a fractional offset along each axis.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

X Step Factor

The step factor for the X axis.

[Variable or Value](../variable-or-value/)

Y Step Factor

The step factor for the Y axis.

[Variable or Value](../variable-or-value/)

Z Step Factor

The step factor for the Z axis.

[Variable or Value](../variable-or-value/)

* * *

## **Rotate Model Sprite**[¶](#rotate-model-sprite "Permanent link")

Rotate Model Sprite elements rotate the target's model or sprite over time.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration of the rotation.

Number

Pitch (X Rotation)

The pitch in degrees, if valid.

Number

Relative Rotation

Whether the rotation is relative to the current value.

Toggle

Roll (Z Rotation)

The roll in degrees, if valid.

Number

Yaw (Y Rotation)

The yaw in degrees, if valid.

Number

* * *

## **Scale**[¶](#scale "Permanent link")

Scale elements change the size of the target.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

X

The scale's X component.

[Variable or Value](../variable-or-value/)

Y

The scale's Y component.

[Variable or Value](../variable-or-value/)

Z

The scale's Z component.

[Variable or Value](../variable-or-value/)

* * *

## **Shake**[¶](#shake "Permanent link")

Shake elements apply a shake effect to the target for a duration.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Duration

The duration of the element in milliseconds.

[Variable or Value](../variable-or-value/)

X

The shake's X component.

[Variable or Value](../variable-or-value/)

Y

The shake's Y component.

[Variable or Value](../variable-or-value/)

Z

The shake's Z component.

[Variable or Value](../variable-or-value/)

* * *

## **Sound Effect**[¶](#sound-effect "Permanent link")

Sound Effect elements play a sound effect.

## **Properties**[¶](#properties_9 "Permanent link")

#### **System**[¶](#system_9 "Permanent link")

Name

Explanation

Type

Sound

The sound effect to play.

[Sound Effect](../sound-effect/)

* * *

## **Step**[¶](#step "Permanent link")

Step elements move the target one tile in a direction.

## **Properties**[¶](#properties_10 "Permanent link")

#### **System**[¶](#system_10 "Permanent link")

Name

Explanation

Type

Direction

The direction to step.

[Direction](../direction/)

Direction Step

Whether the step is a directional step.

Toggle

Step Away From Hero

Whether the step is away from the hero.

Toggle

Step Backward

Whether the step is backward.

Toggle

Step Factor

The step amount to move.

Number

Step Forward

Whether the step is forward.

Toggle

Step Random

Whether the step is random.

Toggle

Step Toward Hero

Whether the step is toward the hero.

Toggle

Step Vertical Only

Whether the step is vertical only.

Toggle

#### **Optional Details**[¶](#optional-details "Permanent link")

Name

Explanation

Type

Ascend

Whether the step is ascending.

Toggle

Descend

Whether the step is descending.

Toggle

Random Ascent or Descent

Whether to include ascent/descent operations in random.

Toggle

* * *

## **Step In Relation**[¶](#step-in-relation "Permanent link")

Step In Relation elements move the target toward or away from another actor.

## **Properties**[¶](#properties_11 "Permanent link")

#### **System**[¶](#system_11 "Permanent link")

Name

Explanation

Type

Step Away

Whether the step is away.

Toggle

Step Factor

The step amount to move.

Number

Step Toward

Whether the step is forward.

Toggle

Target

The target to move in relation to.

[Actor Reference](../actor-reference/)

* * *

## **Switch**[¶](#switch "Permanent link")

Switch elements set a global or local switch value.

## **Properties**[¶](#properties_12 "Permanent link")

#### **System**[¶](#system_12 "Permanent link")

Name

Explanation

Type

Switch

The switch operation to execute.

[Switch](../switch/)

* * *

## **Teleport**[¶](#teleport "Permanent link")

Teleport elements instantly move the target to a specific location.

> **Note**: An Edit button is available to configure the X, Y, and Z coordinates.

## **Properties**[¶](#properties_13 "Permanent link")

#### **System**[¶](#system_13 "Permanent link")

Name

Explanation

Type

Include X

Whether to use the X component when teleporting.

Toggle

Include Y

Whether to use the Y component when teleporting.

Toggle

Include Z

Whether to use the Z component when teleporting.

Toggle

X

The location's X component.

[Variable or Value](../variable-or-value/)

Y

The location's Y component.

[Variable or Value](../variable-or-value/)

Z

The location's Z component.

[Variable or Value](../variable-or-value/)

* * *

## **Translation**[¶](#translation "Permanent link")

Translation elements offset the target's visual position.

## **Properties**[¶](#properties_14 "Permanent link")

#### **System**[¶](#system_14 "Permanent link")

Name

Explanation

Type

Is Absolute

Whether the translation is set to an absolute value.

Toggle

Is Relative

Whether the translation is set to alter the current translation by a delta.

Toggle

X

The translation on the X axis.

[Variable or Value](../variable-or-value/)

Y

The translation on the Y axis.

[Variable or Value](../variable-or-value/)

Z

The translation on the Z axis.

[Variable or Value](../variable-or-value/)

* * *

## **Turn**[¶](#turn "Permanent link")

Turn elements rotate the target's facing direction clockwise or counter-clockwise.

## **Properties**[¶](#properties_15 "Permanent link")

#### **System**[¶](#system_15 "Permanent link")

Name

Explanation

Type

Clockwise

Whether the rotation is clockwise.

Toggle

Turn Factor

The amount to turn.

Number

* * *

## **Variable**[¶](#variable "Permanent link")

Variable elements modify a global or local variable value.

## **Properties**[¶](#properties_16 "Permanent link")

#### **System**[¶](#system_16 "Permanent link")

Name

Explanation

Type

Variable

The variable operation to execute.

[Variable](../variable/)

* * *

## **Visibility**[¶](#visibility "Permanent link")

Visibility elements toggle whether the target is visible.

## **Properties**[¶](#properties_17 "Permanent link")

#### **System**[¶](#system_17 "Permanent link")

Name

Explanation

Type

Is Visible

Whether the entity should be visible.

[Switch or Value](../switch-or-value/)

* * *

## **Wait**[¶](#wait "Permanent link")

Wait elements pause the movement path for a duration.

## **Properties**[¶](#properties_18 "Permanent link")

#### **System**[¶](#system_18 "Permanent link")

Name

Explanation

Type

Wait Time (milliseconds)

The time to wait.

[Variable or Value](../variable-or-value/)