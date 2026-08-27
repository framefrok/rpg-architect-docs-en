# Display Dialogue Options

*Источник: https://docs.rpg-architect.com/07-commands/04-message/03-display-dialogue-options/*

---

# Display Dialogue Options

## **Display Dialogue Options**[¶](#display-dialogue-options "Permanent link")

Displays a dialogue box with multiple options for the player to choose from, each with its own set of commands to execute.

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

Canceled Commands

The commands to execute when the player cancels the dialogue.

[Script](../../../05-reference/script/)

Dialogue Template

The user interface template used to render the dialogue options.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

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

#### **Display a Simple Dialogue with Two Choices**[¶](#display-a-simple-dialogue-with-two-choices "Permanent link")

This displays a dialogue box with two options, each executing different commands when selected.

Code ScriptVisual Script

`[](#__codelineno-0-1)dialogue_options() { [](#__codelineno-0-2)    case ("Accept") { [](#__codelineno-0-3)    } [](#__codelineno-0-4)    case ("Decline") { [](#__codelineno-0-5)    } [](#__codelineno-0-6)}`

`[](#__codelineno-1-1){"Data":{"UserInterfaceID":"00000000-0000-0000-0000-000000000000","CanceledCommands":[],"IsTimeConstrained":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":0,"IsMaintainingLastMessage":0,"Offset":"0,0","Options":[{"Commands":[],"Conditions":[],"IsCancelationSet":0,"Name":"Accept","Metadata":null},{"Commands":[],"Conditions":[],"IsCancelationSet":0,"Name":"Decline","Metadata":null}],"IsBlockingInput":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DialogueOptionsCommand"}`

#### **Display Dialogue Options with a Cancel Handler**[¶](#display-dialogue-options-with-a-cancel-handler "Permanent link")

This displays a dialogue with a conditional option and a default cancel handler that runs when the player presses cancel.

Code ScriptVisual Script

`[](#__codelineno-2-1)dialogue_options(maintain_last_message) { [](#__codelineno-2-2)    case ("Yes") { [](#__codelineno-2-3)    } [](#__codelineno-2-4)    case ("No") { [](#__codelineno-2-5)    } [](#__codelineno-2-6)    default { [](#__codelineno-2-7)    } [](#__codelineno-2-8)}`

`[](#__codelineno-3-1){"Data":{"UserInterfaceID":"00000000-0000-0000-0000-000000000000","CanceledCommands":[],"IsTimeConstrained":1,"AudioMessage":{"Name":null,"Pan":0,"Pitch":0,"Volume":1,"IsPreventingMultiple":false},"IsCancelable":1,"IsMaintainingLastMessage":1,"Offset":"0,0","Options":[{"Commands":[],"Conditions":[],"IsCancelationSet":0,"Name":"Yes","Metadata":null},{"Commands":[],"Conditions":[],"IsCancelationSet":0,"Name":"No","Metadata":null}],"IsBlockingInput":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Message.DialogueOptionsCommand"}`