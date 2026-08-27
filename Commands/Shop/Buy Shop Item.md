# Buy Shop Item

*Источник: https://docs.rpg-architect.com/07-commands/21-shop/11-buy-shop-item/*

---

# Buy Shop Item

## **Buy Shop Item**[¶](#buy-shop-item "Permanent link")

Attempts to purchase a shop item identified by its unique ID stored in a variable.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Result

The switch to store whether the purchase succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Shop Item

The variable referencing the shop item to operate on.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the purchase attempt is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Buy a Shop Item Referenced by Global Variable 0**[¶](#buy-a-shop-item-referenced-by-global-variable-0 "Permanent link")

This attempts to purchase the shop item whose unique ID is stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)buy($gv[0]);`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.BuyShopItemCommand"}`

#### **Buy a Shop Item and Store Whether the Purchase Succeeded**[¶](#buy-a-shop-item-and-store-whether-the-purchase-succeeded "Permanent link")

This attempts to purchase the shop item referenced by Local Variable 2 and stores the result in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = buy($lv[2]);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.BuyShopItemCommand"}`