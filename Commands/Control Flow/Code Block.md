# Code Block

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/99-code-block/*

---

# Code Block

## **Code Block**[¶](#code-block "Permanent link")

Groups commands into a single block that can be commented out to disable all contained commands.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Commands

The commands to execute when the block is not commented out.

[Script](../../../05-reference/script/)

Comment

The comment text displayed when the block is commented out.

String

Ignore

Whether the block is commented out. When enabled, the commands inside the block are skipped during execution.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Group Commands in a Block**[¶](#group-commands-in-a-block "Permanent link")

This groups commands into a single block that executes normally.

Code ScriptVisual Script

`[](#__codelineno-0-1)block [](#__codelineno-0-2){ [](#__codelineno-0-3)    wait(100); [](#__codelineno-0-4)}`

`[](#__codelineno-1-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Comment":null,"IsCommented":0,"IsTimeConstrained":1,"Name":"Code Block","SortOrder":99,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.CodeBlockCommand"}`

#### **Disable a Block of Commands with a Label**[¶](#disable-a-block-of-commands-with-a-label "Permanent link")

This disables (comments out) a block of commands so they are skipped during execution. The label provides context for why the block is disabled.

Code ScriptVisual Script

`[](#__codelineno-2-1)disabled "Disabled for testing" [](#__codelineno-2-2){ [](#__codelineno-2-3)    wait(100); [](#__codelineno-2-4)}`

`[](#__codelineno-3-1){"Data":{"Commands":[{"$":"WaitCommand","Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null}],"Comment":"Disabled for testing","IsCommented":1,"IsTimeConstrained":1,"Name":"Code Block","SortOrder":99,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.CodeBlockCommand"}`