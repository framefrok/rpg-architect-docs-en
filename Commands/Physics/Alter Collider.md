# Alter Collider

*Источник: https://docs.rpg-architect.com/07-commands/10-physics/02-alter-collider/*

---

# Alter Collider

## **Alter Collider**[¶](#alter-collider "Permanent link")

Changes the collider shape and dimensions of a physics object.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Depth

The depth of the collider along the Z axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Height

The height of the collider along the Y axis.

[Variable or Value](../../../05-reference/variable-or-value/)

Points

The vertices that define a convex hull collider shape. Requires at least 3 points.

Vector

Shape

The shape of the collider. Valid shapes include sphere, box, and convex hull.

[Variable or Value](../../../05-reference/variable-or-value/)

Target

The physics object to target with this command.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Width

The width of the collider along the X axis.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Entity Collider to a Sphere**[¶](#set-entity-collider-to-a-sphere "Permanent link")

Changes entity 0's collider to a sphere shape with width, height, and depth of 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)alter_collider(entity(0), sphere, 1, 1, 1);`

`[](#__codelineno-1-1){"Data":{"Depth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Points":[],"Shape":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterColliderCommand"}`

#### **Set Entity Collider to a Box**[¶](#set-entity-collider-to-a-box "Permanent link")

Changes entity 0's collider to a box shape with width 2, height 3, and depth 1.

Code ScriptVisual Script

`[](#__codelineno-2-1)alter_collider(entity(0), box, 2, 3, 1);`

`[](#__codelineno-3-1){"Data":{"Depth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Points":[],"Shape":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterColliderCommand"}`

#### **Set Entity Collider to a Convex Hull with Points**[¶](#set-entity-collider-to-a-convex-hull-with-points "Permanent link")

Changes entity 0's collider to a convex hull shape defined by four vertices.

Code ScriptVisual Script

`[](#__codelineno-4-1)alter_collider(entity(0), convex_hull, 1, 1, 1, points: [{ 0, 0, 0 }, { 1, 0, 0 }, { 0, 1, 0 }, { 0, 0, 1 }]);`

`[](#__codelineno-5-1){"Data":{"Depth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Points":["0,0,0","1,0,0","0,1,0","0,0,1"],"Shape":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"4","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterColliderCommand"}`