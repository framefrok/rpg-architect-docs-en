# Change Money

*Источник: https://docs.rpg-architect.com/07-commands/05-inventory/100-change-money/*

---

# Change Money

## **Change Money**[¶](#change-money "Permanent link")

Adjusts the party's currency by the specified amount.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Amount

The amount of money to add or remove. Positive values increase the party's money and negative values decrease it.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Add 500 Money to the Party**[¶](#add-500-money-to-the-party "Permanent link")

This increases the party's money by 500.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_money(500);`

`[](#__codelineno-1-1){"Data":{"Money":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ChangeMoneyCommand"}`

#### **Adjust Money by Global Variable 1**[¶](#adjust-money-by-global-variable-1 "Permanent link")

Adjusts the party's money by the amount stored in Global Variable 1. Store a negative value to subtract.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_money($gv[1]);`

`[](#__codelineno-3-1){"Data":{"Money":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Inventory.ChangeMoneyCommand"}`