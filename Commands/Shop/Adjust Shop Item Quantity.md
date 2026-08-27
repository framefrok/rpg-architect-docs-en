# Adjust Shop Item Quantity

*Источник: https://docs.rpg-architect.com/07-commands/21-shop/10-adjust-shop-item-quantity/*

---

# Adjust Shop Item Quantity

## **Adjust Shop Item Quantity**[¶](#adjust-shop-item-quantity "Permanent link")

Adjusts the quantity of an item in the currently open shop.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Quantity

The amount to adjust the shop item's quantity by. Positive values increase the quantity and negative values decrease it.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The switch to store whether the quantity adjustment succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Shop Item

The variable referencing the shop item to operate on.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the quantity adjustment is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Increase a Shop Item Quantity by 1**[¶](#increase-a-shop-item-quantity-by-1 "Permanent link")

This increases the quantity of the shop item referenced by Global Variable 0 by 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)alter_shop_item_qty($gv[0], 1);`

`[](#__codelineno-1-1){"Data":{"Quantity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.AlterShopItemQuantityCommand"}`

#### **Decrease a Shop Item Quantity and Store the Result**[¶](#decrease-a-shop-item-quantity-and-store-the-result "Permanent link")

This decreases the quantity of the shop item referenced by Local Variable 1 by 3 and stores whether the adjustment succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = alter_shop_item_qty($lv[1], -3);`

`[](#__codelineno-3-1){"Data":{"Quantity":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"-3","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"ShopItem":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.AlterShopItemQuantityCommand"}`