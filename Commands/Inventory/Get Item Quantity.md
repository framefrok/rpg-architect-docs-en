# Get Item Quantity

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/22-get-item-quantity/*

---

# Get Item Quantity

## **Get Item Quantity**[¶](#get-item-quantity "Permanent link")

Counts the total number of a specific item or equipment held in the party's inventory and stores the result in a variable.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Include Equipped Items

When enabled, equipment currently worn by party members is included in the count. Only applies when counting equipment.

Toggle

Item

When enabled, the command counts items. When disabled, the command counts equipment.

Toggle

Reference Index

The database index of the item or equipment to count in the inventory.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable where the total count of the specified item or equipment is stored.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Count Item 3 in the Inventory and Store in Global Variable 0**[¶](#count-item-3-in-the-inventory-and-store-in-global-variable-0 "Permanent link")

This counts how many of item 3 are in the party's inventory and stores the total in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = item_qty(3);`

`[](#__codelineno-1-1){"Data":{"IncludeEquipped":0,"IsItem":1,"ReferenceIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ItemQuantityCommand"}`

#### **Count Equipment 1 Including Equipped Copies**[¶](#count-equipment-1-including-equipped-copies "Permanent link")

This counts how many of equipment 1 are in the inventory, including copies currently equipped by party members, and stores the result in Local Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$lv[0] = item_qty(1, equipment, include_equipped);`

`[](#__codelineno-3-1){"Data":{"IncludeEquipped":1,"IsItem":0,"ReferenceIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ItemQuantityCommand"}`

#### **Count Equipment by Index from Global Variable 2**[¶](#count-equipment-by-index-from-global-variable-2 "Permanent link")

This counts equipment at the index stored in Global Variable 2 and stores the result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = item_qty($gv[2], equipment);`

`[](#__codelineno-5-1){"Data":{"IncludeEquipped":0,"IsItem":0,"ReferenceIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ItemQuantityCommand"}`