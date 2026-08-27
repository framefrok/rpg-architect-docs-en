# Fixed Loop

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/10-fixed-loop/*

---

# Fixed Loop

## **Fixed Loop**[¶](#fixed-loop "Permanent link")

Repeats a set of commands a fixed number of times, iterating from a start value to an end value with a configurable step increment.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Commands

The commands to execute on each iteration of the loop.

[Script](../../../05-reference/script/)

End

The ending value of the loop. The loop iterates until this value is reached.

[Variable or Value](../../../05-reference/variable-or-value/)

Increment

The step value added to the iterator on each loop iteration. Use a negative value to count downward.

[Variable or Value](../../../05-reference/variable-or-value/)

Is Inclusive

Whether the loop includes the end value. When enabled, the loop iterates up to and including the end value. When disabled, the loop stops one step before the end value.

Toggle

Iterator

The variable that stores the current loop index on each iteration. Only used when **Use Iterator** is enabled.

[Variable or Value](../../../05-reference/variable-or-value/)

Start

The starting value of the loop. The loop begins iterating from this value.

[Variable or Value](../../../05-reference/variable-or-value/)

Use Iterator

Whether to store the current loop index in a variable on each iteration. When enabled, the **Iterator** variable is updated with the current loop value.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Loop from 0 to 5 Inclusive**[¶](#loop-from-0-to-5-inclusive "Permanent link")

This repeats the contained commands 6 times, iterating from 0 to 5 inclusive without an iterator variable.

Code ScriptVisual Script

`[](#__codelineno-0-1)for(; 0..5) [](#__codelineno-0-2){ [](#__codelineno-0-3)    wait(100); [](#__codelineno-0-4)}`

`[](#__codelineno-1-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsInclusive":1,"IsTimeConstrained":1,"End":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Increment":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Iterator":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Start":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"UseIterator":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.ForLoopCommand"}`

#### **Loop from 0 to 10 Exclusive with Iterator and Step of 2**[¶](#loop-from-0-to-10-exclusive-with-iterator-and-step-of-2 "Permanent link")

This iterates from 0 to 10 exclusive, stepping by 2, and stores the current loop index in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)for($gv[0]; 0..10 exclusive; step 2) [](#__codelineno-2-2){ [](#__codelineno-2-3)    wait(100); [](#__codelineno-2-4)}`

`[](#__codelineno-3-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsInclusive":0,"IsTimeConstrained":1,"End":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Increment":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Iterator":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Start":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"UseIterator":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.ForLoopCommand"}`

#### **Loop with Local Variable Iterator**[¶](#loop-with-local-variable-iterator "Permanent link")

This iterates from 1 to 3 inclusive, storing the current loop index in Local Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)for($lv[0]; 1..3) [](#__codelineno-4-2){ [](#__codelineno-4-3)    wait(500); [](#__codelineno-4-4)}`

`[](#__codelineno-5-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsInclusive":1,"IsTimeConstrained":1,"End":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"Increment":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Iterator":{"IsGlobalVariable":false,"IsLocalVariable":true,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Start":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"UseIterator":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.ForLoopCommand"}`