# Change Switch

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/00-change-switch/*

---

# Change Switch

## **Change Switch**[¶](#change-switch "Permanent link")

Alters the value of a [Switch](../../../05-reference/switch/), with support for ranges and [Local or Global](../../../05-reference/local-and-global-data/) switches.

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

#### **Set Global Switch 0 to Random**[¶](#set-global-switch-0-to-random "Permanent link")

This sets Global Switch 0 to a random value.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gs[0] = random();`

`[](#__codelineno-1-1){"Data":{"Random":1,"Value":0,"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SwitchCommand"}`

#### **Set Global Switches 0 through 99 to Off**[¶](#set-global-switches-0-through-99-to-off "Permanent link")

This sets Global Switches 0 through 99 to Off.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0:99] = false;`

`[](#__codelineno-3-1){"Data":{"Random":0,"Value":0,"Index":0,"IndexEnd":99,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SwitchCommand"}`

#### **Set Global Switch by Reference, Based on Global Variable 3**[¶](#set-global-switch-by-reference-based-on-global-variable-3 "Permanent link")

This sets a Global Switch, with an index specified by Global Variable 3, to On.

Code ScriptVisual Script

`[](#__codelineno-4-1)$ref_gs[3] = true;`

`[](#__codelineno-5-1){"Data":{"Random":0,"Value":1,"Index":3,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":1,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SwitchCommand"}`

#### **Set Local Switch 3 to Global Switch 0**[¶](#set-local-switch-3-to-global-switch-0 "Permanent link")

This sets Local Switch 3 to the value in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-6-1)$ls[3] = $gs[0];`

`[](#__codelineno-7-1){"Data":{"Random":0,"Value":0,"Index":3,"IndexEnd":null,"IsGlobal":0,"IsLocal":1,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":0,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SwitchCommand"}`