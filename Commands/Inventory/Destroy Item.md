# Destroy Item

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/21-destroy-item/*

---

# Destroy Item

## **Destroy Item**[¶](#destroy-item "Permanent link")

Permanently remove a specific item or equipment instance from the inventory by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Item or Equipment Unique ID

The unique ID of the item or equipment instance to destroy.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Destroy an Item by Unique Identifier in Global Variable 0**[¶](#destroy-an-item-by-unique-identifier-in-global-variable-0 "Permanent link")

This permanently removes the item or equipment identified by the unique ID stored in Global Variable 0 from the inventory.

Code ScriptVisual Script

`[](#__codelineno-0-1)destroy_item($gv[0]);`

`[](#__codelineno-1-1){"Data":{"Identifier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.DestroyItemCommand"}`

#### **Destroy an Item by Unique Identifier in Local Variable 3**[¶](#destroy-an-item-by-unique-identifier-in-local-variable-3 "Permanent link")

This permanently removes the item or equipment identified by the unique ID stored in Local Variable 3 from the inventory.

Code ScriptVisual Script

`[](#__codelineno-2-1)destroy_item($lv[3]);`

`[](#__codelineno-3-1){"Data":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":3,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.DestroyItemCommand"}`