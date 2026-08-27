# Adjust Light

*Источник: https://docs.rpg-architect.com/07-commands/11-map/1001-adjust-light/*

---

# Adjust Light

## **Adjust Light**[¶](#adjust-light "Permanent link")

Modifies the light properties of an entity or doodad over a specified duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Duration

The duration to adjust the light in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Intensity

The intensity value of the light.

[Variable or Value](../../../05-reference/variable-or-value/)

Intensity Enabled

Whether the intensity adjustment is enabled.

Toggle

Pitch

The pitch of the light direction in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Pitch Enabled

Whether the pitch adjustment is enabled.

Toggle

Radius

The radius of the light.

[Variable or Value](../../../05-reference/variable-or-value/)

Radius Enabled

Whether the radius adjustment is enabled.

Toggle

Roll

The roll of the light in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Roll Enabled

Whether the roll adjustment is enabled.

Toggle

Run Asynchronously

Whether the adjustment runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Target

The target entity or doodad whose light to adjust.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Use As Delta Values

When enabled, adjusts the light by the specified amount relative to its current value rather than setting it to an absolute value.

Toggle

X

The X offset of the light position.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

Whether the X offset adjustment is enabled.

Toggle

Y

The Y offset of the light position.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

Whether the Y offset adjustment is enabled.

Toggle

Yaw

The yaw of the light direction in degrees.

[Variable or Value](../../../05-reference/variable-or-value/)

Yaw Enabled

Whether the yaw adjustment is enabled.

Toggle

Z

The Z offset of the light position.

[Variable or Value](../../../05-reference/variable-or-value/)

Z Enabled

Whether the Z offset adjustment is enabled.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Rotate Entity 0 Light Yaw by 45 Degrees Over 500 Milliseconds**[¶](#rotate-entity-0-light-yaw-by-45-degrees-over-500-milliseconds "Permanent link")

This adjusts the yaw of entity 0's light by 45 degrees relative to its current value over 500 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-0-1)adjust_light(entity(0), 500, yaw: 45, delta);`

`[](#__codelineno-1-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"Intensity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsDeltaOperation":1,"IsIntensityEnabled":0,"IsOffsetXEnabled":0,"IsOffsetYEnabled":0,"IsOffsetZEnabled":0,"IsPitchEnabled":0,"IsRadiusEnabled":0,"IsRollEnabled":0,"IsYawEnabled":1,"OffsetX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"OffsetY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"OffsetZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Pitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Radius":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Roll":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Yaw":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLightAdjustmentCommand"}`

#### **Set Doodad 0 Light Roll to 180 Degrees Over 1 Second**[¶](#set-doodad-0-light-roll-to-180-degrees-over-1-second "Permanent link")

This sets the roll of doodad 0's light to 180 degrees over 1000 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-2-1)adjust_light(doodad(0), 1000, roll: 180);`

`[](#__codelineno-3-1){"Data":{"AdjustmentDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"Intensity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsDeltaOperation":0,"IsIntensityEnabled":0,"IsOffsetXEnabled":0,"IsOffsetYEnabled":0,"IsOffsetZEnabled":0,"IsPitchEnabled":0,"IsRadiusEnabled":0,"IsRollEnabled":1,"IsYawEnabled":0,"OffsetX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"OffsetY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"OffsetZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Pitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Radius":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Roll":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"180","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":1,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Yaw":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLightAdjustmentCommand"}`