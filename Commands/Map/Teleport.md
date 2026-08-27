# Teleport

*Источник: https://docs.rpg-architect.com/07-commands/11-map/00-teleport/*

---

# Teleport

## **Teleport**[¶](#teleport "Permanent link")

Moves the player from one map to another, or to an existing location on the same map without reloading it.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Direction

The direction the party faces upon arrival. When left empty, the current direction is kept.

[Direction](../../../05-reference/direction/)

Map ID

The ID of the map to teleport to.

[Variable or Value](../../../05-reference/variable-or-value/)

X

The X coordinate on the map.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y coordinate on the map.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z coordinate on the map.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Teleport to Map 0 at Position (5, 0, 5)**[¶](#teleport-to-map-0-at-position-5-0-5 "Permanent link")

This command teleports the player to a fixed location, without any variable data.

Code ScriptVisual Script

`[](#__codelineno-0-1)teleport(0, 5, 0, 5);`

`[](#__codelineno-1-1){"Data":{"MapID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapTeleportCommand"}`

#### **Teleport Using Global Variables for Map and Coordinates**[¶](#teleport-using-global-variables-for-map-and-coordinates "Permanent link")

This command teleports the player to a variable location, determined by Global Variables 0 through 3.

Code ScriptVisual Script

`[](#__codelineno-2-1)teleport($gv[0], $gv[1], $gv[2], $gv[3]);`

`[](#__codelineno-3-1){"Data":{"MapID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Z":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":3,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapTeleportCommand"}`