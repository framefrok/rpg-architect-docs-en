# Change Text Speed

*Источник: https://docs.rpg-architect.com/07-commands/20-system/101-change-text-speed/*

---

# Change Text Speed

## **Change Text Speed**[¶](#change-text-speed "Permanent link")

Adjusts the speed multiplier that controls how fast text is rendered.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Speed Multiplier

The speed multiplier to apply to text rendering. A value of 1.0 is normal speed.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Text Speed to Normal**[¶](#set-text-speed-to-normal "Permanent link")

Resets the text rendering speed multiplier to the default value of 1.0.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_text_speed(1);`

`[](#__codelineno-1-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeTextSpeedCommand"}`

#### **Set Text Speed to Double**[¶](#set-text-speed-to-double "Permanent link")

Sets the text rendering speed to twice the normal rate.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_text_speed(2);`

`[](#__codelineno-3-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeTextSpeedCommand"}`

#### **Set Text Speed from a Variable**[¶](#set-text-speed-from-a-variable "Permanent link")

Sets the text rendering speed multiplier using the value stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_text_speed($gv[0]);`

`[](#__codelineno-5-1){"Data":{"Multiplier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeTextSpeedCommand"}`