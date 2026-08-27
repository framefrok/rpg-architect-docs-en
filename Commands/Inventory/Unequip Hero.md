# Unequip Hero

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/41-unequip-hero/*

---

# Unequip Hero

## **Unequip Hero**[¶](#unequip-hero "Permanent link")

Removes equipment from a hero's equipment slot and return it to the inventory.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Equipment Slot

The equipment slot to unequip. If not specified, all equipment slots are unequipped.

[Equipment Slot](../../../06-database/02-items/10-equipment-slots/)

Hero

The hero whose equipment will be removed.

[Character](../../../06-database/00-characters/00-characters/)

Ignore Constraints

When enabled, equipment restrictions are bypassed when unequipping.

Toggle

Result

The switch to store whether the unequip operation succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Store Results

When enabled, the success or failure of the unequip operation is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Unequip Hero 0 from Equipment Slot 0**[¶](#unequip-hero-0-from-equipment-slot-0 "Permanent link")

This removes the equipment in equipment slot 0 from hero 0 and returns it to the inventory.

Code ScriptVisual Script

`[](#__codelineno-0-1)unequip_item(hero(0), equip_slot(0));`

`[](#__codelineno-1-1){"Data":{"EquipmentSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IgnoreConstraints":0,"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.UnequipItemCommand"}`

#### **Unequip Hero 1 Ignoring Constraints and Store the Result**[¶](#unequip-hero-1-ignoring-constraints-and-store-the-result "Permanent link")

This removes equipment from equipment slot 2 on hero 1, bypassing restrictions, and stores whether the operation succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = unequip_item(hero(1), equip_slot(2), ignore_constraints);`

`[](#__codelineno-3-1){"Data":{"EquipmentSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IgnoreConstraints":1,"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.UnequipItemCommand"}`