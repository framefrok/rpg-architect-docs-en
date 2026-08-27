# Hide Screen

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/51-hide-screen/*

---

# Hide Screen

## **Hide Screen**[¶](#hide-screen "Permanent link")

Hide the screen using a specified transition effect.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Asynchronous Transition

Whether the transition runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Render Scene

Whether the scene should continue to be rendered after hiding.

Toggle

Render User Interface

Whether the user interface should continue to be rendered after hiding.

Toggle

Transition

The transition effect to use when hiding the screen.

[Scene Transition](../../../05-reference/scene-transition/)

## **Examples**[¶](#examples "Permanent link")

#### **Hide Screen with a Fade Out Transition**[¶](#hide-screen-with-a-fade-out-transition "Permanent link")

Hides the screen using a fade-out transition over 1000 milliseconds with a black color.

Code ScriptVisual Script

`[](#__codelineno-0-1)hide_screen(fade_out(linear(1000), #000000));`

`[](#__codelineno-1-1){"Data":{"IsAsynchronousTransition":0,"IsRenderingScene":0,"IsRenderingUserInterface":0,"Transition":{"$":"FadeOutSceneTransition","Color":"0,0,0,1","BlendMode":0,"Duration":"00:00:01","EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.HideScreenCommand"}`

#### **Hide Screen Instantly**[¶](#hide-screen-instantly "Permanent link")

Hides the screen immediately without any transition effect.

Code ScriptVisual Script

`[](#__codelineno-2-1)hide_screen(instant);`

`[](#__codelineno-3-1){"Data":{"IsAsynchronousTransition":0,"IsRenderingScene":0,"IsRenderingUserInterface":0,"Transition":{"$":"InstantSceneTransition","Duration":"00:00:00","BlendMode":0,"EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.HideScreenCommand"}`

#### **Hide Screen Asynchronously While Continuing to Render the Scene**[¶](#hide-screen-asynchronously-while-continuing-to-render-the-scene "Permanent link")

Fades out the screen asynchronously while keeping the scene rendering active behind the transition.

Code ScriptVisual Script

`[](#__codelineno-4-1)hide_screen(fade_out(linear(1000), #000000), async, render_scene);`

`[](#__codelineno-5-1){"Data":{"IsAsynchronousTransition":1,"IsRenderingScene":1,"IsRenderingUserInterface":0,"Transition":{"$":"FadeOutSceneTransition","Color":"0,0,0,1","BlendMode":0,"Duration":"00:00:01","EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.HideScreenCommand"}`

## **See Also**[¶](#see-also "Permanent link")

*   [Transition Editor](../../../04-editor/transition-editor/)