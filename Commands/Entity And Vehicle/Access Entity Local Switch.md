# Access Entity Local Switch

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/21-access-entity-local-switch/*

---

# Access Entity Local Switch

## **Access Entity Local Switch**[¶](#access-entity-local-switch "Permanent link")

Gets or set the value of a local switch on a specific entity.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Entity

The entity whose local switch will be accessed.

[Actor Reference](../../../05-reference/actor-reference/)

Get Value

Whether the command reads the entity switch value into a global or local switch.

Toggle

Global Switch

The global switch index to read from or write to.

Number

Local Switch

The local switch index to read from or write to.

Number

Reference Switch

The index of the local switch on the target entity to access.

Number

Set Value

Whether the command writes a value to the entity switch.

Toggle

Use Global Switch

Whether to use a global switch as the source or destination.

Toggle

Use Local Switch

Whether to use a local switch as the source or destination.

Toggle

Use Value

Whether to set the entity switch to a literal value instead of copying from a global or local switch.

Toggle

Value

The literal value to set the entity switch to when **Use Value** is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Read Entity 0 Local Switch 0 into Global Switch 0**[¶](#read-entity-0-local-switch-0-into-global-switch-0 "Permanent link")

This reads the value of local switch 0 on entity 0 and stores it in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gs[0] = entity_switch(entity(0), 0);`

`[](#__codelineno-1-1){"Data":{"GlobalIndex":0,"IsGetter":1,"IsGlobal":1,"IsLocal":0,"IsSetter":0,"IsValue":0,"LocalIndex":0,"ReferenceIndex":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Value":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityLocalSwitchAccessCommand"}`

#### **Set Entity 0 Local Switch 0 to True**[¶](#set-entity-0-local-switch-0-to-true "Permanent link")

This sets local switch 0 on entity 0 to true.

Code ScriptVisual Script

`[](#__codelineno-2-1)entity_switch(entity(0), 0, true);`

`[](#__codelineno-3-1){"Data":{"GlobalIndex":0,"IsGetter":0,"IsGlobal":0,"IsLocal":0,"IsSetter":1,"IsValue":1,"LocalIndex":0,"ReferenceIndex":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Value":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityLocalSwitchAccessCommand"}`