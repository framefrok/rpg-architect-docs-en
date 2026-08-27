# Display Static Message

*Источник: https://docs.rpg-architect.com/07-commands/04-message/00-display-static-message/*

---

# Display Static Message

## **Display Static Message**[¶](#display-static-message "Permanent link")

Displays a message box on screen with an optional portrait, header, audio, and customizable template.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Audio

The audio clip to play when the message is displayed.

[Sound Effect](../../../05-reference/sound-effect/)

Block Input

When enabled, player input is blocked while the message is displayed.

Toggle

Body

The main message text to display in the message box.

String

Header

The header text displayed at the top of the message box.

String

Hero Portrait

The hero whose portrait image is displayed alongside the message.

[Character](../../../06-database/00-characters/00-characters/)

Hero Portrait

When enabled, the portrait is sourced from a hero reference. When disabled, a custom portrait image is used.

Toggle

Is Cancelable

When enabled, the player can cancel the message or dialogue.

Toggle

Maintain Last Message Displayed

When enabled, the previous message remains visible while the dialogue is displayed.

Toggle

Message Template

The user interface template used to render the message box.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

Offset

The pixel offset applied to the message box position.

Point

Options

The list of dialogue options the player can choose from.

[Array](../../../05-reference/array/)

Portrait

A custom portrait image displayed alongside the message.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Portrait Expression

The portrait expression to apply to the hero's portrait image.

[Portrait Expression](../../../06-database/00-characters/11-portrait-expressions/)

Result

The variable to store the unique ID of the displayed message into.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Message ID

When enabled, the unique ID of the displayed message is stored in a variable for later reference.

Toggle

Use Portrait Expression

When enabled, a portrait expression is applied to the hero's portrait.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Display a Simple Static Message**[¶](#display-a-simple-static-message "Permanent link")

This displays a basic message box with the specified text.

Code ScriptVisual Script

`[](#__codelineno-0-1)static_message("Hello world");`

`[](#__codelineno-1-1){"Data":{"Body":"Hello world","Header":"","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"UseHeroReference":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"UsePortraitExpressionReference":0,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.StaticMessageCommand"}`

#### **Display a Message with Header and Hero Portrait**[¶](#display-a-message-with-header-and-hero-portrait "Permanent link")

This displays a message box with a header, using the first hero in the party as the portrait.

Code ScriptVisual Script

`[](#__codelineno-2-1)static_message("Welcome to the castle.", header: "Guard", hero: hero(0));`

`[](#__codelineno-3-1){"Data":{"Body":"Welcome to the castle.","Header":"Guard","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"UseHeroReference":1,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"UsePortraitExpressionReference":0,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.StaticMessageCommand"}`

#### **Display a Message and Store Its Unique Identifier**[¶](#display-a-message-and-store-its-unique-identifier "Permanent link")

This displays a message with input enabled and stores the resulting unique ID in global variable 0 for later dismissal.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = static_message("Press any key to continue.", enable_input);`

`[](#__codelineno-5-1){"Data":{"Body":"Press any key to continue.","Header":"","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"UseHeroReference":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":1,"UsePortraitExpressionReference":0,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":0,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.StaticMessageCommand"}`