# Spawn Vehicle

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/100-spawn-vehicle/*

---

# Spawn Vehicle

## **Spawn Vehicle**[¶](#spawn-vehicle "Permanent link")

Spawns a vehicle from the database at a specified position on a map.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Map ID

The ID of the map to spawn the vehicle on.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the spawned vehicle's unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Store ID

Whether to store the unique ID of the spawned vehicle in a variable.

Toggle

Vehicle

The vehicle definition from the database to spawn.

[Variable or Value](../../../05-reference/variable-or-value/)

X

The X coordinate to spawn the vehicle at.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y coordinate to spawn the vehicle at.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z coordinate to spawn the vehicle at.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Spawn Vehicle 0 on Map 1 at Position (5, 0, 5)**[¶](#spawn-vehicle-0-on-map-1-at-position-5-0-5 "Permanent link")

This spawns vehicle definition 0 on map 1 at coordinates (5, 0, 5).

Code ScriptVisual Script

`[](#__codelineno-0-1)spawn_vehicle(0, 1, 5, 0, 5);`

`[](#__codelineno-1-1){"Data":{"MapID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"VehicleID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.VehicleSpawnVehicleCommand"}`