# New Game

*Источник: https://docs.rpg-architect.com/07-commands/22-scene/01-new-game/*

---

# New Game

## **New Game**[¶](#new-game "Permanent link")

Pops all scenes and start a new game from the beginning.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Use Scene Transition

Whether to use the transitions associated with the current scene.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Start a New Game**[¶](#start-a-new-game "Permanent link")

Pops all scenes and starts a new game from the beginning using the current scene's exit transition.

Code ScriptVisual Script

`[](#__codelineno-0-1)new_game();`

`[](#__codelineno-1-1){"Data":{"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneNewGameCommand"}`

#### **Start a New Game Without a Transition**[¶](#start-a-new-game-without-a-transition "Permanent link")

Starts a new game immediately without playing any scene transition.

Code ScriptVisual Script

`[](#__codelineno-2-1)new_game(no_transition);`

`[](#__codelineno-3-1){"Data":{"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneNewGameCommand"}`