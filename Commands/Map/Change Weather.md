# Change Weather

*Источник: https://docs.rpg-architect.com/07-commands/11-map/201-change-weather/*

---

# Change Weather

## **Change Weather**[¶](#change-weather "Permanent link")

Modifies the input switches and variables of an existing weather effect identified by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Input Switches

The input switches to update on the weather effect.

[Switch or Value](../../../05-reference/switch-or-value/)

Input Variables

The input variables to update on the weather effect.

[Variable or Value](../../../05-reference/variable-or-value/)

Weather Unique ID

The unique ID of the weather effect to modify. This is the ID returned when the weather effect was added.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Change Weather Instance Using Unique ID from Global Variable 0**[¶](#change-weather-instance-using-unique-id-from-global-variable-0 "Permanent link")

This changes the weather instance identified by the Unique ID stored in Global Variable 0, passing updated switch and variable inputs.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_weather($gv[0], switches: [true], variables: [50]);`

`[](#__codelineno-1-1){"Data":{"InputSwitches":[{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null}],"InputVariables":[{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"50","VariableIndex":0,"Metadata":null}],"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapWeatherChangeCommand"}`