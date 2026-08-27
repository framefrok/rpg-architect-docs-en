# Switch Conditional

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/01-switch-conditional/*

---

# Switch Conditional

## **Switch Conditional**[¶](#switch-conditional "Permanent link")

Evaluates multiple cases in order and executes the commands for the first case whose conditions are met.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Default Commands

The commands to execute when none of the switch cases match. Acts as the fallback or "else" branch.

[Script](../../../05-reference/script/)

Switch Items

The list of cases in the switch conditional. Each case has its own conditions and commands to execute when matched.

[Array](../../../05-reference/array/)

## **Examples**[¶](#examples "Permanent link")

#### **Switch with Two Cases and a Default**[¶](#switch-with-two-cases-and-a-default "Permanent link")

This evaluates multiple cases in order. If Global Variable 0 equals 1, the first case executes. If it equals 2, the second case executes. Otherwise, the default block runs.

Code ScriptVisual Script

`[](#__codelineno-0-1)switch [](#__codelineno-0-2){ [](#__codelineno-0-3)    case ($gv[0] == 1) [](#__codelineno-0-4)    { [](#__codelineno-0-5)        wait(100); [](#__codelineno-0-6)    } [](#__codelineno-0-7)    case ($gv[0] == 2) [](#__codelineno-0-8)    { [](#__codelineno-0-9)        wait(200); [](#__codelineno-0-10)    } [](#__codelineno-0-11)    default [](#__codelineno-0-12)    { [](#__codelineno-0-13)        wait(500); [](#__codelineno-0-14)    } [](#__codelineno-0-15)}`

`[](#__codelineno-1-1){"Data":{"DefaultCommands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsTimeConstrained":1,"SwitchItems":[{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Conditions":[{"$":"GlobalVariableCondition","ComparisonGlobalVariableIndex":null,"ComparisonLocalVariableIndex":null,"Index":0,"Operand":0,"Value":"1","Metadata":null}],"IsDefaultSet":0,"Name":"","Metadata":null},{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"200","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Conditions":[{"$":"GlobalVariableCondition","ComparisonGlobalVariableIndex":null,"ComparisonLocalVariableIndex":null,"Index":0,"Operand":0,"Value":"2","Metadata":null}],"IsDefaultSet":0,"Name":"","Metadata":null}],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.SwitchConditionalCommand"}`

#### **Switch with Named Cases**[¶](#switch-with-named-cases "Permanent link")

This uses named cases for editor readability. The name is a label that appears in the editor for organizational purposes.

Code ScriptVisual Script

`[](#__codelineno-2-1)switch [](#__codelineno-2-2){ [](#__codelineno-2-3)    case "Player is high level" ($gv[0] > 50) [](#__codelineno-2-4)    { [](#__codelineno-2-5)        wait(100); [](#__codelineno-2-6)    } [](#__codelineno-2-7)    default [](#__codelineno-2-8)    { [](#__codelineno-2-9)        wait(500); [](#__codelineno-2-10)    } [](#__codelineno-2-11)}`

`[](#__codelineno-3-1){"Data":{"DefaultCommands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"IsTimeConstrained":1,"SwitchItems":[{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Conditions":[{"$":"GlobalVariableCondition","ComparisonGlobalVariableIndex":null,"ComparisonLocalVariableIndex":null,"Index":0,"Operand":4,"Value":"50","Metadata":null}],"IsDefaultSet":0,"Name":"Player is high level","Metadata":null}],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.SwitchConditionalCommand"}`