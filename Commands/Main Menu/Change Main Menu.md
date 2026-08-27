# Change Main Menu

*Источник: https://docs.rpg-architect.com/07-commands/16-main-menu/05-change-main-menu/*

---

# Change Main Menu

## **Change Main Menu**[¶](#change-main-menu "Permanent link")

Changes the main menu user interface for the current map scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Menu

The menu user interface to assign as the main menu for the current scene.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

## **Examples**[¶](#examples "Permanent link")

#### **Change the Main Menu to a Different User Interface**[¶](#change-the-main-menu-to-a-different-user-interface "Permanent link")

This changes the main menu for the current map scene to the user interface identified by the given unique ID.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_main_menu("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-1-1){"Data":{"MenuID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.MainMenu.SetMainMenuCommand"}`