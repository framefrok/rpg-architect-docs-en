# Spawn Entity

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/00-spawn-entity/*

---

# Spawn Entity

## **Spawn Entity**[¶](#spawn-entity "Permanent link")

Spawns an entity from the database at a specified position on the current map.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Direction

The cardinal direction the spawned entity should face.

[Variable or Value](../../../05-reference/variable-or-value/)

Entity

The entity definition from the database to spawn.

[Variable or Value](../../../05-reference/variable-or-value/)

Persist

Whether the spawned entity should be saved in persistence data so it survives scene transitions.

Toggle

Result

The variable to store the spawned entity's unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Specify Direction

Whether to set a specific facing direction for the spawned entity.

Toggle

Store ID

Whether to store the unique ID of the spawned entity in a variable.

Toggle

X

The X coordinate to spawn the entity at.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y coordinate to spawn the entity at.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z coordinate to spawn the entity at.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Spawn Entity Definition 1 at Position (10, 5, 0)**[¶](#spawn-entity-definition-1-at-position-10-5-0 "Permanent link")

This spawns an entity from database definition 1 at coordinates (10, 5, 0) on the current map.

Code ScriptVisual Script

`[](#__codelineno-0-1)spawn_entity(1, 10, 5, 0);`

`[](#__codelineno-1-1){"Data":{"Direction":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"EntityDefinitionID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsDirectionSpecified":0,"Persist":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntitySpawnEntityCommand"}`

#### **Spawn Entity with Direction and Persistence**[¶](#spawn-entity-with-direction-and-persistence "Permanent link")

This spawns an entity from database definition 1 at coordinates (10, 5, 0), facing direction 2, and persists the entity across map reloads.

Code ScriptVisual Script

`[](#__codelineno-2-1)spawn_entity(1, 10, 5, 0, direction: 2, persist);`

`[](#__codelineno-3-1){"Data":{"Direction":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"EntityDefinitionID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsDirectionSpecified":1,"Persist":1,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntitySpawnEntityCommand"}`