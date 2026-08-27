# Flash Screen

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/20-flash-screen/*

---

# Flash Screen

## **Flash Screen**[¶](#flash-screen "Permanent link")

Flashes the screen with a specified color for a given duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color

The color to flash the screen with.

Color

Duration (milliseconds)

The duration to flash the screen in milliseconds.

[Variable or Value](../../../05-reference/variable-or-value/)

Include User Interface

Whether to include the user interface in the screen flash.

Toggle

Run Asynchronously

Whether the flash runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Flash Screen White for One Second**[¶](#flash-screen-white-for-one-second "Permanent link")

Flashes the screen white for 1000 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-0-1)flash_screen(#FFFFFF, 1000);`

`[](#__codelineno-1-1){"Data":{"FlashColor":"1,1,1,1","FlashDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsUserInterfaceIncluded":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.FlashScreenCommand"}`

#### **Flash Screen Asynchronously**[¶](#flash-screen-asynchronously "Permanent link")

Flashes the screen white for 1000 milliseconds without blocking subsequent commands.

Code ScriptVisual Script

`[](#__codelineno-2-1)flash_screen(#FFFFFF, 1000, async);`

`[](#__codelineno-3-1){"Data":{"FlashColor":"1,1,1,1","FlashDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":1,"IsUserInterfaceIncluded":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.FlashScreenCommand"}`

#### **Flash Screen Including the User Interface**[¶](#flash-screen-including-the-user-interface "Permanent link")

Flashes the screen white for 1000 milliseconds including the user interface layer.

Code ScriptVisual Script

`[](#__codelineno-4-1)flash_screen(#FFFFFF, 1000, include_ui);`

`[](#__codelineno-5-1){"Data":{"FlashColor":"1,1,1,1","FlashDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsAsynchronousOperation":0,"IsUserInterfaceIncluded":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.FlashScreenCommand"}`