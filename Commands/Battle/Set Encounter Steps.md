# Set Encounter Steps

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/300-set-encounter-steps/*

---

# Set Encounter Steps

## **Set Encounter Steps**[¶](#set-encounter-steps "Permanent link")

Changes the number of steps until the next random encounter.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Steps

The number of steps to set the encounter counter to.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Encounter Steps to a Fixed Value**[¶](#set-encounter-steps-to-a-fixed-value "Permanent link")

This sets the number of steps until the next random encounter to 100.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_encounter_steps(100);`

`[](#__codelineno-1-1){"Data":{"Steps":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"100","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.SetEncounterStepsCommand"}`

#### **Set Encounter Steps Using a Global Variable**[¶](#set-encounter-steps-using-a-global-variable "Permanent link")

This sets the number of steps until the next random encounter to the value stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_encounter_steps($gv[0]);`

`[](#__codelineno-3-1){"Data":{"Steps":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.SetEncounterStepsCommand"}`