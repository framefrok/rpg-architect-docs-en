# Alter Gravity

*Источник: https://docs.rpg-architect.com/07-commands/10-physics/10-alter-gravity/*

---

# Alter Gravity

## **Alter Gravity**[¶](#alter-gravity "Permanent link")

Changes the gravity vector for the current scene, affecting all physics objects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

X

The X component of the gravity vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y component of the gravity vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z component of the gravity vector.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Standard Downward Gravity**[¶](#set-standard-downward-gravity "Permanent link")

Sets the scene gravity to a standard downward force of -9.8 on the Y axis.

Code ScriptVisual Script

`[](#__codelineno-0-1)alter_gravity(0, -9.8, 0);`

`[](#__codelineno-1-1){"Data":{"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-9.8","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterGravityCommand"}`

#### **Disable Gravity**[¶](#disable-gravity "Permanent link")

Sets the scene gravity to zero on all axes, creating a zero-gravity environment.

Code ScriptVisual Script

`[](#__codelineno-2-1)alter_gravity(0, 0, 0);`

`[](#__codelineno-3-1){"Data":{"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterGravityCommand"}`

#### **Set Gravity from Variables**[¶](#set-gravity-from-variables "Permanent link")

Sets the scene gravity using values from global variables for each axis.

Code ScriptVisual Script

`[](#__codelineno-4-1)alter_gravity($gv[0], $gv[1], $gv[2]);`

`[](#__codelineno-5-1){"Data":{"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Z":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterGravityCommand"}`