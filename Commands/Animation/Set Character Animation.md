# Set Character Animation

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/10-set-character-animation/*

---

# Set Character Animation

## **Set Character Animation**[¶](#set-character-animation "Permanent link")

Changes the active character animation on an actor.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Character Animation

The index of the character animation to set from the database.

[Variable or Value](../../../05-reference/variable-or-value/)

Reset Animation

Whether to reset the character animation back to the default.

Toggle

Target

The actor to set the character animation on.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Character Animation on an Entity**[¶](#set-character-animation-on-an-entity "Permanent link")

Sets character animation 3 from the database on entity 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_actor_pose(entity(0), 3);`

`[](#__codelineno-1-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsReset":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetActorPoseCommand"}`

#### **Reset Character Animation on an Entity**[¶](#reset-character-animation-on-an-entity "Permanent link")

Resets the character animation back to the default on entity 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_actor_pose(entity(0), reset);`

`[](#__codelineno-3-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsReset":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetActorPoseCommand"}`