# Play Video

*Источник: https://docs.rpg-architect.com/07-commands/18-video/00-play-video/*

---

# Play Video

## **Play Video**[¶](#play-video "Permanent link")

Plays a video file on screen with configurable position, size, and visual effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color Mask

The color mask to apply to the video.

Color

Fullscreen

Whether the video plays at fullscreen.

[Switch or Value](../../../05-reference/switch-or-value/)

Height

The height to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Hue Shift

The hue shift to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

ID

The ID of the video to use.

[Variable or Value](../../../05-reference/variable-or-value/)

Loop

Whether the video loops continuously.

[Switch or Value](../../../05-reference/switch-or-value/)

Opacity

The opacity to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Rotation (Degrees)

The rotation to apply to the video, in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Use Relative Positioning

Whether the video uses relative coordinates scaled to the screen resolution.

Toggle

Video

The video file to play.

[Video](../../../05-reference/video/)

Volume

The volume to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Width

The width to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

X

The X position to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y position to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

Z-Index

The Z-index to apply to the video.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Play a Fullscreen Video**[¶](#play-a-fullscreen-video "Permanent link")

Plays a video file at fullscreen using video ID 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)play_video(0, "Content/Videos/Intro.ogg");`

`[](#__codelineno-1-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VideoFile":"Content/Videos/Intro.ogg","Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.PlayVideoCommand"}`

#### **Play a Windowed Video with Custom Position and Size**[¶](#play-a-windowed-video-with-custom-position-and-size "Permanent link")

Plays a video in a window at a specific position and size using absolute coordinates.

Code ScriptVisual Script

`[](#__codelineno-2-1)play_video($gv[0], "Content/Videos/Cutscene.ogg", fullscreen: false, x: 100, y: 50, width: 640, height: 480);`

`[](#__codelineno-3-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"480","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":0,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VideoFile":"Content/Videos/Cutscene.ogg","Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"640","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"50","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.PlayVideoCommand"}`

#### **Play a Looping Video with Reduced Volume**[¶](#play-a-looping-video-with-reduced-volume "Permanent link")

Plays a looping video at half volume using relative coordinates.

Code ScriptVisual Script

`[](#__codelineno-4-1)play_video(0, "Content/Videos/Background.ogg", loop: true, relative_coordinates, volume: 0.5);`

`[](#__codelineno-5-1){"Data":{"ColorMask":"1,1,1,1","Height":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"HueShift":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsRelativeCoordinates":1,"Opacity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Rotation":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VideoFile":"Content/Videos/Background.ogg","Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"Width":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ZIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.PlayVideoCommand"}`