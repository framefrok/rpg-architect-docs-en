# Refresh Overlay

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/05-refresh-overlay/*

---

# Refresh Overlay

## **Refresh Overlay**[¶](#refresh-overlay "Permanent link")

Refreshes the context of an open overlay, causing it to reload its data.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Overlay ID

The unique ID of the overlay to refresh.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Refresh an Overlay by Unique ID in Global Variable 0**[¶](#refresh-an-overlay-by-unique-id-in-global-variable-0 "Permanent link")

This refreshes the overlay whose unique ID is stored in Global Variable 0, causing it to reload its data.

Code ScriptVisual Script

`[](#__codelineno-0-1)refresh_overlay($gv[0]);`

`[](#__codelineno-1-1){"Data":{"OverlayID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.RefreshOverlayCommand"}`