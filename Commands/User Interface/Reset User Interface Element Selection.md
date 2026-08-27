# Reset User Interface Element Selection

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/103-reset-user-interface-element-selection/*

---

# Reset User Interface Element Selection

## **Reset User Interface Element Selection**[¶](#reset-user-interface-element-selection "Permanent link")

Resets the selection state of a specific user interface element, clearing any currently selected item.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

User Interface Element

The unique ID of the user interface element to reset the selection on.

[User Interface Element](../../../10-user-interfaces/user-interface-element/)

## **Examples**[¶](#examples "Permanent link")

#### **Reset the Selection on a User Interface Element**[¶](#reset-the-selection-on-a-user-interface-element "Permanent link")

This resets the selection state of the user interface element identified by the given unique ID.

Code ScriptVisual Script

`[](#__codelineno-0-1)reset_ui_element_selection("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-1-1){"Data":{"ID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.ResetUserInterfaceElementSelectionCommand"}`