# Variable Manipulation

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/10-variable-manipulation/*

---

# Variable Manipulation

## **Variable Manipulation**[¶](#variable-manipulation "Permanent link")

Applies a transformation function to a [Variable](../../../05-reference/variable/), including math, string, and array operations.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Manipulator

The transformation function to apply to the target variable, such as abs, floor, round, uppercase, lowercase, or trim.

[Variable Manipulator](../../../05-reference/variable-manipulator/)

Target

The variable to apply the manipulation to.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Floor the Value in Global Variable 0**[¶](#floor-the-value-in-global-variable-0 "Permanent link")

This applies the floor function to the value stored in Global Variable 0, rounding it down to the nearest integer.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = manipulate(floor);`

`[](#__codelineno-1-1){"Data":{"Manipulator":{"$":"FloorVariableManipulator","Name":"Floor","IsTargetable":1,"Metadata":null},"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableManipulationCommand"}`

#### **Round the Value in Global Variable 0 to 2 Decimal Places**[¶](#round-the-value-in-global-variable-0-to-2-decimal-places "Permanent link")

This rounds the value stored in Global Variable 0 to 2 decimal places.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = manipulate(round, 2);`

`[](#__codelineno-3-1){"Data":{"Manipulator":{"$":"RoundVariableManipulator","Digits":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Name":"Round","IsTargetable":1,"Metadata":null},"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableManipulationCommand"}`

#### **Convert the String in Global Variable 0 to Uppercase**[¶](#convert-the-string-in-global-variable-0-to-uppercase "Permanent link")

This converts the string value stored in Global Variable 0 to uppercase.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = manipulate(uppercase);`

`[](#__codelineno-5-1){"Data":{"Manipulator":{"$":"UppercaseVariableManipulator","Name":"Uppercase","IsTargetable":1,"Metadata":null},"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.VariableManipulationCommand"}`