# Display All Messages

*Источник: https://docs.rpg-architect.com/07-commands/04-message/10-display-all-messages/*

---

# Display All Messages

## **Display All Messages**[¶](#display-all-messages "Permanent link")

Instantly displays the full text of all currently active messages, skipping any text animation.

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

## **Examples**[¶](#examples "Permanent link")

#### **Instantly Display All Active Message Text**[¶](#instantly-display-all-active-message-text "Permanent link")

This skips any text animation and instantly shows the full text of all currently active messages.

Code ScriptVisual Script

`[](#__codelineno-0-1)display_all_messages();`

`[](#__codelineno-1-1){"Data":{"Name":"Display All Messages","SortOrder":10,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[],"IsBlockingInput":1,"UserInterfaceID":"00000000-0000-0000-0000-000000000000","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Message.DisplayAllMessageCommand"}`