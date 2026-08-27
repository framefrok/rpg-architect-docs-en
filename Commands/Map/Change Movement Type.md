# Change Movement Type

*Источник: https://docs.rpg-architect.com/07-commands/11-map/08-change-movement-type/*

---

# Change Movement Type

## **Change Movement Type**[¶](#change-movement-type "Permanent link")

Switches the map engine between pixel-based and tile-based movement modes.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Pixel-Based Movement

Whether the movement is conducted via pixels, allowing smooth sub-tile positioning.

Toggle

Reset to Default

Whether to reset the movement type to the default configured in the database.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Switch to Pixel-Based Movement**[¶](#switch-to-pixel-based-movement "Permanent link")

This switches the map engine to pixel-based movement, allowing smooth sub-tile positioning.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_movement_type(pixel);`

`[](#__codelineno-1-1){"Data":{"IsPixelBasedMovement":1,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapChangeMovementCommand"}`

#### **Switch to Tile-Based Movement**[¶](#switch-to-tile-based-movement "Permanent link")

This switches the map engine to tile-based movement, snapping to tile grid positions.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_movement_type(tile);`

`[](#__codelineno-3-1){"Data":{"IsPixelBasedMovement":0,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapChangeMovementCommand"}`

#### **Reset Movement Type to Default**[¶](#reset-movement-type-to-default "Permanent link")

This resets the movement type to the default configured in the database.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_movement_type(reset);`

`[](#__codelineno-5-1){"Data":{"IsPixelBasedMovement":1,"IsReset":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapChangeMovementCommand"}`