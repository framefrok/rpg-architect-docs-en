# Adjust Map Layer

*Источник: https://docs.rpg-architect.com/07-commands/11-map/40-adjust-map-layer/*

---

# Adjust Map Layer

## **Adjust Map Layer**[¶](#adjust-map-layer "Permanent link")

Modifies the visual properties of a map layer, such as its color mask and opacity.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the layer.

Color

Map Layer

The map layer to adjust. Use 0 for the base layer, positive numbers for upper layers, and negative numbers for lower layers.

[Variable or Value](../../../05-reference/variable-or-value/)

Opacity

The opacity of the layer, from 0 (fully transparent) to 1 (fully opaque).

[Variable or Value](../../../05-reference/variable-or-value/)

Use Color Mask

Whether to apply the color mask to the layer.

Toggle

Use Opacity

Whether to apply the opacity value to the layer.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Apply a Red Color Mask to Layer 1**[¶](#apply-a-red-color-mask-to-layer-1 "Permanent link")

This applies a red color mask to the first upper map layer (parallax layers only).

Code ScriptVisual Script

`[](#__codelineno-0-1)adjust_map_layer(1, color: #FF0000);`

`[](#__codelineno-1-1){"Data":{"ColorMask":"1,0,0,1","MapLayer":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"UseColorMask":1,"UseOpacity":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLayerAdjustmentCommand"}`

#### **Set Layer Opacity to 50 Percent Using a Variable**[¶](#set-layer-opacity-to-50-percent-using-a-variable "Permanent link")

This sets the opacity of the map layer specified by Global Variable 0 to 0.5 (50%).

Code ScriptVisual Script

`[](#__codelineno-2-1)adjust_map_layer($gv[0], opacity: 0.5);`

`[](#__codelineno-3-1){"Data":{"ColorMask":"1,1,1,1","MapLayer":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"UseColorMask":0,"UseOpacity":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLayerAdjustmentCommand"}`