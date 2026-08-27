# Change Game Speed

*Источник: https://docs.rpg-architect.com/07-commands/20-system/100-change-game-speed/*

---

# Change Game Speed

## **Change Game Speed**[¶](#change-game-speed "Permanent link")

Adjusts the speed multiplier that controls how fast the game runs.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Speed Multiplier

The speed multiplier to apply to the game. A value of 1.0 is normal speed.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Game Speed to Normal**[¶](#set-game-speed-to-normal "Permanent link")

Resets the game speed multiplier to the default value of 1.0.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_game_speed(1);`

`[](#__codelineno-1-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGameSpeedCommand"}`

#### **Set Game Speed to Double**[¶](#set-game-speed-to-double "Permanent link")

Sets the game speed multiplier to 2.0, making the game run twice as fast.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_game_speed(2);`

`[](#__codelineno-3-1){"Data":{"Multiplier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGameSpeedCommand"}`

#### **Set Game Speed from a Variable**[¶](#set-game-speed-from-a-variable "Permanent link")

Sets the game speed multiplier using the value stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_game_speed($gv[0]);`

`[](#__codelineno-5-1){"Data":{"Multiplier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeGameSpeedCommand"}`