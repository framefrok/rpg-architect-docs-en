# Sell To Shop

*Источник: https://docs.rpg-architect.com/07-commands/21-shop/12-sell-to-shop/*

---

# Sell To Shop

## **Sell To Shop**[¶](#sell-to-shop "Permanent link")

Sells an item from the party's inventory to the currently open shop.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Result

The switch to store whether the sale succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Shop Item

The variable referencing the shop item to operate on.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the sale attempt is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Sell an Item to the Shop**[¶](#sell-an-item-to-the-shop "Permanent link")

This sells the item referenced by Global Variable 0 to the currently open shop.

Code ScriptVisual Script

`[](#__codelineno-0-1)sell($gv[0]);`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.SellToShopCommand"}`

#### **Sell an Item and Store Whether the Sale Succeeded**[¶](#sell-an-item-and-store-whether-the-sale-succeeded "Permanent link")

This sells the item referenced by Local Variable 1 to the shop and stores whether the sale succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = sell($lv[1]);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.SellToShopCommand"}`