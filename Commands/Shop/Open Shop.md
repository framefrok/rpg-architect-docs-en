# Open Shop

*Источник: https://docs.rpg-architect.com/07-commands/21-shop/00-open-shop/*

---

# Open Shop

## **Open Shop**[¶](#open-shop "Permanent link")

Opens a shop user interface, allowing the player to buy and sell items.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Local

When enabled, the shop's unique ID is stored in a local variable. When disabled, it is stored in a global variable.

Toggle

Shop

The shop configuration, including categories, items, and pricing modifiers.

[Shop](../../../06-database/03-maps/03-doodads/)

Shop Template

The user interface to use as the shop template.

[User Interface](../../../06-database/09-user-interfaces/00-user-interfaces/)

Store ID

When enabled, the shop's unique ID is stored in a variable for later reference.

Toggle

Variable Index

The variable index to store the shop's unique ID in.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Open a Shop with a User Interface Template**[¶](#open-a-shop-with-a-user-interface-template "Permanent link")

This opens a shop using the specified user interface template GUID. The shop block configures buy and sell modifiers, permissions, and item categories.

Code ScriptVisual Script

`[](#__codelineno-0-1)access_shop("00000000-0000-0000-0000-000000000001") { [](#__codelineno-0-2)    buy_modifier: 100 [](#__codelineno-0-3)    sell_modifier: 50 [](#__codelineno-0-4)    is_buy_allowed: true [](#__codelineno-0-5)    is_sell_allowed: true [](#__codelineno-0-6)};`

`[](#__codelineno-1-1){"Data":{"Index":0,"IsLocal":0,"IsTimeConstrained":1,"ShopID":"00000000-0000-0000-0000-000000000001","Shop":{"BuyModifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"Categories":[],"IsBuyAllowed":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLocal":0,"IsSellAllowed":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"LootTableSeed":0,"Name":null,"SellItems":[],"SellModifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"50","VariableIndex":0,"Metadata":null},"UseMoney":1,"UseVariable":0,"VariableIndex":0,"Metadata":null},"StoreID":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.AccessShopCommand"}`

#### **Open a Shop and Store Its Unique Identifier**[¶](#open-a-shop-and-store-its-unique-identifier "Permanent link")

This opens a shop and stores its unique ID in Global Variable 0 for later reference by other shop commands.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = access_shop("00000000-0000-0000-0000-000000000001") { [](#__codelineno-2-2)    buy_modifier: 100 [](#__codelineno-2-3)    sell_modifier: 50 [](#__codelineno-2-4)    is_buy_allowed: true [](#__codelineno-2-5)    is_sell_allowed: false [](#__codelineno-2-6)};`

`[](#__codelineno-3-1){"Data":{"Index":0,"IsLocal":0,"IsTimeConstrained":1,"ShopID":"00000000-0000-0000-0000-000000000001","Shop":{"BuyModifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"Categories":[],"IsBuyAllowed":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IsLocal":0,"IsSellAllowed":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"LootTableSeed":0,"Name":null,"SellItems":[],"SellModifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"50","VariableIndex":0,"Metadata":null},"UseMoney":1,"UseVariable":0,"VariableIndex":0,"Metadata":null},"StoreID":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Shop.AccessShopCommand"}`