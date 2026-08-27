# Jump

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/15-jump/*

---

# Jump

## **Jump**[¶](#jump "Permanent link")

Makes an actor or entity jump with a specified velocity and duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration of the jumping force in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Fine Control Switch

The switch that controls whether the jump can be exited early for fine height control.

[Switch or Value](../../../05-reference/switch-or-value/)

Is Animated

Whether to apply a visual translation animation to the target during the jump.

Toggle

Is Fine Control Allowed

Whether fine control is allowed, enabling early exit from the jump via a switch.

Toggle

Is Parabolic Animation

Whether the jump animation follows a parabolic arc.

Toggle

Target

The actor or entity that will jump.

[Actor Reference](../../../05-reference/actor-reference/)

Translation X

The visual translation offset along the X axis during the jump animation.

[Variable or Value](../../../05-reference/variable-or-value/)

Translation Y

The visual translation offset along the Y axis during the jump animation.

[Variable or Value](../../../05-reference/variable-or-value/)

Translation Z

The visual translation offset along the Z axis during the jump animation.

[Variable or Value](../../../05-reference/variable-or-value/)

Velocity X

The velocity of the jump along the X axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Velocity Y

The velocity of the jump along the Y axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Velocity Z

The velocity of the jump along the Z axis.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Make the Calling Entity Jump Upward Over 500 Milliseconds**[¶](#make-the-calling-entity-jump-upward-over-500-milliseconds "Permanent link")

This makes the calling entity jump with a vertical velocity of 1 over 500 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-0-1)jump(self, 0, 1, 0, 500);`

`[](#__codelineno-1-1){"Data":{"AnimationTranslationX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"AnimationTranslationY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"AnimationTranslationZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"FineControlSwitch":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsAnimated":0,"IsFineControlAllowed":0,"IsParabolicAnimation":0,"IsReadyForPhysicsLoop":0,"JumpVelocityX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"JumpVelocityY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"JumpVelocityZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityJumpCommand"}`

#### **Jump with Parabolic Animation Translation**[¶](#jump-with-parabolic-animation-translation "Permanent link")

This makes the calling entity jump with animation offsets and parabolic interpolation over 500 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-2-1)jump(self, 0, 1, 0, 500, anim_x: 5, anim_y: 10, anim_z: 0, parabolic);`

`[](#__codelineno-3-1){"Data":{"AnimationTranslationX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"AnimationTranslationY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"AnimationTranslationZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"FineControlSwitch":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsAnimated":1,"IsFineControlAllowed":0,"IsParabolicAnimation":1,"IsReadyForPhysicsLoop":0,"JumpVelocityX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"JumpVelocityY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"JumpVelocityZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityJumpCommand"}`