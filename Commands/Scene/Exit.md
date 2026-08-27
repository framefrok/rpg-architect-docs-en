# Exit

*Источник: https://docs.rpg-architect.com/07-commands/22-scene/04-exit/*

---

# Exit

## **Exit**[¶](#exit "Permanent link")

Ends the scene engine and exit the game.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Use Scene Transition

Whether to use the transitions associated with the current scene.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Exit the Game**[¶](#exit-the-game "Permanent link")

Ends the scene engine and exits the game using the current scene's exit transition.

Code ScriptVisual Script

`[](#__codelineno-0-1)exit_game();`

`[](#__codelineno-1-1){"Data":{"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneExitCommand"}`

#### **Exit the Game Without a Transition**[¶](#exit-the-game-without-a-transition "Permanent link")

Exits the game immediately without playing any scene transition.

Code ScriptVisual Script

`[](#__codelineno-2-1)exit_game(no_transition);`

`[](#__codelineno-3-1){"Data":{"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Scene.SceneExitCommand"}`