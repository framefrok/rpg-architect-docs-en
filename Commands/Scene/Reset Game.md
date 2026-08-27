# Reset Game

*Источник: https://docs.rpg-architect.com/07-commands/22-scene/02-reset-game/*

---

# Reset Game

## **Reset Game**[¶](#reset-game "Permanent link")

Clears the entire scene stack and restart all cores from the very beginning.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Use Scene Transition

Whether to use the transitions associated with the current scene.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Reset the Entire Game**[¶](#reset-the-entire-game "Permanent link")

Clears the entire scene stack and restarts all cores from the very beginning using the current scene's exit transition.

Code ScriptVisual Script

`[](#__codelineno-0-1)reset_game();`

`[](#__codelineno-1-1){"Data":{"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneResetGameCommand"}`

#### **Reset the Entire Game Without a Transition**[¶](#reset-the-entire-game-without-a-transition "Permanent link")

Resets the game immediately without playing any scene transition.

Code ScriptVisual Script

`[](#__codelineno-2-1)reset_game(no_transition);`

`[](#__codelineno-3-1){"Data":{"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneResetGameCommand"}`