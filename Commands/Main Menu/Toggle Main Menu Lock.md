# Toggle Main Menu Lock

*Источник: https://docs.rpg-architect.com/07-commands/16-main-menu/03-toggle-main-menu-lock/*

---

# Toggle Main Menu Lock

## **Toggle Main Menu Lock**[¶](#toggle-main-menu-lock "Permanent link")

Toggles whether the main menu is enabled or disabled for the current map scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Is Enabled

Whether the main menu is enabled. When disabled, the player cannot open the main menu.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Disable the Main Menu**[¶](#disable-the-main-menu "Permanent link")

This disables the main menu, preventing the player from opening it.

Code ScriptVisual Script

`[](#__codelineno-0-1)toggle_main_menu(false);`

`[](#__codelineno-1-1){"Data":{"IsEnabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.MainMenu.ToggleMainMenuCommand"}`

#### **Enable the Main Menu**[¶](#enable-the-main-menu "Permanent link")

This enables the main menu, allowing the player to open it again.

Code ScriptVisual Script

`[](#__codelineno-2-1)toggle_main_menu(true);`

`[](#__codelineno-3-1){"Data":{"IsEnabled":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.MainMenu.ToggleMainMenuCommand"}`

#### **Toggle the Main Menu Based on a Global Switch**[¶](#toggle-the-main-menu-based-on-a-global-switch "Permanent link")

This sets whether the main menu is enabled based on the value of Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)toggle_main_menu($gs[0]);`

`[](#__codelineno-5-1){"Data":{"IsEnabled":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.MainMenu.ToggleMainMenuCommand"}`