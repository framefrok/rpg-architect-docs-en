# Adjust Lighting

*Источник: https://docs.rpg-architect.com/07-commands/11-map/1000-adjust-lighting/*

---

# Adjust Lighting

## **Adjust Lighting**[¶](#adjust-lighting "Permanent link")

Modifies the map's ambient and directional lighting settings, including colors and light direction.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Ambient Color

The color of the ambient light applied to the map.

Color

Ambient Color Enabled

Whether the ambient light color is updated by this command.

Toggle

Direction X

The X component of the directional light direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Y

The Y component of the directional light direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Direction Z

The Z component of the directional light direction vector.

[Variable or Value](../../../05-reference/variable-or-value/)

Directional Color

The color of the directional light applied to the map.

Color

Directional Color Enabled

Whether the directional light color is updated by this command.

Toggle

Directional Light Direction Enabled

Whether the directional light direction is updated by this command.

Toggle

Is Enabled

Whether the lighting toggle is updated by this command.

Toggle

Is Lighting Active

Whether lighting is active on the map.

Toggle

Reset to Default

Whether to reset the lighting to the map's default configuration.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Set the Ambient Light Color to White**[¶](#set-the-ambient-light-color-to-white "Permanent link")

This sets the ambient light color on the map to white.

Code ScriptVisual Script

`[](#__codelineno-0-1)adjust_lighting(ambient: #FFFFFF);`

`[](#__codelineno-1-1){"Data":{"AmbientLightColor":"1,1,1,1","DirectionalLightColor":"1,1,1,1","DirectionalLightDirectionX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-1","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAmbientLightColorEnabled":1,"IsDirectionalLightColorEnabled":0,"IsDirectionalLightDirectionEnabled":0,"IsToggle":1,"IsToggleEnabled":0,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLightingAdjustmentCommand"}`

#### **Set Ambient Color and Enable Lighting**[¶](#set-ambient-color-and-enable-lighting "Permanent link")

This sets the ambient light color to white and enables lighting on the map.

Code ScriptVisual Script

`[](#__codelineno-2-1)adjust_lighting(ambient: #FFFFFF, enable);`

`[](#__codelineno-3-1){"Data":{"AmbientLightColor":"1,1,1,1","DirectionalLightColor":"1,1,1,1","DirectionalLightDirectionX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-1","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAmbientLightColorEnabled":1,"IsDirectionalLightColorEnabled":0,"IsDirectionalLightDirectionEnabled":0,"IsToggle":1,"IsToggleEnabled":1,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLightingAdjustmentCommand"}`

#### **Reset Lighting to Map Defaults**[¶](#reset-lighting-to-map-defaults "Permanent link")

This resets all lighting properties to the map's default configuration.

Code ScriptVisual Script

`[](#__codelineno-4-1)adjust_lighting(reset);`

`[](#__codelineno-5-1){"Data":{"AmbientLightColor":"1,1,1,1","DirectionalLightColor":"1,1,1,1","DirectionalLightDirectionX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-1","VariableIndex":0,"Metadata":null},"DirectionalLightDirectionZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsAmbientLightColorEnabled":0,"IsDirectionalLightColorEnabled":0,"IsDirectionalLightDirectionEnabled":0,"IsToggle":1,"IsToggleEnabled":0,"IsReset":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapLightingAdjustmentCommand"}`