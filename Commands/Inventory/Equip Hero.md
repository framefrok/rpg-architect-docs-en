# Equip Hero

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/40-equip-hero/*

---

# Equip Hero

## **Equip Hero**[¶](#equip-hero "Permanent link")

Assigns a piece of equipment from the inventory to a specific equipment slot on a hero.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Equipment

The equipment to assign to the hero.

[Equipment](../../../06-database/02-items/02-equipment/)

Equipment Slot

The equipment slot on the hero where the equipment will be placed.

[Equipment Slot](../../../06-database/02-items/10-equipment-slots/)

Hero

The hero who will receive the equipment.

[Character](../../../06-database/00-characters/00-characters/)

Ignore Constraints

When enabled, equipment restrictions such as class or level requirements are bypassed.

Toggle

Require Unequipped

When enabled, the equipment must not already be equipped by another party member.

Toggle

Result

The switch to store whether the equip operation succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Store Results

When enabled, the success or failure of the equip operation is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Equip Hero 0 with Equipment 0 in Equipment Slot 0**[¶](#equip-hero-0-with-equipment-0-in-equipment-slot-0 "Permanent link")

This assigns equipment at index 0 to the first equipment slot on hero 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)equip_item(hero(0), equipment(0), equip_slot(0));`

`[](#__codelineno-1-1){"Data":{"Equipment":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"EquipmentSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IgnoreConstraints":0,"IsConstrainedToUnequipped":0,"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.EquipItemCommand"}`

#### **Equip Hero 1 Ignoring Constraints and Store the Result**[¶](#equip-hero-1-ignoring-constraints-and-store-the-result "Permanent link")

This equips hero 1 with equipment 2 in equipment slot 0, bypassing restrictions, and stores whether the operation succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = equip_item(hero(1), equipment(2), equip_slot(0), ignore_constraints);`

`[](#__codelineno-3-1){"Data":{"Equipment":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"EquipmentSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IgnoreConstraints":1,"IsConstrainedToUnequipped":0,"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.EquipItemCommand"}`

#### **Equip Hero 0 Requiring the Equipment to Be Unequipped**[¶](#equip-hero-0-requiring-the-equipment-to-be-unequipped "Permanent link")

This equips hero 0 with equipment 1 in equipment slot 0, but only if the equipment is not already worn by another party member.

Code ScriptVisual Script

`[](#__codelineno-4-1)equip_item(hero(0), equipment(1), equip_slot(0), require_unequipped);`

`[](#__codelineno-5-1){"Data":{"Equipment":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"EquipmentSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IgnoreConstraints":0,"IsConstrainedToUnequipped":1,"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.EquipItemCommand"}`