# Start Battle

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/00-start-battle/*

---

# Start Battle

## **Start Battle**[¶](#start-battle "Permanent link")

Initiates a battle with the specified enemy formation and battle backdrop.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battle Backdrop

The battle backdrop to use for the battle scene.

[Variable or Value](../../../05-reference/variable-or-value/)

Enemy Formation

The enemy formation to use for the battle.

[Variable or Value](../../../05-reference/variable-or-value/)

Enemy Formation Seed

The seed value to use for enemy formation randomization. Only used when **Use Enemy Formation Seed** is enabled.

[Variable or Value](../../../05-reference/variable-or-value/)

Enemy Formation Seed Result

The variable to store the resulting enemy formation seed in. Only used when **Store Results** is enabled.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the resulting enemy formation seed will be saved to the specified variable.

Toggle

Use Enemy Formation Seed

When enabled, a specific seed value will be used for enemy formation randomization instead of a random seed.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Start a Battle with Backdrop 0 and Formation 0**[¶](#start-a-battle-with-backdrop-0-and-formation-0 "Permanent link")

This starts a battle using battle backdrop 0 and enemy formation 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)start_battle(0, 0);`

`[](#__codelineno-1-1){"Data":{"BattleBackdropIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"EnemyFormationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"EnemyFormationSeed":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"EnemyFormationSeedResult":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":-1,"Metadata":null},"StoreResults":0,"UseEnemyFormationSeed":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.StartBattleCommand"}`

#### **Start a Battle with a Specific Seed Value**[¶](#start-a-battle-with-a-specific-seed-value "Permanent link")

This starts a battle using backdrop 1 and formation 2, with a specific seed for enemy formation randomization.

Code ScriptVisual Script

`[](#__codelineno-2-1)start_battle(1, 2, seed: 42);`

`[](#__codelineno-3-1){"Data":{"BattleBackdropIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"EnemyFormationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"EnemyFormationSeed":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"42","VariableIndex":0,"Metadata":null},"EnemyFormationSeedResult":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":-1,"Metadata":null},"StoreResults":0,"UseEnemyFormationSeed":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.StartBattleCommand"}`

#### **Start a Battle and Store the Resulting Seed**[¶](#start-a-battle-and-store-the-resulting-seed "Permanent link")

This starts a battle and stores the resulting enemy formation seed in Global Variable 0 for later use.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = start_battle(0, 1, seed: $gv[1]);`

`[](#__codelineno-5-1){"Data":{"BattleBackdropIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"EnemyFormationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"EnemyFormationSeed":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"EnemyFormationSeedResult":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"UseEnemyFormationSeed":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.StartBattleCommand"}`