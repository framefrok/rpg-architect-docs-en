# Run Global Script

*Источник: https://docs.rpg-architect.com/07-commands/20-system/00-run-global-script/*

---

# Run Global Script

## **Run Global Script**[¶](#run-global-script "Permanent link")

Executes a global script defined in the database, running inline and blocking until complete.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Global Script

The global script to execute from the database.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Run Global Script by Index**[¶](#run-global-script-by-index "Permanent link")

Executes global script 0 from the database, running it inline and blocking until complete.

Code ScriptVisual Script

`[](#__codelineno-0-1)run_global_script(0);`

`[](#__codelineno-1-1){"Data":{"ScriptIndex":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.GlobalScriptCommand"}`

#### **Run a Different Global Script**[¶](#run-a-different-global-script "Permanent link")

Executes global script 5 from the database.

Code ScriptVisual Script

`[](#__codelineno-2-1)run_global_script(5);`

`[](#__codelineno-3-1){"Data":{"ScriptIndex":5,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.GlobalScriptCommand"}`