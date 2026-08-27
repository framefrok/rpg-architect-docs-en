# Open Menu

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/00-open-menu/*

---

# Open Menu

## **Open Menu**[¶](#open-menu "Permanent link")

Opens a new menu user interface, optionally including the context of the current menu.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Global

Whether the variable used to store the unique ID is global.

Toggle

Include Context

Whether to include the context of the current menu when opening the new menu.

Toggle

Local

Whether the variable used to store the unique ID is local.

Toggle

Menu

The menu user interface to open.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

Store ID

Whether to store the opened menu's unique ID in a variable for later reference.

Toggle

Variable Index

The index of the variable to store the menu's unique ID in.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Open a Menu User Interface**[¶](#open-a-menu-user-interface "Permanent link")

This opens the menu identified by the given unique ID.

Code ScriptVisual Script

`[](#__codelineno-0-1)open_menu("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-1-1){"Data":{"IncludeContext":0,"Index":0,"IsGlobal":1,"IsLocal":0,"MenuID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","StoreID":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushMenuCommand"}`

#### **Open a Menu and Include the Current Context**[¶](#open-a-menu-and-include-the-current-context "Permanent link")

This opens the menu and passes along the context from the currently focused user interface element.

Code ScriptVisual Script

`[](#__codelineno-2-1)open_menu("a1b2c3d4-e5f6-7890-abcd-ef1234567890", include_context);`

`[](#__codelineno-3-1){"Data":{"IncludeContext":1,"Index":0,"IsGlobal":1,"IsLocal":0,"MenuID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","StoreID":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushMenuCommand"}`

#### **Open a Menu and Store Its Unique ID in Global Variable 0**[¶](#open-a-menu-and-store-its-unique-id-in-global-variable-0 "Permanent link")

This opens the menu and stores its runtime unique ID in Global Variable 0 for later reference.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = open_menu("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-5-1){"Data":{"IncludeContext":0,"Index":0,"IsGlobal":1,"IsLocal":0,"MenuID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","StoreID":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.PushMenuCommand"}`