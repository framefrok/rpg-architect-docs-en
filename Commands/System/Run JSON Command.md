# Run JSON Command

*Источник: https://docs.rpg-architect.com/07-commands/20-system/200-run-json-command/*

---

# Run JSON Command

## **Run JSON Command**[¶](#run-json-command "Permanent link")

Deserializes a JSON string into a command and executes it at runtime for dynamic command construction.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

JSON Command

The JSON string to deserialize into a command and executes at runtime.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Run a JSON Command from a String Literal**[¶](#run-a-json-command-from-a-string-literal "Permanent link")

Deserializes and executes a command from a JSON string at runtime.

Code ScriptVisual Script

`[](#__codelineno-0-1)run_json("{}");`

`[](#__codelineno-1-1){"Data":{"JsonCommand":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"{}","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.RunJsonCommand"}`

#### **Run a JSON Command from a Variable**[¶](#run-a-json-command-from-a-variable "Permanent link")

Deserializes and executes a command stored as a JSON string in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)run_json($gv[0]);`

`[](#__codelineno-3-1){"Data":{"JsonCommand":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.RunJsonCommand"}`