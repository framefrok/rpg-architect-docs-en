# Clear Inventory

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/01-clear-inventory/*

---

# Clear Inventory

## **Clear Inventory**[¶](#clear-inventory "Permanent link")

Removes all items of a specified type from the party's inventory.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Item Type

The item type to clear from the inventory. Only items matching the specified type will be removed.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Clear All Items of Type 0 from the Inventory**[¶](#clear-all-items-of-type-0-from-the-inventory "Permanent link")

This removes all items matching item type 0 from the party's inventory.

Code ScriptVisual Script

`[](#__codelineno-0-1)clear_inventory(0);`

`[](#__codelineno-1-1){"Data":{"ItemType":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ClearInventoryCommand"}`

#### **Clear Items by Type Stored in Local Variable 2**[¶](#clear-items-by-type-stored-in-local-variable-2 "Permanent link")

This removes all items matching the type stored in Local Variable 2 from the party's inventory.

Code ScriptVisual Script

`[](#__codelineno-2-1)clear_inventory($lv[2]);`

`[](#__codelineno-3-1){"Data":{"ItemType":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ClearInventoryCommand"}`