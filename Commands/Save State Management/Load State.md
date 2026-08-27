# Load State

*Источник: https://docs.rpg-architect.com/07-commands/02-save-state-management/01-load-state/*

---

# Load State

## **Load State**[¶](#load-state "Permanent link")

Loads a previously saved game state from the specified index.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Result

The switch to store whether the load operation succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

State Index

The index of the saved state to load.

[Variable or Value](../../../05-reference/variable-or-value/)

Store Results

When enabled, the result of the load operation is stored in a switch.

Toggle

Use Transition

When enabled, the scene transition effect plays when loading the state. When disabled, the state loads immediately without a transition.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Load the Game State from Slot 1**[¶](#load-the-game-state-from-slot-1 "Permanent link")

This loads the previously saved game state from slot index 1, playing the scene transition effect.

Code ScriptVisual Script

`[](#__codelineno-0-1)load_state(1);`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"StoreResults":0,"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.LoadStateCommand"}`

#### **Load the Game State without a Transition**[¶](#load-the-game-state-without-a-transition "Permanent link")

This loads the game state from slot 2 immediately, skipping the scene transition effect.

Code ScriptVisual Script

`[](#__codelineno-2-1)load_state(2, no_transition);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"StoreResults":0,"UseTransition":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.LoadStateCommand"}`

#### **Load a Game State from a Variable and Store the Result**[¶](#load-a-game-state-from-a-variable-and-store-the-result "Permanent link")

This loads the game state from the slot specified by Global Variable 0, storing whether the load succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gs[0] = load_state($gv[0]);`

`[](#__codelineno-5-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"StateIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreResults":1,"UseTransition":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.StateData.LoadStateCommand"}`