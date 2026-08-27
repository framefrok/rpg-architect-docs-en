# Scene

*Источник: https://docs.rpg-architect.com/05-reference/scene/*

---

# Scene

## **Scene**[¶](#scene "Permanent link")

Scenes are the top-level containers that drive what the player sees and interacts with. The engine maintains a scene stack — scenes can be pushed onto or popped from the stack, and the topmost scene is active.

Each scene type handles a specific phase of the game:

## **Scene Types**[¶](#scene-types "Permanent link")

Name

Explanation

Startup

The initial scene loaded when the game starts. Handles bootstrapping and loading anything that needs to be initialized before the Title sequence. The default implementation transitions to the Title scene once ready.

Title

Displays the title screen. Renders the background, title, and a [User Interface](../../06-database/09-user-interfaces/00-user-interfaces/) for the main menu (new game, load game, etc.). Can be configured via [Database / System / Title](../../06-database/10-system/20-title/).

New Game

A transitional scene between Title and Map. Loads the starting map and character data, then transitions to the Map scene. Can be configured via [Database / System / New Game](../../06-database/10-system/21-new-game/).

Load Game

A transitional scene that restores a saved game state and transitions to the Map scene.

Map

The primary gameplay scene. Handles map rendering, entity movement, player input, encounters, physics, and script execution. Can be configured via [Database / Maps / Configuration](../../06-database/03-maps/00-configuration/).

Battle

The battle engine scene. Manages battlers, turn order, action sequences, battle programs, and battle UI. Supports both turn-based and counter-based battle systems. Can be configured via [Database / Battles / Configuration](../../06-database/07-battles/00-configuration/).

Game Over

Displays the game over screen when the player loses. Can be configured via [Database / System / Game Over](../../06-database/10-system/25-game-over/).