# Change Tileset Image

*Источник: https://docs.rpg-architect.com/07-commands/11-map/10-change-tileset-image/*

---

# Change Tileset Image

## **Change Tileset Image**[¶](#change-tileset-image "Permanent link")

Replaces the image used by a tileset or an individual tileset slot at runtime.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Image Source

The path to the new image file to use for the tileset slot.

[Variable or Value](../../../05-reference/variable-or-value/)

Index

The index of the tileset or tileset slot to change.

[Variable or Value](../../../05-reference/variable-or-value/)

Slot Type

The type of tileset slot to change: Flat, Terraforming, or Structure.

[Tileset Slot Type](#tileset-slot-type)

Tileset

Whether to replace the entire tileset's images.

Toggle

Tileset Slot

Whether to replace a single slot's image in the tileset.

Toggle

#### **[Tileset Slot Type](#tileset-slot-type)**[¶](#tileset-slot-type "Permanent link")

Name

Explanation

Animated

An animated tileset slot that cycles through frames over time.

Terraforming

A terraforming tileset slot that supports auto-tiling based on neighboring tiles.

Structure

A structure tileset slot that represents multi-tile objects like buildings or trees.

Normal

A standard tileset slot for single, static tiles.

## **Examples**[¶](#examples "Permanent link")

#### **Change Tileset Image at Index 0**[¶](#change-tileset-image-at-index-0 "Permanent link")

This changes the tileset at index 0 to use the image source specified by Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_tileset_image(0, $gv[0]);`

`[](#__codelineno-1-1){"Data":{"Index":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsTileset":0,"IsTilesetSlot":1,"SlotSource":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SlotType":3,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapTilesetImageChangeCommand"}`