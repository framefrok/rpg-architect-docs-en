# Tint Screen

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/20-tint-screen/*

---

# Tint Screen

## **Tint Screen**[¶](#tint-screen "Permanent link")

Applies or remove a color tint on the screen using an easing function.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color

The color to tint the screen with.

Color

Easing Function

The easing function that controls the tint transition over time.

[Easing Function](../../../05-reference/easing-function/)

Enable Tint

Whether to apply a tint to the screen. When disabled, the tint is removed.

Toggle

Run Asynchronously

Whether the tint runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Tint Screen Red with a Linear Transition**[¶](#tint-screen-red-with-a-linear-transition "Permanent link")

Applies a red tint to the screen over 1000 milliseconds using a linear easing function.

Code ScriptVisual Script

`[](#__codelineno-0-1)tint_screen(#FF0000, linear(1000));`

`[](#__codelineno-1-1){"Data":{"EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronousOperation":0,"IsTinting":1,"TintColor":"1,0,0,1","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.TintScreenCommand"}`

#### **Remove Screen Tint with a Linear Transition**[¶](#remove-screen-tint-with-a-linear-transition "Permanent link")

Removes the screen tint over 500 milliseconds using a linear easing function.

Code ScriptVisual Script

`[](#__codelineno-2-1)tint_screen(reset, linear(500));`

`[](#__codelineno-3-1){"Data":{"EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:00.5000000","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronousOperation":0,"IsTinting":0,"TintColor":"0,0,0,0","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.TintScreenCommand"}`

#### **Tint Screen Asynchronously with a Bounce Effect**[¶](#tint-screen-asynchronously-with-a-bounce-effect "Permanent link")

Applies a red tint using a bounce easing function over 2000 milliseconds without blocking subsequent commands.

Code ScriptVisual Script

`[](#__codelineno-4-1)tint_screen(#FF0000, bounce(2000), async);`

`[](#__codelineno-5-1){"Data":{"EasingFunction":{"$":"BounceEasingFunction","Bounces":3,"Elasticity":0.5,"Gravity":1.5,"Name":"Bounce","Duration":"00:00:02","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronousOperation":1,"IsTinting":1,"TintColor":"1,0,0,1","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.TintScreenCommand"}`

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../../04-editor/easing-function-editor/)