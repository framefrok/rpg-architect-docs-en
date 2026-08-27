# Add Weather

*Источник: https://docs.rpg-architect.com/07-commands/11-map/200-add-weather/*

---

# Add Weather

## **Add Weather**[¶](#add-weather "Permanent link")

Adds a weather effect from the database to the current map scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Input Switches

The input switches to pass to the weather effect.

[Switch or Value](../../../05-reference/switch-or-value/)

Input Variables

The input variables to pass to the weather effect.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the weather effect's unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Skip Enter Script

Whether to skip the weather effect's enter script when adding it.

Toggle

Store ID

Whether to store the weather effect's unique ID in a variable for later reference.

Toggle

Weather

The index of the weather effect in the database to add.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Add Weather Effect from Database Index 5**[¶](#add-weather-effect-from-database-index-5 "Permanent link")

This adds the weather effect at database index 5 to the current map.

Code ScriptVisual Script

`[](#__codelineno-0-1)add_weather(5);`

`[](#__codelineno-1-1){"Data":{"InputSwitches":[],"InputVariables":[],"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SkipEnterScript":0,"StoreID":0,"WeatherIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherAddCommand"}`

#### **Add Weather with Input Data, Skipping Enter Script**[¶](#add-weather-with-input-data-skipping-enter-script "Permanent link")

This adds the weather effect at database index 5, passing in switch and variable inputs, and skipping the weather's enter script.

Code ScriptVisual Script

`[](#__codelineno-2-1)add_weather(5, switches: [true, false], variables: [100, $gv[0]], skip_script);`

`[](#__codelineno-3-1){"Data":{"InputSwitches":[{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null}],"InputVariables":[{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null}],"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SkipEnterScript":1,"StoreID":0,"WeatherIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherAddCommand"}`