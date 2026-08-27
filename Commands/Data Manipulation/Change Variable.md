# Change Variable

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/01-change-variable/*

---

# Change Variable

## **Change Variable**[¶](#change-variable "Permanent link")

Alters the value of a [Variable](../../../05-reference/variable/), with support for ranges and [Local or Global](../../../05-reference/local-and-global-data/) variables.

## **Targets**[¶](#targets "Permanent link")

Name

Explanation

Global / Local

Targets a single [Variable](../../../05-reference/variable/).

Global / Local Range

Targets multiple contiguous [Variables](../../../05-reference/variable/).

Global / Local Reference

Targets a single [Variable](../../../05-reference/variable/) based on a [Variable](../../../05-reference/variable/) index.

## **Values**[¶](#values "Permanent link")

Name

Explanation

Value

Leverages a value, as a Number or String.

Local

Leverages a single [Local Variable](../../../05-reference/variable/).

Global

Leverages a single [Global Variables](../../../05-reference/variable/).

Random

Leverages a random Number value, between a **Minimum** and **Maximum**.

## **Examples**[¶](#examples "Permanent link")

#### **Set Global Variable 3 to a Random Value Between 6 and 12**[¶](#set-global-variable-3-to-a-random-value-between-6-and-12 "Permanent link")

This sets Global Variable 3 to a random value between 6 and 12.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[3] = random(6, 12);`

`[](#__codelineno-1-1){"Data":{"Operation":0,"RandomEnd":"12","RandomStart":"6","Value":"0","Index":3,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableCommand"}`

#### **Add 20 to Local Variables 0 through 6**[¶](#add-20-to-local-variables-0-through-6 "Permanent link")

This adds 20 to Local Variables 0 through 6.

Code ScriptVisual Script

`[](#__codelineno-2-1)$lv[0:6] += 20;`

`[](#__codelineno-3-1){"Data":{"Operation":1,"RandomEnd":null,"RandomStart":null,"Value":"20","Index":0,"IndexEnd":6,"IsGlobal":0,"IsLocal":1,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableCommand"}`

#### **Subtract 1 from Global Variable by Reference, Based on Global Variable 0**[¶](#subtract-1-from-global-variable-by-reference-based-on-global-variable-0 "Permanent link")

This subtracts 1 from a Global Variable, with an index specified by Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$ref_gv[0] -= 1;`

`[](#__codelineno-5-1){"Data":{"Operation":2,"RandomEnd":null,"RandomStart":null,"Value":"1","Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":1,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableCommand"}`

#### **Multiply Global Variable by Reference, Based on Global Variable 0, by 5**[¶](#multiply-global-variable-by-reference-based-on-global-variable-0-by-5 "Permanent link")

This multiplies the value of a Global Variable, with an index specified by Global Variable 0, by 5.

Code ScriptVisual Script

`[](#__codelineno-6-1)$ref_gv[0] *= 5;`

`[](#__codelineno-7-1){"Data":{"Operation":3,"RandomEnd":null,"RandomStart":null,"Value":"5","Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":1,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableCommand"}`

#### **Set Local Variable 0 to the Value of Global Variable 5**[¶](#set-local-variable-0-to-the-value-of-global-variable-5 "Permanent link")

This sets Local Variable 0 to the value in Global Variable 5.

Code ScriptVisual Script

`[](#__codelineno-8-1)$lv[0] = $gv[5];`

`[](#__codelineno-9-1){"Data":{"Operation":0,"RandomEnd":null,"RandomStart":null,"Value":"0","Index":0,"IndexEnd":null,"IsGlobal":0,"IsLocal":1,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":5,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableCommand"}`