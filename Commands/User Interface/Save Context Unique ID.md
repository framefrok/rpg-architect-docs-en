# Save Context Unique ID

*Источник: https://docs.rpg-architect.com/07-commands/19-user-interface/100-save-context-unique-id/*

---

# Save Context Unique ID

## **Save Context Unique ID**[¶](#save-context-unique-id "Permanent link")

Saves the unique ID of the current context object to a variable for later reference.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Local

Whether to store the unique ID in a local variable.

Toggle

Variable Index

The index of the variable to store the unique ID in.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Save the Context Unique ID to Global Variable 0**[¶](#save-the-context-unique-id-to-global-variable-0 "Permanent link")

This saves the unique ID of the current context object to Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = save_context_unique_id();`

`[](#__codelineno-1-1){"Data":{"Context":null,"Index":0,"IsLocal":0,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SaveUniqueIDToVariableCommand"}`

#### **Save the Context Unique ID to Local Variable 3**[¶](#save-the-context-unique-id-to-local-variable-3 "Permanent link")

This saves the unique ID of the current context object to Local Variable 3.

Code ScriptVisual Script

`[](#__codelineno-2-1)$lv[3] = save_context_unique_id();`

`[](#__codelineno-3-1){"Data":{"Context":null,"Index":3,"IsLocal":1,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.UserInterface.SaveUniqueIDToVariableCommand"}`