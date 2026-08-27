# Save Entity Unique ID

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/22-save-entity-unique-id/*

---

# Save Entity Unique ID

## **Save Entity Unique ID**[¶](#save-entity-unique-id "Permanent link")

Saves the unique ID of an entity to a variable for later reference.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Destination Variable

The variable where the entity's unique ID will be stored.

[Variable or Value](../../../05-reference/variable-or-value/)

Entity

The entity whose unique ID will be saved.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Save Entity 0 Unique ID to Global Variable 0**[¶](#save-entity-0-unique-id-to-global-variable-0 "Permanent link")

This saves the Unique ID of entity 0 into Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = save_actor_uid(entity(0));`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntitySaveUniqueIDCommand"}`

#### **Save Self Unique ID to Global Variable 0**[¶](#save-self-unique-id-to-global-variable-0 "Permanent link")

This saves the Unique ID of the calling entity into Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = save_actor_uid(self);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntitySaveUniqueIDCommand"}`