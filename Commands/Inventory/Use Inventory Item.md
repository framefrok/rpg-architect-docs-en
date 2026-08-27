# Use Inventory Item

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/30-use-inventory-item/*

---

# Use Inventory Item

## **Use Inventory Item**[¶](#use-inventory-item "Permanent link")

Applies the effects of an inventory item to a hero, consuming it if it is a consumable type.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Hero

The hero who will use the item.

[Character](../../../06-database/00-characters/00-characters/)

Inventory Item

The inventory item to use on the hero.

InventorySlot

Result

The switch to store whether the item use succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Store Results

When enabled, the success or failure of the item use is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Use an Inventory Item on Hero 0**[¶](#use-an-inventory-item-on-hero-0 "Permanent link")

This applies the effects of the inventory item referenced by its unique ID to hero 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)use_item(hero(0), inventory(0));`

`[](#__codelineno-1-1){"Data":{"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"InventorySlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.UseItemCommand"}`

#### **Use an Inventory Item on Hero 2 and Store the Result**[¶](#use-an-inventory-item-on-hero-2-and-store-the-result "Permanent link")

This uses the inventory item on hero 2 and stores whether the use succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = use_item(hero(2), inventory(0));`

`[](#__codelineno-3-1){"Data":{"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"InventorySlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.UseItemCommand"}`