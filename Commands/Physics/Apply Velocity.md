# Apply Velocity

*Источник: https://docs.rpg-architect.com/07-commands/10-physics/00-apply-velocity/*

---

# Apply Velocity

## **Apply Velocity**[¶](#apply-velocity "Permanent link")

Applies an instantaneous velocity impulse to a physics object in the specified X, Y, and Z directions.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Target

The physics object to target with this command.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Use As Delta Values

When enabled, the specified values are added to the velocity already applied this frame. When disabled, the specified values replace it.

Toggle

X

The X component of the velocity to apply.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y component of the velocity to apply.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z component of the velocity to apply.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Apply Upward Velocity to an Entity**[¶](#apply-upward-velocity-to-an-entity "Permanent link")

Applies an upward velocity impulse of 5 units to entity 0 along the Y axis.

Code ScriptVisual Script

`[](#__codelineno-0-1)apply_velocity(entity(0), 0, 5, 0);`

`[](#__codelineno-1-1){"Data":{"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.ApplyVelocityCommand"}`

#### **Apply Velocity from Variables**[¶](#apply-velocity-from-variables "Permanent link")

Applies a velocity impulse to entity 0 using values from global variables for each axis.

Code ScriptVisual Script

`[](#__codelineno-2-1)apply_velocity(entity(0), $gv[0], $gv[1], $gv[2]);`

`[](#__codelineno-3-1){"Data":{"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Z":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.ApplyVelocityCommand"}`

#### **Apply Velocity to a Doodad**[¶](#apply-velocity-to-a-doodad "Permanent link")

Applies a forward velocity impulse of 3 units to doodad 0 along the Z axis.

Code ScriptVisual Script

`[](#__codelineno-4-1)apply_velocity(doodad(0), 0, 0, 3);`

`[](#__codelineno-5-1){"Data":{"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":1,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.ApplyVelocityCommand"}`