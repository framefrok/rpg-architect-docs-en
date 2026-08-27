# Open Overlay

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/02-open-overlay/*

---

# Open Overlay

## **Open Overlay**[¶](#open-overlay "Permanent link")

Opens a new overlay user interface, optionally storing its unique ID in a variable.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Local

Whether the variable used to store the unique ID is local.

Toggle

Overlay

The overlay user interface to display.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

Store ID

Whether to store the opened overlay's unique ID in a variable for later reference.

Toggle

Variable Index

The index of the variable to store the overlay's unique ID in.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Open an Overlay User Interface**[¶](#open-an-overlay-user-interface "Permanent link")

This opens the overlay identified by the given unique ID.

Code ScriptVisual Script

`[](#__codelineno-0-1)open_overlay("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-1-1){"Data":{"Index":0,"IsLocal":0,"OverlayID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","StoreID":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.OpenOverlayCommand"}`

#### **Open an Overlay and Store Its Unique ID in Global Variable 0**[¶](#open-an-overlay-and-store-its-unique-id-in-global-variable-0 "Permanent link")

This opens the overlay and stores its runtime unique ID in Global Variable 0 for later reference.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = open_overlay("a1b2c3d4-e5f6-7890-abcd-ef1234567890");`

`[](#__codelineno-3-1){"Data":{"Index":0,"IsLocal":0,"OverlayID":"a1b2c3d4-e5f6-7890-abcd-ef1234567890","StoreID":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.OpenOverlayCommand"}`