# Conditional Loop

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/11-conditional-loop/*

---

# Conditional Loop

## **Conditional Loop**[¶](#conditional-loop "Permanent link")

Repeats commands as long as all specified conditions continue to be met.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Commands

The commands to execute on each iteration of the loop while the conditions remain met.

[Script](../../../05-reference/script/)

Conditions

The conditions that must all be met for the loop to continue iterating. The conditions are re-evaluated at the start of each iteration.

[Condition](../../../05-reference/condition/)

## **Examples**[¶](#examples "Permanent link")

#### **Loop While Global Switch 0 is On**[¶](#loop-while-global-switch-0-is-on "Permanent link")

This repeats the contained commands as long as Global Switch 0 remains on.

Code ScriptVisual Script

`[](#__codelineno-0-1)while ($gs[0] == true) [](#__codelineno-0-2){ [](#__codelineno-0-3)    wait(100); [](#__codelineno-0-4)}`

`[](#__codelineno-1-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Conditions":[{"$":"GlobalSwitchCondition","ComparisonGlobalSwitchIndex":null,"ComparisonLocalSwitchIndex":null,"Index":0,"Value":1,"Metadata":null}],"IsTimeConstrained":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.WhileLoopCommand"}`

#### **Loop While Global Variable 0 is Less Than 100**[¶](#loop-while-global-variable-0-is-less-than-100 "Permanent link")

This repeats the contained commands as long as Global Variable 0 is less than 100.

Code ScriptVisual Script

`[](#__codelineno-2-1)while ($gv[0] < 100) [](#__codelineno-2-2){ [](#__codelineno-2-3)    $gv[0] += 1; [](#__codelineno-2-4)}`

`[](#__codelineno-3-1){"Data":{"Commands":[{"$":"VariableCommand","Operation":1,"RandomEnd":null,"RandomStart":null,"Value":"1","Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null}],"Conditions":[{"$":"GlobalVariableCondition","ComparisonGlobalVariableIndex":null,"ComparisonLocalVariableIndex":null,"Index":0,"Operand":2,"Value":"100","Metadata":null}],"IsTimeConstrained":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.WhileLoopCommand"}`