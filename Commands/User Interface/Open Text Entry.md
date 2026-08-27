# Open Text Entry

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/03-open-text-entry/*

---

# Open Text Entry

## **Open Text Entry**[¶](#open-text-entry "Permanent link")

Opens a text entry user interface that allows the player to type in text.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Initial Value

The initial text to populate the text entry field with.

[Variable or Value](../../../05-reference/variable-or-value/)

Picture

An image to display alongside the text entry.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Prompt

The prompt text to display to the player in the text entry.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the entered text in when the text entry is closed.

[Variable or Value](../../../05-reference/variable-or-value/)

Text Entry

The text entry user interface to open.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

## **Examples**[¶](#examples "Permanent link")

#### **Open a Text Entry User Interface**[¶](#open-a-text-entry-user-interface "Permanent link")

This opens the text entry identified by the given unique ID, storing the player's input in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = open_text_entry("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-1-1){"Data":{"InitialValue":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Picture":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"Prompt":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"TextEntryID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","Blocking":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.OpenTextEntryCommand"}`

#### **Open a Text Entry with a Prompt and Initial Value**[¶](#open-a-text-entry-with-a-prompt-and-initial-value "Permanent link")

This opens the text entry with the prompt 'Enter your name' and the initial value 'Hero', storing the result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = open_text_entry("a1b2c3d4-e5f6-7890-abcd-ef1234567890", prompt: "Enter your name", initial_value: "Hero");`

`[](#__codelineno-3-1){"Data":{"InitialValue":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"Hero","VariableIndex":0,"Metadata":null},"Picture":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"Prompt":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"Enter your name","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"TextEntryID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","Blocking":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.OpenTextEntryCommand"}`