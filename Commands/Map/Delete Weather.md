# Delete Weather

*Источник: https://docs.rpg-architect.com/07-commands/11-map/202-delete-weather/*

---

# Delete Weather

## **Delete Weather**[¶](#delete-weather "Permanent link")

Removes a specific weather effect from the map scene by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Apply Immediately

Whether the weather effect ends immediately without a transition.

Toggle

Skip Exit Script

Whether to skip the weather effect's exit script when deleting it.

Toggle

Weather Unique ID

The unique ID of the weather effect to remove. This is the ID returned when the weather effect was added.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Delete a Specific Weather Instance by Unique ID**[¶](#delete-a-specific-weather-instance-by-unique-id "Permanent link")

This removes the weather instance identified by the Unique ID stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)delete_weather($gv[0]);`

`[](#__codelineno-1-1){"Data":{"IsImmediate":0,"SkipExitScript":0,"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherDeleteCommand"}`

#### **Delete Weather Immediately, Skipping Exit Script**[¶](#delete-weather-immediately-skipping-exit-script "Permanent link")

This immediately removes the weather instance from Global Variable 0, skipping the exit script.

Code ScriptVisual Script

`[](#__codelineno-2-1)delete_weather($gv[0], immediate, skip_script);`

`[](#__codelineno-3-1){"Data":{"IsImmediate":1,"SkipExitScript":1,"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherDeleteCommand"}`