# Title

*Источник: https://docs.rpg-architect.com/07-commands/22-scene/00-title/*

---

# Title

## **Title**[¶](#title "Permanent link")

Returns to the title screen scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Use Scene Transition

Whether to use the transitions associated with the current scene.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Return to the Title Screen**[¶](#return-to-the-title-screen "Permanent link")

Returns to the title screen using the current scene's exit transition.

Code ScriptVisual Script

`[](#__codelineno-0-1)scene_title();`

`[](#__codelineno-1-1){"Data":{"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneTitleCommand"}`

#### **Return to the Title Screen Without a Transition**[¶](#return-to-the-title-screen-without-a-transition "Permanent link")

Returns to the title screen immediately without playing any scene transition.

Code ScriptVisual Script

`[](#__codelineno-2-1)scene_title(no_transition);`

`[](#__codelineno-3-1){"Data":{"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneTitleCommand"}`