# Dismiss Message

*Источник: https://docs.rpg-architect.com/07-commands/04-message/02-dismiss-message/*

---

# Dismiss Message

## **Dismiss Message**[¶](#dismiss-message "Permanent link")

Dismisses one or all active dynamic message boxes currently displayed on screen.

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

Dismiss All Dynamic Messages

When enabled, all active dynamic messages are dismissed. When disabled, only the message matching the specified unique ID is dismissed.

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

Message Unique ID

The unique ID of the specific message to dismiss. Ignored when dismissing all messages.

[Variable or Value](../../../05-reference/variable-or-value/)

Offset

The pixel offset applied to the message box position.

Point

Options

The list of dialogue options the player can choose from.

[Array](../../../05-reference/array/)

## **Examples**[¶](#examples "Permanent link")

#### **Dismiss All Active Dynamic Messages**[¶](#dismiss-all-active-dynamic-messages "Permanent link")

This dismisses all currently active dynamic message boxes on screen.

Code ScriptVisual Script

`[](#__codelineno-0-1)dismiss_message();`

`[](#__codelineno-1-1){"Data":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsDismissingAll":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DismissMessageCommand"}`

#### **Dismiss a Specific Message by Unique Identifier**[¶](#dismiss-a-specific-message-by-unique-identifier "Permanent link")

This dismisses only the message whose unique ID was previously stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)dismiss_message($gv[0]);`

`[](#__codelineno-3-1){"Data":{"Identifier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsDismissingAll":0,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DismissMessageCommand"}`