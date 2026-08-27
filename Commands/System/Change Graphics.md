# Change Graphics

*Источник: https://docs.rpg-architect.com/07-commands/20-system/50-change-graphics/*

---

# Change Graphics

## **Change Graphics**[¶](#change-graphics "Permanent link")

Modifies the display settings of the game, including fullscreen mode, internal resolution, and viewport resolution.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Fullscreen Enabled

Whether the fullscreen setting is applied by this command.

Toggle

Height

The height of the internal rendering resolution in pixels.

[Variable or Value](../../../05-reference/variable-or-value/)

Is Fullscreen

Whether the game should run in fullscreen mode.

[Switch or Value](../../../05-reference/switch-or-value/)

Resolution Enabled

Whether the internal resolution setting is applied by this command.

Toggle

Use Viewport Resolution

Whether to use a custom viewport resolution instead of the default window size.

[Switch or Value](../../../05-reference/switch-or-value/)

Viewport Height

The height of the viewport or window in pixels.

[Variable or Value](../../../05-reference/variable-or-value/)

Viewport Resolution Enabled

Whether the viewport resolution setting is applied by this command.

Toggle

Viewport Width

The width of the viewport or window in pixels.

[Variable or Value](../../../05-reference/variable-or-value/)

Width

The width of the internal rendering resolution in pixels.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Enable Fullscreen Mode**[¶](#enable-fullscreen-mode "Permanent link")

Switches the game display to fullscreen mode.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_graphics(fullscreen: true);`

`[](#__codelineno-1-1){"Data":{"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsFullscreenEnabled":1,"IsResolutionEnabled":0,"IsViewportResolutionEnabled":0,"ResolutionHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"480","VariableIndex":0,"Metadata":null},"ResolutionWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"640","VariableIndex":0,"Metadata":null},"UseViewportResolution":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"ViewportHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"480","VariableIndex":0,"Metadata":null},"ViewportWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"640","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGraphicsCommand"}`

#### **Change Internal Resolution**[¶](#change-internal-resolution "Permanent link")

Sets the internal rendering resolution to 1280 by 720 pixels.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_graphics(width: 1280, height: 720);`

`[](#__codelineno-3-1){"Data":{"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsFullscreenEnabled":0,"IsResolutionEnabled":1,"IsViewportResolutionEnabled":0,"ResolutionHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"720","VariableIndex":0,"Metadata":null},"ResolutionWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1280","VariableIndex":0,"Metadata":null},"UseViewportResolution":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"ViewportHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"480","VariableIndex":0,"Metadata":null},"ViewportWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"640","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGraphicsCommand"}`

#### **Enable Viewport Resolution with Custom Size**[¶](#enable-viewport-resolution-with-custom-size "Permanent link")

Enables a custom viewport resolution of 1920 by 1080 pixels.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_graphics(viewport: true, viewport_width: 1920, viewport_height: 1080);`

`[](#__codelineno-5-1){"Data":{"IsFullscreen":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsFullscreenEnabled":0,"IsResolutionEnabled":0,"IsViewportResolutionEnabled":1,"ResolutionHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"480","VariableIndex":0,"Metadata":null},"ResolutionWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"640","VariableIndex":0,"Metadata":null},"UseViewportResolution":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"ViewportHeight":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1080","VariableIndex":0,"Metadata":null},"ViewportWidth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1920","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGraphicsCommand"}`