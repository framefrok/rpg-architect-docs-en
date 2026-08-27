# Delete State

*Источник: https://docs.rpg-architect.com/07-commands/02-save-state-management/03-delete-state/*

---

# Delete State

## **Delete State**[¶](#delete-state "Permanent link")

Deletes a previously saved game state at the specified index.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Result

The switch to store whether the delete operation succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

State Index

The index of the saved state to delete.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the delete operation is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Delete the Save State at Slot 1**[¶](#delete-the-save-state-at-slot-1 "Permanent link")

This deletes the saved game state at slot index 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)delete_state(1);`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"StoreResults":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.DeleteStateCommand"}`

#### **Delete a Save State and Store the Result**[¶](#delete-a-save-state-and-store-the-result "Permanent link")

This deletes the saved game state at the slot specified by Global Variable 0, storing whether the deletion succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gs[0] = delete_state($gv[0]);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.DeleteStateCommand"}`