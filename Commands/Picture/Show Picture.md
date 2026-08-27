# Show Picture

*Источник: https://docs.rpg-architect.com/07-commands/17-picture/00-show-picture/*

---

# Show Picture

## **Show Picture**[¶](#show-picture "Permanent link")

Displays an image on screen with configurable position, scale, and visual effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the picture.

Color

Height

The height to stretch the picture to.

[Variable or Value](../../../05-reference/variable-or-value/)

Height Enabled

Whether to use a custom height for the picture.

Toggle

Hue Shift

The hue shift to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

ID

The ID of the picture to use.

[Variable or Value](../../../05-reference/variable-or-value/)

Image

The image to use for the picture.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Opacity

The opacity to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Persist Between Scenes

Whether the picture persists between scenes.

[Switch or Value](../../../05-reference/switch-or-value/)

Rotation (Degrees)

The rotation to apply to the picture, in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Scale X

The X scaling to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Scale Y

The Y scaling to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Width

The width to stretch the picture to.

[Variable or Value](../../../05-reference/variable-or-value/)

Width Enabled

Whether to use a custom width for the picture.

Toggle

X

The X position to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y position to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

Z-Index

The Z-index to apply to the picture.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Show a Picture at a Specific Position**[¶](#show-a-picture-at-a-specific-position "Permanent link")

This displays picture ID 1 using the specified image at position (100, 50) on screen.

Code ScriptVisual Script

`[](#__codelineno-0-1)show_picture(1, "Content/Pictures/Background.png", x: 100, y: 50);`

`[](#__codelineno-1-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Image":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":"Content/Pictures/Background.png","SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":1,"SpriteLayers":{},"SpriteOrientation":1,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"IsHeightEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsWidthEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"50","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ShowPictureCommand"}`

#### **Show a Picture Using Variable References**[¶](#show-a-picture-using-variable-references "Permanent link")

This displays a picture using global variable 0 as the ID and global variables 1 and 2 for the position.

Code ScriptVisual Script

`[](#__codelineno-2-1)show_picture($gv[0], "Content/Pictures/Picture.png", x: $gv[1], y: $gv[2]);`

`[](#__codelineno-3-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Image":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":"Content/Pictures/Picture.png","SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":1,"SpriteLayers":{},"SpriteOrientation":1,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"IsHeightEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsWidthEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ShowPictureCommand"}`

#### **Show a Persistent Picture with Custom Scale and Opacity**[¶](#show-a-persistent-picture-with-custom-scale-and-opacity "Permanent link")

This displays a picture that persists between scenes with 50% opacity and doubled scale.

Code ScriptVisual Script

`[](#__codelineno-4-1)show_picture(1, "Content/Pictures/Overlay.png", x: 0, y: 0, scale_x: 2, scale_y: 2, opacity: 0.5, is_static: true);`

`[](#__codelineno-5-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Image":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":"Content/Pictures/Overlay.png","SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":1,"SpriteLayers":{},"SpriteOrientation":1,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"IsHeightEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsWidthEnabled":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ScaleX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"ScaleY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ShowPictureCommand"}`