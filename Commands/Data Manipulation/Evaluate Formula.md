# Evaluate Formula

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/11-evaluate-formula/*

---

# Evaluate Formula

## **Evaluate Formula**[¶](#evaluate-formula "Permanent link")

Evaluates a mathematical expression and stores the result in a [Variable](../../../05-reference/variable/).

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Floating Point

When enabled, the formula result will be stored as a floating point (decimal) number instead of an integer.

Toggle

Formula

The mathematical expression to evaluate.

[Formula](../../../05-reference/formulas/)

Integer

When enabled, the formula result will be truncated to a whole number (integer).

Toggle

Target

The variable where the evaluated formula result will be stored.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Add Two Variables and Store the Result in Global Variable 0**[¶](#add-two-variables-and-store-the-result-in-global-variable-0 "Permanent link")

This evaluates the sum of Global Variable 1 and Global Variable 2, storing the integer result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = eval($gv[1] + $gv[2]);`

`[](#__codelineno-1-1){"Data":{"Formula":"global(1) \u002B global(2)","IsFloatingPoint":0,"IsInteger":1,"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.EvaluateFormulaCommand"}`

#### **Evaluate the Maximum of a Variable and a Fixed Value**[¶](#evaluate-the-maximum-of-a-variable-and-a-fixed-value "Permanent link")

This evaluates the maximum of Global Variable 1 and 10, storing the integer result in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = eval(max($gv[1], 10));`

`[](#__codelineno-3-1){"Data":{"Formula":"max(global(1), 10)","IsFloatingPoint":0,"IsInteger":1,"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.EvaluateFormulaCommand"}`

#### **Evaluate a Formula with Floating Point Result**[¶](#evaluate-a-formula-with-floating-point-result "Permanent link")

This evaluates the expression using Global Variable 1, storing the result as a floating point number in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = eval($gv[1] * 2 + 1, floating_point);`

`[](#__codelineno-5-1){"Data":{"Formula":"global(1) * 2 \u002B 1","IsFloatingPoint":1,"IsInteger":0,"Target":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.EvaluateFormulaCommand"}`