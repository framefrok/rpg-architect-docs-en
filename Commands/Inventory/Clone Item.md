# Clone Item

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/20-clone-item/*

---

# Clone Item

## **Clone Item**[¶](#clone-item "Permanent link")

Creates a duplicate of an existing item or equipment in the inventory as a new instance with its own unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Ignore Constraints

When enabled, inventory constraints such as maximum stack size or carry limits are bypassed when adding the cloned item.

Toggle

Item or Equipment Unique ID

The unique ID of the item or equipment to clone.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable where the unique ID of the newly cloned item is stored.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the unique ID of the cloned item is stored in the specified result variable.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Clone an Item by Unique Identifier Stored in Global Variable 0**[¶](#clone-an-item-by-unique-identifier-stored-in-global-variable-0 "Permanent link")

This duplicates the item or equipment identified by the unique ID stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)copy_item($gv[0]);`

`[](#__codelineno-1-1){"Data":{"Identifier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IgnoreConstraints":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.CopyItemCommand"}`

#### **Clone an Item and Store the New Unique Identifier**[¶](#clone-an-item-and-store-the-new-unique-identifier "Permanent link")

This duplicates the item identified by the unique ID in Global Variable 1, ignoring constraints, and stores the new item's unique ID in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = copy_item($gv[1], ignore_constraints);`

`[](#__codelineno-3-1){"Data":{"Identifier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"IgnoreConstraints":1,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.CopyItemCommand"}`