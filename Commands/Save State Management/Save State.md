# Save State

*Источник: https://docs.rpg-architect.com/07-commands/02-save-state-management/02-save-state/*

---

# Save State

## **Save State**[¶](#save-state "Permanent link")

Saves the current game state to the specified index, including optional data such as pictures, weather, and system settings.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Is Visible

Whether the save state is visible when listing saved games.

[Switch or Value](../../../05-reference/switch-or-value/)

Result

The switch to store whether the save operation succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Save Background Effects

When enabled, background effects playing at the time of saving are included in the save state.

[Switch or Value](../../../05-reference/switch-or-value/)

Save Pictures

When enabled, pictures displayed at the time of saving are included in the save state.

[Switch or Value](../../../05-reference/switch-or-value/)

Save Video and Audio Settings

When enabled, video and audio system settings are included in the save state.

[Switch or Value](../../../05-reference/switch-or-value/)

Save Weather

When enabled, active weather effects are included in the save state.

[Switch or Value](../../../05-reference/switch-or-value/)

State Index

The index of the save slot to write the game state to.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the save operation is stored in a switch.

Toggle

Tags

Key-value tags to associate with the save state for identification or filtering.

[Tags](../../../05-reference/tags/)

Title

The display title for the save state.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Save the Game State to Slot 1**[¶](#save-the-game-state-to-slot-1 "Permanent link")

This saves the current game state to save slot 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)save_state(1);`

`[](#__codelineno-1-1){"Data":{"IncludeBackgroundEffects":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludePictures":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeSystemSettings":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeWeather":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"StoreResults":0,"Tags":{},"Title":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.SaveStateCommand"}`

#### **Save the Game State with a Title and Pictures**[¶](#save-the-game-state-with-a-title-and-pictures "Permanent link")

This saves the current game state to the slot specified by Global Variable 0, with a custom title and including pictures.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = save_state($gv[0], title: "My Save", include_pictures);`

`[](#__codelineno-3-1){"Data":{"IncludeBackgroundEffects":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludePictures":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeSystemSettings":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeWeather":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"Tags":{},"Title":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"My Save","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.SaveStateCommand"}`

#### **Save the Game State with All Optional Data Included**[¶](#save-the-game-state-with-all-optional-data-included "Permanent link")

This saves the game state to slot 0, including pictures, weather, background effects, and system settings, with a title from Global Variable 1.

Code ScriptVisual Script

`[](#__codelineno-4-1)save_state(0, title: $gv[1], include_bg_effects, include_pictures, include_system, include_weather);`

`[](#__codelineno-5-1){"Data":{"IncludeBackgroundEffects":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludePictures":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeSystemSettings":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeWeather":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsVisible":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"StoreResults":0,"Tags":{},"Title":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.SaveStateCommand"}`