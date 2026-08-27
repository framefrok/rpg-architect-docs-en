# Remove Entity

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/01-remove-entity/*

---

# Remove Entity

## **Remove Entity**[¶](#remove-entity "Permanent link")

Removes one or more entities from the scene and optionally clear their persistence data.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

All

Whether to remove all entities from the current scene.

Toggle

All Persisted

Whether to remove all persisted entities across all maps.

Toggle

All Persisted on Map

Whether to remove all persisted entities on the current map only.

Toggle

Entity

The specific entity to remove from the scene.

[Actor Reference](../../../05-reference/actor-reference/)

Remove Persistence

Whether to also remove the entity from persistence data so it does not respawn.

Toggle

Specific

Whether to remove a specific entity identified by the target reference.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Remove a Specific Entity**[¶](#remove-a-specific-entity "Permanent link")

This removes entity 0 from the map and clears its persistence data.

Code ScriptVisual Script

`[](#__codelineno-0-1)remove_actor(entity(0));`

`[](#__codelineno-1-1){"Data":{"IsAll":0,"IsAllPersisted":0,"IsMapPersisted":0,"IsSpecific":1,"RemovePersistence":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityRemoveEntityCommand"}`

#### **Remove All Spawned Entities**[¶](#remove-all-spawned-entities "Permanent link")

This removes all spawned entities from the map and clears their persistence data.

Code ScriptVisual Script

`[](#__codelineno-2-1)remove_actor(all);`

`[](#__codelineno-3-1){"Data":{"IsAll":1,"IsAllPersisted":0,"IsMapPersisted":0,"IsSpecific":0,"RemovePersistence":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":1,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityRemoveEntityCommand"}`

#### **Remove Entity But Keep Its Persistence Data**[¶](#remove-entity-but-keep-its-persistence-data "Permanent link")

This removes entity 0 from the map but preserves its persistence data so it returns on map reload.

Code ScriptVisual Script

`[](#__codelineno-4-1)remove_actor(entity(0), keep_persistence);`

`[](#__codelineno-5-1){"Data":{"IsAll":0,"IsAllPersisted":0,"IsMapPersisted":0,"IsSpecific":1,"RemovePersistence":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityRemoveEntityCommand"}`