# Game Over

*Источник: https://docs.rpg-architect.com/07-commands/22-scene/03-game-over/*

---

# Game Over

## **Game Over**[¶](#game-over "Permanent link")

Transitions the current scene to the game over screen.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Use Scene Transition

Whether to use the transitions associated with the current scene.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Trigger the Game Over Screen**[¶](#trigger-the-game-over-screen "Permanent link")

Transitions to the game over screen using the current scene's exit transition.

Code ScriptVisual Script

`[](#__codelineno-0-1)scene_game_over();`

`[](#__codelineno-1-1){"Data":{"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneGameOverCommand"}`

#### **Trigger the Game Over Screen Without a Transition**[¶](#trigger-the-game-over-screen-without-a-transition "Permanent link")

Transitions to the game over screen immediately without playing any scene transition.

Code ScriptVisual Script

`[](#__codelineno-2-1)scene_game_over(no_transition);`

`[](#__codelineno-3-1){"Data":{"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneGameOverCommand"}`