# Clear Weather

*Источник: https://docs.rpg-architect.com/07-commands/11-map/203-clear-weather/*

---

# Clear Weather

## **Clear Weather**[¶](#clear-weather "Permanent link")

Removes all active weather effects from the current map scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Skip Exit Script

Whether to skip the weather effect's exit script when removing it.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Clear All Weather from the Map**[¶](#clear-all-weather-from-the-map "Permanent link")

This removes all active weather effects from the current map.

Code ScriptVisual Script

`[](#__codelineno-0-1)clear_weather();`

`[](#__codelineno-1-1){"Data":{"SkipExitScript":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherClearCommand"}`

#### **Clear All Weather, Skipping Exit Scripts**[¶](#clear-all-weather-skipping-exit-scripts "Permanent link")

This removes all active weather effects and skips running each weather's exit script.

Code ScriptVisual Script

`[](#__codelineno-2-1)clear_weather(skip_script);`

`[](#__codelineno-3-1){"Data":{"SkipExitScript":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherClearCommand"}`