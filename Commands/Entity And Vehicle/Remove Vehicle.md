# Remove Vehicle

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/101-remove-vehicle/*

---

# Remove Vehicle

## **Remove Vehicle**[¶](#remove-vehicle "Permanent link")

Removes a vehicle from the scene and its persistence data using its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Vehicle Unique ID

The unique ID of the vehicle to remove.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Remove Vehicle by Unique ID from Global Variable 0**[¶](#remove-vehicle-by-unique-id-from-global-variable-0 "Permanent link")

This removes the vehicle identified by the Unique ID stored in Global Variable 0 from the map.

Code ScriptVisual Script

`[](#__codelineno-0-1)remove_vehicle($gv[0]);`

`[](#__codelineno-1-1){"Data":{"VehicleUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.VehicleRemoveVehicleCommand"}`