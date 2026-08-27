# Set Portrait Expression

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/11-set-portrait-expression/*

---

# Set Portrait Expression

## **Set Portrait Expression**[¶](#set-portrait-expression "Permanent link")

Changes the active portrait expression on an actor.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Portrait Expression

The index of the portrait expression to set from the database.

[Variable or Value](../../../05-reference/variable-or-value/)

Reset Animation

Whether to reset the portrait expression back to the default.

Toggle

Target

The actor to set the portrait expression on.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Portrait Expression on an Entity**[¶](#set-portrait-expression-on-an-entity "Permanent link")

Sets portrait expression 3 from the database on entity 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_portrait_expression(entity(0), 3);`

`[](#__codelineno-1-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsReset":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetPortaitExpressionCommand"}`

#### **Reset Portrait Expression on Self**[¶](#reset-portrait-expression-on-self "Permanent link")

Resets the portrait expression back to the default on the current entity.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_portrait_expression(self, reset);`

`[](#__codelineno-3-1){"Data":{"CharacterModelAnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsReset":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.SetPortaitExpressionCommand"}`