# Wait

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/03-wait/*

---

# Wait

## **Wait**[¶](#wait "Permanent link")

Pauses execution of the current script for a specified duration in milliseconds.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Block Input

Whether to block player input during the wait period. When enabled, the player cannot interact until the wait completes.

Toggle

Duration (milliseconds)

The duration to wait in milliseconds before continuing script execution.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Wait for One Second**[¶](#wait-for-one-second "Permanent link")

This pauses script execution for 1000 milliseconds (one second).

Code ScriptVisual Script

`[](#__codelineno-0-1)wait(1000);`

`[](#__codelineno-1-1){"Data":{"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1000","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.WaitCommand"}`

#### **Wait for Half a Second and Block Player Input**[¶](#wait-for-half-a-second-and-block-player-input "Permanent link")

This pauses script execution for 500 milliseconds while preventing the player from providing any input.

Code ScriptVisual Script

`[](#__codelineno-2-1)wait(500, block_input);`

`[](#__codelineno-3-1){"Data":{"Duration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"IsBlockingInput":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.WaitCommand"}`

#### **Wait for a Duration Stored in a Global Variable**[¶](#wait-for-a-duration-stored-in-a-global-variable "Permanent link")

This pauses script execution for the number of milliseconds stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)wait($gv[0]);`

`[](#__codelineno-5-1){"Data":{"Duration":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsBlockingInput":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.WaitCommand"}`