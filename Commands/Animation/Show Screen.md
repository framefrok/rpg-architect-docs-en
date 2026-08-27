# Show Screen

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/50-show-screen/*

---

# Show Screen

## **Show Screen**[¶](#show-screen "Permanent link")

Restores the screen to being visible using a specified transition effect.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Asynchronous Transition

Whether the transition runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Render Scene

Whether the scene should be rendered when showing the screen.

Toggle

Render User Interface

Whether the user interface should be rendered when showing the screen.

Toggle

Transition

The transition effect to use when showing the screen.

[Scene Transition](../../../05-reference/scene-transition/)

## **Examples**[¶](#examples "Permanent link")

#### **Show Screen with a Fade In Transition**[¶](#show-screen-with-a-fade-in-transition "Permanent link")

Restores the screen to visible using a fade-in transition over 1000 milliseconds with a black color.

Code ScriptVisual Script

`[](#__codelineno-0-1)show_screen(fade_in(linear(1000), #000000));`

`[](#__codelineno-1-1){"Data":{"IsAsynchronousTransition":0,"IsRenderingScene":1,"IsRenderingUserInterface":1,"Transition":{"$":"FadeInSceneTransition","Color":"0,0,0,1","BlendMode":0,"Duration":"00:00:01","EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.ShowScreenCommand"}`

#### **Show Screen Instantly**[¶](#show-screen-instantly "Permanent link")

Restores the screen to visible immediately without any transition effect.

Code ScriptVisual Script

`[](#__codelineno-2-1)show_screen(instant);`

`[](#__codelineno-3-1){"Data":{"IsAsynchronousTransition":0,"IsRenderingScene":1,"IsRenderingUserInterface":1,"Transition":{"$":"InstantSceneTransition","Duration":"00:00:00","BlendMode":0,"EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.ShowScreenCommand"}`

#### **Show Screen Asynchronously While Hiding the User Interface**[¶](#show-screen-asynchronously-while-hiding-the-user-interface "Permanent link")

Fades in the screen asynchronously while keeping the user interface hidden.

Code ScriptVisual Script

`[](#__codelineno-4-1)show_screen(fade_in(linear(1000), #000000), async, hide_ui);`

`[](#__codelineno-5-1){"Data":{"IsAsynchronousTransition":1,"IsRenderingScene":1,"IsRenderingUserInterface":0,"Transition":{"$":"FadeInSceneTransition","Color":"0,0,0,1","BlendMode":0,"Duration":"00:00:01","EasingFunction":{"$":"LinearEasingFunction","Name":"Linear","Duration":"00:00:01","IsFinished":0,"IsReversed":0,"Metadata":null},"IsAsynchronous":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.ShowScreenCommand"}`

## **See Also**[¶](#see-also "Permanent link")

*   [Transition Editor](../../../04-editor/transition-editor/)