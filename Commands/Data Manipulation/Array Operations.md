# Array Operations

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/02-array-operations/*

---

# Array Operations

## **Array Operations**[¶](#array-operations "Permanent link")

Alters an [Array](../../../05-reference/array/) present in a [Variable](../../../05-reference/variable/), allowing you to access indices or resize it.

## **Index**[¶](#index "Permanent link")

Name

Explanation

Value

Leverages a value, as a Number.

Local Variable

Leverages a single [Local Variable](../../../05-reference/variable/).

Global Variable

Leverages a single [Global Variable](../../../05-reference/variable/).

## **Count**[¶](#count "Permanent link")

Name

Explanation

Value

Leverages a value, as a Number.

Local Variable

Leverages a single [Local Variable](../../../05-reference/variable/).

Global Variable

Leverages a single [Global Variable](../../../05-reference/variable/).

> **Note**: When increasing the size of the Array, new Indices will be filled with a blank value, similar to unused Variables.

## **Examples**[¶](#examples "Permanent link")

#### **Get Array Value at Index 0 from Global Variable 0, Save to Global Variable 77**[¶](#get-array-value-at-index-0-from-global-variable-0-save-to-global-variable-77 "Permanent link")

This retrieves the value at index 0 from the array stored in Global Variable 0 and saves it into Global Variable 77.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[77] = array($gv[0])[0];`

`[](#__codelineno-1-1){"Data":{"ArrayIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ArrayReference":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsCount":0,"IsGet":1,"IsIndexer":1,"IsSet":0,"Operand":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":77,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ArrayCommand"}`

#### **Set Array Value at Variable Index in Global Variable 0 to 45**[¶](#set-array-value-at-variable-index-in-global-variable-0-to-45 "Permanent link")

This sets the value at the index specified by Global Variable 2, inside the array stored in Global Variable 0, to 45.

Code ScriptVisual Script

`[](#__codelineno-2-1)array($gv[0])[$gv[2]] = 45;`

`[](#__codelineno-3-1){"Data":{"ArrayIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"ArrayReference":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsCount":0,"IsGet":0,"IsIndexer":1,"IsSet":1,"Operand":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"45","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ArrayCommand"}`

#### **Resize Array in Global Variable 1 to 20 Elements**[¶](#resize-array-in-global-variable-1-to-20-elements "Permanent link")

This resizes the array stored in Global Variable 1 to 20 elements. New elements are filled with blank values.

Code ScriptVisual Script

`[](#__codelineno-4-1)array_resize($gv[1], 20);`

`[](#__codelineno-5-1){"Data":{"ArrayIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ArrayReference":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"IsCount":1,"IsGet":0,"IsIndexer":0,"IsSet":1,"Operand":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"20","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ArrayCommand"}`

#### **Get Array Count from Global Variable 1, Save to Global Variable 2**[¶](#get-array-count-from-global-variable-1-save-to-global-variable-2 "Permanent link")

This retrieves the number of elements in the array stored in Global Variable 1 and saves it into Global Variable 2.

Code ScriptVisual Script

`[](#__codelineno-6-1)$gv[2] = array_count($gv[1]);`

`[](#__codelineno-7-1){"Data":{"ArrayIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"ArrayReference":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"IsCount":1,"IsGet":1,"IsIndexer":0,"IsSet":0,"Operand":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ArrayCommand"}`