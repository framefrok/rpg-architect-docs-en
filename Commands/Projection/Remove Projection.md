# Remove Projection

*Источник: https://docs.rpg-architect.com/07-commands/13-projection/01-remove-projection/*

---

# Remove Projection

## **Remove Projection**[¶](#remove-projection "Permanent link")

Removes an active projection from the current scene by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Projection Unique ID

The unique ID of the projection to remove from the scene.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Remove a Projection by Variable**[¶](#remove-a-projection-by-variable "Permanent link")

Removes the projection whose unique ID is stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)remove_projection($gv[0]);`

`[](#__codelineno-1-1){"Data":{"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Projection.ProjectionRemoveProjectionCommand"}`

#### **Remove a Projection by String Literal**[¶](#remove-a-projection-by-string-literal "Permanent link")

Removes the projection with the specified unique ID string.

Code ScriptVisual Script

`[](#__codelineno-2-1)remove_projection("550e8400-e29b-41d4-a716-446655440000");`

`[](#__codelineno-3-1){"Data":{"Target":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"550e8400-e29b-41d4-a716-446655440000","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Projection.ProjectionRemoveProjectionCommand"}`