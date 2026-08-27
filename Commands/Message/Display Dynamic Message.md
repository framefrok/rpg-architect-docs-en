# Display Dynamic Message

*Источник: https://docs.rpg-architect.com/07-commands/04-message/01-display-dynamic-message/*

---

# Display Dynamic Message

## **Display Dynamic Message**[¶](#display-dynamic-message "Permanent link")

Displays a speech bubble that can optionally track and follow an entity on screen.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Anchor

The anchor direction for positioning the message bubble relative to the target entity.

[Direction](../../../05-reference/direction/)

Audio

The audio clip to play when the message is displayed.

[Sound Effect](../../../05-reference/sound-effect/)

Block Input

When enabled, player input is blocked while the message is displayed.

Toggle

Body

The main message text to display in the speech bubble.

String

Constrain Message Area

When enabled, the message bubble is constrained to a fixed screen area instead of following the target.

Toggle

Constrained Area

The fixed screen area to constrain the message bubble within.

Rectangle

Dismissable

When enabled, the player can dismiss the message by pressing the confirm key.

Toggle

Duration

The auto-dismiss duration in milliseconds. A value of 0 means the message will not auto-dismiss.

[Variable or Value](../../../05-reference/variable-or-value/)

Header

The header text displayed at the top of the speech bubble.

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

Padding

The padding in pixels between the target's bounding box edge and the message bubble.

[Variable or Value](../../../05-reference/variable-or-value/)

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

Target

The actor the speech bubble is attached to and follows on screen.

[Actor Reference](../../../05-reference/actor-reference/)

Target

When enabled, the speech bubble is attached to a specific actor on the map.

Toggle

Use Portrait Expression

When enabled, a portrait expression is applied to the hero's portrait.

Toggle

#### **[Anchor](#anchor)**[¶](#anchor "Permanent link")

Name

Explanation

None

No anchor positioning.

Center

Anchors to the center of the target.

Left

Anchors to the left side of the target.

Top

Anchors to the top of the target.

Right

Anchors to the right side of the target.

Bottom

Anchors to the bottom of the target.

## **Examples**[¶](#examples "Permanent link")

#### **Display a Speech Bubble on the Current Entity**[¶](#display-a-speech-bubble-on-the-current-entity "Permanent link")

This displays a speech bubble attached to the current entity (self) with default settings.

Code ScriptVisual Script

`[](#__codelineno-0-1)dynamic_message("Hello!", self);`

`[](#__codelineno-1-1){"Data":{"Anchor":3,"Body":"Hello!","ConstrainedArea":"0,0,0,0","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Header":"","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Padding":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"IsDismissable":1,"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"UseConstrainedArea":0,"UseHeroReference":0,"UsePortraitExpressionReference":0,"UseTarget":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DynamicMessageCommand"}`

#### **Display a Timed Speech Bubble on an Entity**[¶](#display-a-timed-speech-bubble-on-an-entity "Permanent link")

This displays a speech bubble on entity 0 that automatically dismisses after 3000 milliseconds and cannot be dismissed manually.

Code ScriptVisual Script

`[](#__codelineno-2-1)dynamic_message("Watch out!", entity(0), duration: 3000, dismissable: false);`

`[](#__codelineno-3-1){"Data":{"Anchor":3,"Body":"Watch out!","ConstrainedArea":"0,0,0,0","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3000","VariableIndex":0,"Metadata":null},"Header":"","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Padding":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"IsDismissable":0,"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"UseConstrainedArea":0,"UseHeroReference":0,"UsePortraitExpressionReference":0,"UseTarget":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DynamicMessageCommand"}`

#### **Display a Speech Bubble and Store Its Unique Identifier**[¶](#display-a-speech-bubble-and-store-its-unique-identifier "Permanent link")

This displays a speech bubble on a party member with a bottom anchor and stores the message unique ID in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = dynamic_message("Follow me!", party(0), anchor: bottom);`

`[](#__codelineno-5-1){"Data":{"Anchor":5,"Body":"Follow me!","ConstrainedArea":"0,0,0,0","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Header":"","HeroReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Padding":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"IsDismissable":1,"Portrait":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":null,"SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"PortraitExpressionReference":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"UseConstrainedArea":0,"UseHeroReference":0,"UsePortraitExpressionReference":0,"UseTarget":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DynamicMessageCommand"}`