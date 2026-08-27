# Spawn Projection

*Источник: https://docs.rpg-architect.com/07-commands/13-projection/00-spawn-projection/*

---

# Spawn Projection

## **Spawn Projection**[¶](#spawn-projection "Permanent link")

Spawns a projection from the database at a specified actor's position.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Origin

The actor whose position is used as the origin for the spawned projection.

[Actor Reference](../../../05-reference/actor-reference/)

Projection

The projection to spawn from the database, specified by index.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the spawned projection's unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Store ID

When enabled, the unique ID of the spawned projection is stored in a variable.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Spawn a Projection at a Party Member**[¶](#spawn-a-projection-at-a-party-member "Permanent link")

Spawns projection 0 at the position of party member 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)spawn_projection(0, party(0));`

`[](#__codelineno-1-1){"Data":{"ProjectionID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"StoreID":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Projection.ProjectionSpawnProjectionCommand"}`

#### **Spawn a Projection and Store Its Unique ID**[¶](#spawn-a-projection-and-store-its-unique-id "Permanent link")

Spawns projection 1 at the position of party member 0 and stores the resulting unique ID in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = spawn_projection(1, party(0));`

`[](#__codelineno-3-1){"Data":{"ProjectionID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"StoreID":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Projection.ProjectionSpawnProjectionCommand"}`

#### **Spawn a Projection at the Current Entity**[¶](#spawn-a-projection-at-the-current-entity "Permanent link")

Spawns projection 2 at the position of the current entity (self).

Code ScriptVisual Script

`[](#__codelineno-4-1)spawn_projection(2, self);`

`[](#__codelineno-5-1){"Data":{"ProjectionID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"StoreID":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Projection.ProjectionSpawnProjectionCommand"}`