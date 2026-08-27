# Save Value

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/05-save-value/*

---

# Save Value

## **Save Value**[¶](#save-value "Permanent link")

Saves engine-specific data from a [Data Source](../../../08-data-sources/) into a [Variable](../../../05-reference/variable/) or [Switch](../../../05-reference/switch/), connecting runtime engine data to your own data layer.

## **Source**[¶](#source "Permanent link")

Name

Explanation

Data Source

The [Data Source](../../../08-data-sources/) to save from.

## **Targets**[¶](#targets "Permanent link")

Name

Explanation

Global / Local

Targets a single [Variable](../../../05-reference/variable/).

Global / Local Range

Targets multiple contiguous [Variables](../../../05-reference/variable/).

Global / Local Reference

Targets a single [Variable](../../../05-reference/variable/) based on a [Variable](../../../05-reference/variable/) index.

## **Examples**[¶](#examples "Permanent link")

#### **Save Party Active Member Count to Global Variable 0**[¶](#save-party-active-member-count-to-global-variable-0 "Permanent link")

This retrieves the active member count from the Party data source and saves it into Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = save_value(party, active_member_count);`

`[](#__codelineno-1-1){"Data":{"IsSwitch":0,"Source":{"$":"PartyDataSource","ParameterIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"PartyProperty":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SaveValueCommand"}`

#### **Save Party Member Unique ID, Based on Global Variable 1, to Global Variable 0**[¶](#save-party-member-unique-id-based-on-global-variable-1-to-global-variable-0 "Permanent link")

This retrieves the Unique ID of a party member at a position specified by Global Variable 1, from all members in the Party data source, and saves it into Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = save_value(party, member_unique_id, $gv[1]);`

`[](#__codelineno-3-1){"Data":{"IsSwitch":0,"Source":{"$":"PartyDataSource","ParameterIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"PartyProperty":12,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SaveValueCommand"}`

#### **Save Inventory Slot Usability Flag to Global Switch 0, Based on Global Variable 5**[¶](#save-inventory-slot-usability-flag-to-global-switch-0-based-on-global-variable-5 "Permanent link")

This checks whether an item is usable in the menu, from an inventory slot identified by the Unique ID stored in Global Variable 5, and saves the result into Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gs[0] = save_value(inventory_slot, $gv[5], is_useable_in_menu);`

`[](#__codelineno-5-1){"Data":{"IsSwitch":1,"Source":{"$":"InventorySlotDataSource","ParameterIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"InventorySlotFlag":0,"InventorySlotProperty":0,"IsLocal":0,"SourceIndex":5,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SaveValueCommand"}`