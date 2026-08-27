# Change Video

*Источник: https://docs.rpg-architect.com/07-commands/18-video/01-change-video/*

---

# Change Video

## **Change Video**[¶](#change-video "Permanent link")

Adjusts the playback properties of a currently playing video over a duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the video.

Color

Color Mask Enabled

Whether color mask adjustment is enabled.

Toggle

Duration (milliseconds)

The duration to adjust the video over in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Fullscreen

Whether to play the video at fullscreen.

[Switch or Value](../../../05-reference/switch-or-value/)

Fullscreen Enabled

Whether fullscreen adjustment is enabled.

Toggle

Height

The height to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Height Enabled

Whether height adjustment is enabled.

Toggle

Hue Shift

The hue shift to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Hue Shift Enabled

Whether hue shift adjustment is enabled.

Toggle

ID

The ID of the video to use.

[Variable or Value](../../../05-reference/variable-or-value/)

Looping

Whether to play the video in a loop.

[Switch or Value](../../../05-reference/switch-or-value/)

Looping Enabled

Whether looping adjustment is enabled.

Toggle

Opacity

The opacity to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Opacity Enabled

Whether opacity adjustment is enabled.

Toggle

Rotation (Degrees)

The rotation to apply to the video, in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Rotation Enabled

Whether rotation adjustment is enabled.

Toggle

Use As Delta Values

Whether to adjust the video by this amount, rather than to the set value.

Toggle

Use Relative Positioning

Whether the video is using relative coordinates.

Toggle

Volume

The volume to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Volume Enabled

Whether volume adjustment is enabled.

Toggle

Width

The width to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Width Enabled

Whether width adjustment is enabled.

Toggle

X

The X position to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

Whether X position adjustment is enabled.

Toggle

Y

The Y position to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

Whether Y position adjustment is enabled.

Toggle

Z-Index

The Z-index to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Z-Index Enabled

Whether Z-index adjustment is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Fade a Video to Half Opacity Over One Second**[¶](#fade-a-video-to-half-opacity-over-one-second "Permanent link")

Adjusts the opacity of a video to 0.5 over 1000 milliseconds using delta mode.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_video($gv[0], duration: 1000, opacity: 0.5);`

`[](#__codelineno-1-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsColorMaskEnabled":0,"IsDeltaOperation":1,"IsFullscreenEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":1,"IsRotationEnabled":0,"IsHeightEnabled":0,"IsLoopingEnabled":0,"IsVolumeEnabled":0,"IsWidthEnabled":0,"IsXEnabled":0,"IsYEnabled":0,"IsZIndexEnabled":0,"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.ChangeVideoCommand"}`

#### **Move a Video to a Set Position Over Half a Second**[¶](#move-a-video-to-a-set-position-over-half-a-second "Permanent link")

Moves a video to absolute coordinates using set mode with relative positioning enabled.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_video($gv[0], duration: 500, set, relative_coordinates, x: $gv[1], y: $gv[2]);`

`[](#__codelineno-3-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsColorMaskEnabled":0,"IsDeltaOperation":0,"IsFullscreenEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":0,"IsRotationEnabled":0,"IsHeightEnabled":0,"IsLoopingEnabled":0,"IsVolumeEnabled":0,"IsWidthEnabled":0,"IsXEnabled":1,"IsYEnabled":1,"IsZIndexEnabled":0,"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":1,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Y":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.ChangeVideoCommand"}`

#### **Set Video Opacity Instantly**[¶](#set-video-opacity-instantly "Permanent link")

Sets a video's opacity to a value from a variable immediately without any transition duration.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_video($gv[0], set, opacity: $gv[1]);`

`[](#__codelineno-5-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsColorMaskEnabled":0,"IsDeltaOperation":0,"IsFullscreenEnabled":0,"IsHueShiftEnabled":0,"IsOpacityEnabled":1,"IsRotationEnabled":0,"IsHeightEnabled":0,"IsLoopingEnabled":0,"IsVolumeEnabled":0,"IsWidthEnabled":0,"IsXEnabled":0,"IsYEnabled":0,"IsZIndexEnabled":0,"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":0,"Opacity":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.ChangeVideoCommand"}`