# Access Entity Local Variable

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/20-access-entity-local-variable/*

---

# Access Entity Local Variable

## **Access Entity Local Variable**[¶](#access-entity-local-variable "Permanent link")

Gets or set the value of a local variable on a specific entity.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Entity

The entity whose local variable will be accessed.

[Actor Reference](../../../05-reference/actor-reference/)

Get Value

Whether the command reads the entity variable value into a global or local variable.

Toggle

Global Variable

The global variable index to read from or write to.

Number

Local Variable

The local variable index to read from or write to.

Number

Reference Variable

The index of the local variable on the target entity to access.

Number

Set Value

Whether the command writes a value to the entity variable.

Toggle

Use Global Variable

Whether to use a global variable as the source or destination.

Toggle

Use Local Variable

Whether to use a local variable as the source or destination.

Toggle

Use Value

Whether to set the entity variable to a literal value instead of copying from a global or local variable.

Toggle

Value

The literal value to set the entity variable to when **Use Value** is enabled.

String

## **Examples**[¶](#examples "Permanent link")

#### **Read Entity 0 Local Variable 0 into Global Variable 0**[¶](#read-entity-0-local-variable-0-into-global-variable-0 "Permanent link")

This reads the value of local variable 0 on entity 0 and stores it in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = entity_var(entity(0), 0);`

`[](#__codelineno-1-1){"Data":{"GlobalIndex":0,"IsGetter":1,"IsGlobal":1,"IsLocal":0,"IsSetter":0,"IsValue":0,"LocalIndex":0,"ReferenceIndex":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Value":"","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityLocalVariableAccessCommand"}`

#### **Set Entity 0 Local Variable 0 to a String Value**[¶](#set-entity-0-local-variable-0-to-a-string-value "Permanent link")

This sets local variable 0 on entity 0 to the string "hello".

Code ScriptVisual Script

`[](#__codelineno-2-1)entity_var(entity(0), 0, "hello");`

`[](#__codelineno-3-1){"Data":{"GlobalIndex":0,"IsGetter":0,"IsGlobal":0,"IsLocal":0,"IsSetter":1,"IsValue":1,"LocalIndex":0,"ReferenceIndex":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Value":"hello","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityLocalVariableAccessCommand"}`

#### **Copy Global Variable 5 to Entity 0 Local Variable 0**[¶](#copy-global-variable-5-to-entity-0-local-variable-0 "Permanent link")

This copies the value of Global Variable 5 into local variable 0 on entity 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)entity_var(entity(0), 0, $gv[5]);`

`[](#__codelineno-5-1){"Data":{"GlobalIndex":5,"IsGetter":0,"IsGlobal":1,"IsLocal":0,"IsSetter":1,"IsValue":0,"LocalIndex":0,"ReferenceIndex":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Value":"","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityLocalVariableAccessCommand"}`