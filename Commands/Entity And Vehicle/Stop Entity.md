# Stop Entity

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/11-stop-entity/*

---

# Stop Entity

## **Stop Entity**[¶](#stop-entity "Permanent link")

Stops an actor or entity's current movement and reset its movement state.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Target

The actor or entity whose movement will be stopped.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Stop Movement on Entity 0**[¶](#stop-movement-on-entity-0 "Permanent link")

This stops all active movement on entity 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)stop_actor(entity(0));`

`[](#__codelineno-1-1){"Data":{"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityStopMovementCommand"}`

#### **Stop Movement on Self**[¶](#stop-movement-on-self "Permanent link")

This stops all active movement on the calling entity.

Code ScriptVisual Script

`[](#__codelineno-2-1)stop_actor(self);`

`[](#__codelineno-3-1){"Data":{"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityStopMovementCommand"}`