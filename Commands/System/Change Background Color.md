# Change Background Color

*Источник: https://docs.rpg-architect.com/07-commands/20-system/102-change-background-color/*

---

# Change Background Color

## **Change Background Color**[¶](#change-background-color "Permanent link")

Sets the background color of the current scene, visible behind all map layers and visual elements.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Background Color

The background color of the current scene.

Color

## **Examples**[¶](#examples "Permanent link")

#### **Set Background Color to Black**[¶](#set-background-color-to-black "Permanent link")

Changes the scene background color to solid black.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_background_color(#000000);`

`[](#__codelineno-1-1){"Data":{"BackgroundColor":"0,0,0,1","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeBackgroundColorCommand"}`

#### **Set Background Color to White**[¶](#set-background-color-to-white "Permanent link")

Changes the scene background color to solid white.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_background_color(#FFFFFF);`

`[](#__codelineno-3-1){"Data":{"BackgroundColor":"1,1,1,1","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeBackgroundColorCommand"}`

#### **Set Background Color with Full Alpha**[¶](#set-background-color-with-full-alpha "Permanent link")

Changes the scene background color to a dark blue with full opacity.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_background_color(#FF000040);`

`[](#__codelineno-5-1){"Data":{"BackgroundColor":"0,0,0.2509804,1","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.ChangeBackgroundColorCommand"}`