# Set Battle Pose

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/11-set-battle-pose/*

---

# Set Battle Pose

## **Set Battle Pose**[¶](#set-battle-pose "Permanent link")

Changes the active battle pose on a battler during combat.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Character Animation

The index of the battle pose to set from the database.

[Variable or Value](../../../05-reference/variable-or-value/)

Reset Animation

Whether to reset the battle pose back to the default.

Toggle

Target

The battler to set the battle pose on.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Battle Pose on a Battler**[¶](#set-battle-pose-on-a-battler "Permanent link")

Sets battle pose 3 from the database on entity 0 during combat.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_battle_pose(entity(0), 3);`

`[](#__codelineno-1-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsReset":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetBattlePoseCommand"}`

#### **Reset Battle Pose on a Battler**[¶](#reset-battle-pose-on-a-battler "Permanent link")

Resets the battle pose back to the default on entity 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_battle_pose(entity(0), reset);`

`[](#__codelineno-3-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsReset":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetBattlePoseCommand"}`