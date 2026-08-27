# Save Unique ID

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/03-save-unique-id/*

---

# Save Unique ID

## **Save Unique ID**[¶](#save-unique-id "Permanent link")

Saves the [Unique ID](../../../05-reference/unique-id/) of the containing object to a [Variable](../../../05-reference/variable/).

> **Note**: This is often used in conjunction with [Save Value](../05-save-value/) to access data within the engine.

## **Examples**[¶](#examples "Permanent link")

#### **Save Unique ID to Global Variable 0**[¶](#save-unique-id-to-global-variable-0 "Permanent link")

This saves the Unique ID of the containing object to Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = save_unique_id();`

`[](#__codelineno-1-1){"Data":{"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SaveUniqueIDCommand"}`

#### **Save Unique ID to Local Variable 0**[¶](#save-unique-id-to-local-variable-0 "Permanent link")

This saves the Unique ID of the containing object to Local Variable 0, keeping the data scoped to the current event.

Code ScriptVisual Script

`[](#__codelineno-2-1)$lv[0] = save_unique_id();`

`[](#__codelineno-3-1){"Data":{"Index":0,"IndexEnd":null,"IsGlobal":0,"IsLocal":1,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.SaveUniqueIDCommand"}`