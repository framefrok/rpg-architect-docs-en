# Conditional (If/Then/Else)

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/00-conditional-%28if-then-else%29/*

---

# Conditional (If/Then/Else)

## **Conditional (If/Then/Else)**[¶](#conditional-ifthenelse "Permanent link")

Evaluates a set of conditions and executes the "Then" commands if all conditions are met, or the "Else" commands if any condition fails.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Conditions

The conditions that must all be met for the "Then" commands to execute. If any condition fails, the "Else" commands are executed instead.

[Condition](../../../05-reference/condition/)

Else

The commands to execute when the conditions are not met.

[Script](../../../05-reference/script/)

Then

The commands to execute when all conditions are met.

[Script](../../../05-reference/script/)

## **Examples**[¶](#examples "Permanent link")

#### **Execute Commands When Global Switch 0 is On**[¶](#execute-commands-when-global-switch-0-is-on "Permanent link")

This checks if Global Switch 0 is on and executes the then-block commands if it is.

Code ScriptVisual Script

`[](#__codelineno-0-1)if ($gs[0] == true) [](#__codelineno-0-2){ [](#__codelineno-0-3)    wait(1000); [](#__codelineno-0-4)}`

`[](#__codelineno-1-1){"Data":{"Conditions":[{"$":"GlobalSwitchCondition","ComparisonGlobalSwitchIndex":null,"ComparisonLocalSwitchIndex":null,"Index":0,"Value":1,"Metadata":null}],"FailureCommands":[],"IsTimeConstrained":1,"SuccessCommands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.ConditionalCommand"}`

#### **Conditional with Both Then and Else Branches**[¶](#conditional-with-both-then-and-else-branches "Permanent link")

This checks if Global Variable 0 is greater than 10. If true, it waits for 500 milliseconds. Otherwise, it waits for 2000 milliseconds.

Code ScriptVisual Script

`[](#__codelineno-2-1)if ($gv[0] > 10) [](#__codelineno-2-2){ [](#__codelineno-2-3)    wait(500); [](#__codelineno-2-4)} [](#__codelineno-2-5)else [](#__codelineno-2-6){ [](#__codelineno-2-7)    wait(2000); [](#__codelineno-2-8)}`

`[](#__codelineno-3-1){"Data":{"Conditions":[{"$":"GlobalVariableCondition","ComparisonGlobalVariableIndex":null,"ComparisonLocalVariableIndex":null,"Index":0,"Operand":4,"Value":"10","Metadata":null}],"FailureCommands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2000","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsTimeConstrained":1,"SuccessCommands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.ConditionalCommand"}`