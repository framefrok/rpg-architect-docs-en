# Change Inventory

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/00-change-inventory/*

---

# Change Inventory

## **Change Inventory**[¶](#change-inventory "Permanent link")

Adds or removes items or equipment from the party's inventory.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Ignore Constraints

When enabled, inventory constraints such as maximum stack size or carry limits are bypassed.

Toggle

Instance

When enabled, each item added to the inventory is treated as a unique instance with its own identity.

Toggle

Inventory Slot

When enabled, the command targets an inventory slot by its unique ID rather than an item or equipment by database index.

Toggle

Item

When enabled, the command targets an item from the items database.

Toggle

Item Index

The database index or unique ID of the item or equipment to modify.

[Variable or Value](../../../05-reference/variable-or-value/)

Quantity

The amount to add or remove. Positive values add to the inventory and negative values remove from the inventory.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the number of items actually added or removed.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the number of items actually added or removed is stored in a variable.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Add 3 of Item 5 to the Inventory**[¶](#add-3-of-item-5-to-the-inventory "Permanent link")

This adds 3 of item index 5 to the party's inventory.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_inventory(5, 3, item);`

`[](#__codelineno-1-1){"Data":{"IgnoreConstraints":0,"Instance":0,"IsInventorySlot":0,"IsItem":1,"ItemIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"ItemQuantity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ChangeInventoryCommand"}`

#### **Remove 1 Equipment at Index from Global Variable 2 and Store the Result**[¶](#remove-1-equipment-at-index-from-global-variable-2-and-store-the-result "Permanent link")

This removes 1 of the equipment at the index stored in Global Variable 2, ignoring constraints, and stores how many were actually removed in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = change_inventory($gv[2], -1, equipment, ignore_constraints);`

`[](#__codelineno-3-1){"Data":{"IgnoreConstraints":1,"Instance":0,"IsInventorySlot":0,"IsItem":0,"ItemIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"ItemQuantity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ChangeInventoryCommand"}`

#### **Add 1 Instanced Item 0 to an Inventory Slot**[¶](#add-1-instanced-item-0-to-an-inventory-slot "Permanent link")

This adds 1 of item 0 to the inventory as a unique instance targeting an inventory slot.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_inventory(0, 1, inventory_slot, instance);`

`[](#__codelineno-5-1){"Data":{"IgnoreConstraints":0,"Instance":1,"IsInventorySlot":1,"IsItem":0,"ItemIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ItemQuantity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ChangeInventoryCommand"}`