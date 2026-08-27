# Move Entity

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/10-move-entity/*

---

# Move Entity

## **Move Entity**[¶](#move-entity "Permanent link")

Makes an actor or entity follow a defined movement pattern.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Movement

The movement pattern to apply to the target actor.

MovementCollection

Target

The actor or entity to apply the movement to.

[Actor Reference](../../../05-reference/actor-reference/)

Wait to Complete

Whether the script waits for the movement to finish before continuing to the next command.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Move Entity 0 with a Movement Sequence**[¶](#move-entity-0-with-a-movement-sequence "Permanent link")

This moves entity 0 along a predefined movement path and waits for the movement to complete before continuing.

Code ScriptVisual Script

`[](#__codelineno-0-1)move_actor(entity(0), [step(north), step(east), step(south)], wait_for_completion);`

`[](#__codelineno-1-1){"Data":{"IsRequiringMovementToComplete":1,"MovementCollection":{"Elements":[{"$":"StepMovementElement","Direction":1,"IsAscentStep":0,"IsAwayFromHeroStep":0,"IsBackwardStep":0,"IsDescentStep":0,"IsDirectionStep":1,"IsForwardStep":0,"IsRandomAscentDescent":0,"IsRandomStep":0,"IsTowardHeroStep":0,"IsVerticalMovementOnly":0,"StepFactor":1,"Summary":null,"Metadata":null},{"$":"StepMovementElement","Direction":3,"IsAscentStep":0,"IsAwayFromHeroStep":0,"IsBackwardStep":0,"IsDescentStep":0,"IsDirectionStep":1,"IsForwardStep":0,"IsRandomAscentDescent":0,"IsRandomStep":0,"IsTowardHeroStep":0,"IsVerticalMovementOnly":0,"StepFactor":1,"Summary":null,"Metadata":null},{"$":"StepMovementElement","Direction":5,"IsAscentStep":0,"IsAwayFromHeroStep":0,"IsBackwardStep":0,"IsDescentStep":0,"IsDirectionStep":1,"IsForwardStep":0,"IsRandomAscentDescent":0,"IsRandomStep":0,"IsTowardHeroStep":0,"IsVerticalMovementOnly":0,"StepFactor":1,"Summary":null,"Metadata":null}],"IgnoreInvalidMovement":0,"IsRecycling":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Blocking":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityMovementCommand"}`