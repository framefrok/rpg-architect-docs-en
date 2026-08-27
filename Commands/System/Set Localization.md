# Set Localization

*Источник: https://docs.rpg-architect.com/07-commands/20-system/60-set-localization/*

---

# Set Localization

## **Set Localization**[¶](#set-localization "Permanent link")

Changes the active localization used by the engine.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Localization

The index of the localization to use, corresponding to a localization defined in the database.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Localization to First Language**[¶](#set-localization-to-first-language "Permanent link")

Changes the active localization to the first language defined in the database.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_localization("0");`

`[](#__codelineno-1-1){"Data":{"Localization":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.SetLocalizationCommand"}`

#### **Set Localization from a Variable**[¶](#set-localization-from-a-variable "Permanent link")

Changes the active localization using the index stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_localization($gv[0]);`

`[](#__codelineno-3-1){"Data":{"Localization":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.SetLocalizationCommand"}`