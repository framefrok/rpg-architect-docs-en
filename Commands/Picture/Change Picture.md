# Change Picture

*Источник: https://docs.rpg-architect.com/07-commands/17-picture/01-change-picture/*

---

# Change Picture

## **Change Picture**[¶](#change-picture "Permanent link")

Adjusts the properties of a currently displayed picture over a duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the picture.

Color

Color Mask Enabled

Whether color mask adjustment is enabled.

Toggle

Duration (milliseconds)

The duration to adjust the picture over in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Height

The height to stretch the picture to.

[Variable or Value](../../../05-reference/variable-or-value/)

Height Enabled

Whether height adjustment is enabled.

Toggle

Hue Shift

The hue shift to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Hue Shift Enabled

Whether hue shift adjustment is enabled.

Toggle

ID

The ID of the picture to use.

[Variable or Value](../../../05-reference/variable-or-value/)

Opacity

The opacity to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Opacity Enabled

Whether opacity adjustment is enabled.

Toggle

Rotation (Degrees)

The rotation to apply to the picture, in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Rotation Enabled

Whether rotation adjustment is enabled.

Toggle

Run Asynchronously

Whether the operation runs asynchronously.

Toggle

Scale X

The X scaling to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Scale X Enabled

Whether X scaling adjustment is enabled.

Toggle

Scale Y

The Y scaling to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Scale Y Enabled

Whether Y scaling adjustment is enabled.

Toggle

Use As Delta Values

Whether to adjust the picture by this amount, rather than to the set value.

Toggle

Width

The width to stretch the picture to.

[Variable or Value](../../../05-reference/variable-or-value/)

Width Enabled

Whether width adjustment is enabled.

Toggle

X

The X position to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

Whether X position adjustment is enabled.

Toggle

Y

The Y position to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

Whether Y position adjustment is enabled.

Toggle

Z-Index

The Z-index to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Z-Index Enabled

Whether Z-index adjustment is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Move a Picture to a New Position Over One Second**[¶](#move-a-picture-to-a-new-position-over-one-second "Permanent link")

This moves picture ID stored in global variable 0 to position (200, 100) over 1000 milliseconds using delta values.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_picture($gv[0], duration: 1000, x: 200, y: 100);`

`[](#__codelineno-1-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsColorMaskEnabled":0,"IsDeltaOperation":1,"IsHeightEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":0,"IsRotationEnabled":0,"IsScaleXEnabled":0,"IsScaleYEnabled":0,"IsWidthEnabled":0,"IsXEnabled":1,"IsYEnabled":1,"IsZIndexEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"200","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ChangePictureCommand"}`

#### **Fade a Picture to Zero Opacity with Set Mode**[¶](#fade-a-picture-to-zero-opacity-with-set-mode "Permanent link")

This fades picture ID stored in global variable 0 to 0 opacity over 500 milliseconds using set mode (absolute values instead of delta).

Code ScriptVisual Script

`[](#__codelineno-2-1)change_picture($gv[0], duration: 500, set, opacity: 0);`

`[](#__codelineno-3-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsColorMaskEnabled":0,"IsDeltaOperation":0,"IsHeightEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":1,"IsRotationEnabled":0,"IsScaleXEnabled":0,"IsScaleYEnabled":0,"IsWidthEnabled":0,"IsXEnabled":0,"IsYEnabled":0,"IsZIndexEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ChangePictureCommand"}`

#### **Asynchronously Rotate a Picture**[¶](#asynchronously-rotate-a-picture "Permanent link")

This rotates picture ID 1 by 45 degrees over 500 milliseconds without blocking the script.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_picture(1, duration: 500, async, rotation: 45);`

`[](#__codelineno-5-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":1,"IsColorMaskEnabled":0,"IsDeltaOperation":1,"IsHeightEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":0,"IsRotationEnabled":1,"IsScaleXEnabled":0,"IsScaleYEnabled":0,"IsWidthEnabled":0,"IsXEnabled":0,"IsYEnabled":0,"IsZIndexEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ChangePictureCommand"}`