# End Battle

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/110-end-battle/*

---

# End Battle

## **End Battle**[¶](#end-battle "Permanent link")

Ends the current battle, optionally returning to the prior scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Return to Prior Scene

When enabled, the game will return to the scene that was active before the battle started.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **End the Current Battle**[¶](#end-the-current-battle "Permanent link")

This ends the current battle without returning to the prior scene.

Code ScriptVisual Script

`[](#__codelineno-0-1)end_battle();`

`[](#__codelineno-1-1){"Data":{"ReturnToPriorScene":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.EndBattleCommand"}`

#### **End the Current Battle and Return to the Prior Scene**[¶](#end-the-current-battle-and-return-to-the-prior-scene "Permanent link")

This ends the current battle and returns to the scene that was active before the battle started.

Code ScriptVisual Script

`[](#__codelineno-2-1)end_battle(true);`

`[](#__codelineno-3-1){"Data":{"ReturnToPriorScene":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.EndBattleCommand"}`