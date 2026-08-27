# Shake Screen

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/20-shake-screen/*

---

# Shake Screen

## **Shake Screen**[¶](#shake-screen "Permanent link")

Shakes the camera with configurable intensity on each axis for a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration (milliseconds)

The duration to shake the screen in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Run Asynchronously

Whether the shake runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

X

The shake intensity on the X axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The shake intensity on the Y axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The shake intensity on the Z axis.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Shake Screen on the X and Y Axes**[¶](#shake-screen-on-the-x-and-y-axes "Permanent link")

Shakes the screen for 1000 milliseconds with intensity 5 on both the X and Y axes.

Code ScriptVisual Script

`[](#__codelineno-0-1)shake_screen(1000, x: 5, y: 5);`

`[](#__codelineno-1-1){"Data":{"IsAsynchronousOperation":0,"ShakeDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.ShakeScreenCommand"}`

#### **Shake Screen Asynchronously on All Axes**[¶](#shake-screen-asynchronously-on-all-axes "Permanent link")

Shakes the screen for 1000 milliseconds on all three axes without blocking subsequent commands.

Code ScriptVisual Script

`[](#__codelineno-2-1)shake_screen(1000, x: 5, y: 5, z: 3, async);`

`[](#__codelineno-3-1){"Data":{"IsAsynchronousOperation":1,"ShakeDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.ShakeScreenCommand"}`