# Adjust Camera

*Источник: https://docs.rpg-architect.com/07-commands/11-map/100-adjust-camera/*

---

# Adjust Camera

## **Adjust Camera**[¶](#adjust-camera "Permanent link")

Modifies the camera's position, rotation, scale, distance, and field of view over a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Camera Distance

The distance of the camera from the target.

[Variable or Value](../../../05-reference/variable-or-value/)

Clamp Pitch

Whether to clamp the pitch of the camera to the configured minimum and maximum values.

Toggle

Clamp Roll

Whether to clamp the roll of the camera to the configured minimum and maximum values.

Toggle

Clamp Yaw

Whether to clamp the yaw of the camera to the configured minimum and maximum values.

Toggle

Distance Enabled

Whether the camera distance adjustment is enabled.

Toggle

Duration

The duration to adjust the camera in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Field of View

The field of view of the camera in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Field of View Enabled

Whether the field of view adjustment is enabled.

Toggle

Pitch Enabled

Whether the pitch rotation adjustment is enabled.

Toggle

Roll Enabled

Whether the roll rotation adjustment is enabled.

Toggle

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Scale

The scale factor of the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Scale Enabled

Whether the scale adjustment is enabled.

Toggle

Use As Delta Values

When enabled, adjusts the camera by the specified amount relative to its current value rather than setting it to an absolute value.

Toggle

X

The X offset of the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

X (Pitch)

The pitch rotation of the camera in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

Whether the X offset adjustment is enabled.

Toggle

Y

The Y offset of the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Y (Yaw)

The yaw rotation of the camera in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

Whether the Y offset adjustment is enabled.

Toggle

Yaw Enabled

Whether the yaw rotation adjustment is enabled.

Toggle

Z

The Z offset of the camera.

[Variable or Value](../../../05-reference/variable-or-value/)

Z (Roll)

The roll rotation of the camera in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Z Enabled

Whether the Z offset adjustment is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Move Camera X Position Over 500 Milliseconds**[¶](#move-camera-x-position-over-500-milliseconds "Permanent link")

This adjusts the camera's X offset to 10 over a duration of 500 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-0-1)adjust_camera(500, x: 10);`

`[](#__codelineno-1-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"ClampPitch":0,"ClampRoll":0,"ClampYaw":0,"Distance":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"FieldOfView":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsDeltaOperation":0,"IsDistanceEnabled":0,"IsFieldOfViewEnabled":0,"IsRollEnabled":0,"IsPitchEnabled":0,"IsScaleEnabled":0,"IsXEnabled":1,"IsYEnabled":0,"IsYawEnabled":0,"IsZEnabled":0,"Pitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Roll":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Scale":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Yaw":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraAdjustmentCommand"}`

#### **Rotate Camera Pitch by 45 Degrees as Delta, Clamped**[¶](#rotate-camera-pitch-by-45-degrees-as-delta-clamped "Permanent link")

This adjusts the camera's pitch by 45 degrees relative to its current rotation over 1000 milliseconds, clamping it to configured limits.

Code ScriptVisual Script

`[](#__codelineno-2-1)adjust_camera(1000, pitch: 45, clamp_pitch, delta);`

`[](#__codelineno-3-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"ClampPitch":1,"ClampRoll":0,"ClampYaw":0,"Distance":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"FieldOfView":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsDeltaOperation":1,"IsDistanceEnabled":0,"IsFieldOfViewEnabled":0,"IsRollEnabled":0,"IsPitchEnabled":1,"IsScaleEnabled":0,"IsXEnabled":0,"IsYEnabled":0,"IsYawEnabled":0,"IsZEnabled":0,"Pitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"Roll":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Scale":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Yaw":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraAdjustmentCommand"}`

#### **Set Camera Scale Asynchronously**[¶](#set-camera-scale-asynchronously "Permanent link")

This sets the camera scale to 2 instantly (0 duration), running asynchronously so the script continues immediately.

Code ScriptVisual Script

`[](#__codelineno-4-1)adjust_camera(0, scale: 2, async);`

`[](#__codelineno-5-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ClampPitch":0,"ClampRoll":0,"ClampYaw":0,"Distance":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"FieldOfView":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":1,"IsDeltaOperation":0,"IsDistanceEnabled":0,"IsFieldOfViewEnabled":0,"IsRollEnabled":0,"IsPitchEnabled":0,"IsScaleEnabled":1,"IsXEnabled":0,"IsYEnabled":0,"IsYawEnabled":0,"IsZEnabled":0,"Pitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Roll":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Scale":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Yaw":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraAdjustmentCommand"}`