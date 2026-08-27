# Rotate Object

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/15-rotate-object/*

---

# Rotate Object

## **Rotate Object**[¶](#rotate-object "Permanent link")

Sets a rotational value on a model or rendered sprite over a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration to rotate the object over in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Run Asynchronously

Whether the rotation runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Target

The rendered physics object to rotate.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Use As Delta Values

Whether the rotation values are relative to the current rotation instead of absolute.

Toggle

X

The rotation value for the X (pitch) axis in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

X (Pitch)

Whether the X (pitch) rotation axis is enabled.

Toggle

Y

The rotation value for the Y (yaw) axis in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Y (Yaw)

Whether the Y (yaw) rotation axis is enabled.

Toggle

Z

The rotation value for the Z (roll) axis in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Z (Roll)

Whether the Z (roll) rotation axis is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Rotate an Entity on X and Y Axes Over One Second**[¶](#rotate-an-entity-on-x-and-y-axes-over-one-second "Permanent link")

Rotates entity 0 to 45 degrees on the X axis and 90 degrees on the Y axis over 1000 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-0-1)rotate_object(entity(0), duration: 1000, x: 45, y: 90);`

`[](#__codelineno-1-1){"Data":{"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsAbsolute":1,"IsAsynchronousOperation":0,"IsRelative":0,"IsXEnabled":1,"IsYEnabled":1,"IsZEnabled":0,"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"90","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.RotateObjectCommand"}`

#### **Rotate a Doodad Relative to Current Rotation Asynchronously**[¶](#rotate-a-doodad-relative-to-current-rotation-asynchronously "Permanent link")

Rotates doodad 0 by 45 degrees on the X axis relative to its current rotation without blocking subsequent commands.

Code ScriptVisual Script

`[](#__codelineno-2-1)rotate_object(doodad(0), x: 45, relative, async);`

`[](#__codelineno-3-1){"Data":{"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsAbsolute":0,"IsAsynchronousOperation":1,"IsRelative":1,"IsXEnabled":1,"IsYEnabled":0,"IsZEnabled":0,"Target":{"IsDoodad":1,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.RotateObjectCommand"}`