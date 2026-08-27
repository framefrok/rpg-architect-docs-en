# Change Name

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/1000-change-name/*

---

# Change Name

## **Change Name**[¶](#change-name "Permanent link")

Renames an object identified by its [Unique ID](../../../05-reference/unique-id/), targeting heroes, battlers, skills, or inventory items.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Name

The new name to assign to the target object.

[Variable or Value](../../../05-reference/variable-or-value/)

Target Unique ID

The unique identifier of the object to rename. This can be a hero, battler, skill, or inventory item.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Rename Object to a Fixed Name Using Unique ID from Global Variable 0**[¶](#rename-object-to-a-fixed-name-using-unique-id-from-global-variable-0 "Permanent link")

This renames the object identified by the Unique ID stored in Global Variable 0 to "Hero Name".

Code ScriptVisual Script

`[](#__codelineno-0-1)change_name($gv[0], "Hero Name");`

`[](#__codelineno-1-1){"Data":{"TargetName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"Hero Name","VariableIndex":0,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Data.ChangeNameCommand"}`

#### **Rename Object Using Variables for Both Unique ID and Name**[¶](#rename-object-using-variables-for-both-unique-id-and-name "Permanent link")

This renames the object identified by the Unique ID stored in Global Variable 0 to the name stored in Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_name($gv[0], $gv[1]);`

`[](#__codelineno-3-1){"Data":{"TargetName":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"TargetUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Data.ChangeNameCommand"}`