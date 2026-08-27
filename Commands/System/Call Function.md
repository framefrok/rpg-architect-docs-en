# Call Function

*Источник: https://docs.rpg-architect.com/07-commands/20-system/01-call-function/*

---

# Call Function

## **Call Function**[¶](#call-function "Permanent link")

Executes a reusable function defined in the database, passing input and output switches and variables to exchange data.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Function

The function to call from the database.

Number

Input Switches

The switch values to pass as input parameters to the function.

[Switch or Value](../../../05-reference/switch-or-value/)

Input Variables

The variable values to pass as input parameters to the function.

[Variable or Value](../../../05-reference/variable-or-value/)

Output Switches

The switch references that receive output values from the function after it executes.

[Switch or Value](../../../05-reference/switch-or-value/)

Output Variables

The variable references that receive output values from the function after it executes.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Call a Function by Index**[¶](#call-a-function-by-index "Permanent link")

Calls function 0 from the database with no input or output parameters.

Code ScriptVisual Script

`[](#__codelineno-0-1)call_function(0);`

`[](#__codelineno-1-1){"Data":{"FunctionIndex":0,"InputSwitches":[],"InputVariables":[],"OutputSwitches":[],"OutputVariables":[],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.CallFunctionCommand"}`

#### **Call a Function with Input and Output Variables**[¶](#call-a-function-with-input-and-output-variables "Permanent link")

Calls function 1, passing two global variables as input and receiving one global variable as output.

Code ScriptVisual Script

`[](#__codelineno-2-1)call_function(1, iv: [$gv[0], $gv[1]], ov: [$gv[2]]);`

`[](#__codelineno-3-1){"Data":{"FunctionIndex":1,"InputSwitches":[],"InputVariables":[{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null}],"OutputSwitches":[],"OutputVariables":[{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null}],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.CallFunctionCommand"}`

#### **Call a Function with Input Switches**[¶](#call-a-function-with-input-switches "Permanent link")

Calls function 2, passing a global switch as input.

Code ScriptVisual Script

`[](#__codelineno-4-1)call_function(2, is: [$gs[0]]);`

`[](#__codelineno-5-1){"Data":{"FunctionIndex":2,"InputSwitches":[{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null}],"InputVariables":[],"OutputSwitches":[],"OutputVariables":[],"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.CallFunctionCommand"}`