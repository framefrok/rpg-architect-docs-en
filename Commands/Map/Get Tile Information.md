# Get Tile Information

*Источник: https://docs.rpg-architect.com/07-commands/11-map/04-get-tile-information/*

---

# Get Tile Information

## **Get Tile Information**[¶](#get-tile-information "Permanent link")

Retrieves details about a tile at the specified coordinates, such as its region, collision, height, shape, or tile tag. Optionally targets a specific layer directly instead of locating the tile by its Y position.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Collision

Whether to retrieve the collision value of the tile.

Toggle

Height

Whether to retrieve the height value of the tile.

Toggle

Layer

The layer to read the tile from when Use Layer is enabled, referenced by its unique ID.

[Variable or Value](../../../05-reference/variable-or-value/)

Region

Whether to retrieve the region value of the tile.

Toggle

Result

The variable to store the tile information result in.

[Variable or Value](../../../05-reference/variable-or-value/)

Shape

Whether to retrieve the shape value of the tile.

Toggle

Strategy

The strategy used to find a tile based on the Y position: Down (at or below), Up (at or above), or Closest (nearest). Only used when Use Layer is disabled.

[Tile Location Strategy](#tile-location-strategy)

Tile Tag

Whether to retrieve the tile tag value of the tile.

Toggle

Use Layer

Whether to read the tile from a specific layer directly, ignoring the Y coordinate and strategy.

Toggle

X

The X coordinate of the tile to inspect.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y coordinate of the tile to inspect.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z coordinate of the tile to inspect.

[Variable or Value](../../../05-reference/variable-or-value/)

#### **[Tile Location Strategy](#tile-location-strategy)**[¶](#tile-location-strategy "Permanent link")

Name

Explanation

Down

Finds the nearest tile at or below the current Y position.

Up

Finds the nearest tile at or above the current Y position.

Closest

Finds the nearest tile in either direction from the current Y position.

## **Examples**[¶](#examples "Permanent link")

#### **Get Tile Collision at Position (5, 0, 5)**[¶](#get-tile-collision-at-position-5-0-5 "Permanent link")

This retrieves the collision value of the tile at coordinates (5, 0, 5) using the closest layer, and stores the result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = get_tile_info(5, 0, 5, collision, closest);`

`[](#__codelineno-1-1){"Data":{"IsCollision":1,"IsHeight":0,"IsRegion":0,"IsShape":0,"IsTileTag":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"LocationStrategy":2,"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapTileGetDetailsCommand"}`

#### **Get Tile Height at Variable Position, Looking Down**[¶](#get-tile-height-at-variable-position-looking-down "Permanent link")

This retrieves the height of the tile at coordinates from Global Variables 0 through 2, searching downward, and stores the result in Global Variable 3.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[3] = get_tile_info($gv[0], $gv[1], $gv[2], height, down);`

`[](#__codelineno-3-1){"Data":{"IsCollision":0,"IsHeight":1,"IsRegion":0,"IsShape":0,"IsTileTag":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":3,"Metadata":null},"LocationStrategy":0,"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Z":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapTileGetDetailsCommand"}`