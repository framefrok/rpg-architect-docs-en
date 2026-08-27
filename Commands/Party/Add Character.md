# Add Character

*Источник: https://docs.rpg-architect.com/07-commands/08-party/00-add-character/*

---

# Add Character

## **Add Character**[¶](#add-character "Permanent link")

Creates a new character and adds them to the active or inactive party.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add to Active Party

Whether to add the character to the active party. When disabled, the character is added to the inactive (reserve) party instead.

[Switch or Value](../../../05-reference/switch-or-value/)

Add to Scene

Whether the character is immediately added to the current scene. When enabled, the party display on the map updates right away.

Toggle

Character

The database character to add to the party.

[Variable or Value](../../../05-reference/variable-or-value/)

Global

Whether to store the unique ID in a global variable.

Toggle

Local

Whether to store the unique ID in a local variable.

Toggle

Store ID

Whether to store the new character's unique ID in a variable. This allows the character to be referenced later by their unique ID.

Toggle

Variable Index

The variable index to store the character's unique ID in.

Number

## **Examples**[¶](#examples "Permanent link")

#### **Add a Character to the Active Party**[¶](#add-a-character-to-the-active-party "Permanent link")

This creates a new character from database index stored in Global Variable 0 and adds them to the active party.

Code ScriptVisual Script

`[](#__codelineno-0-1)add_character($gv[0]);`

`[](#__codelineno-1-1){"Data":{"AddToActiveParty":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Character":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IsGlobal":1,"IsLocal":0,"IsReflectedImmediately":0,"StoreID":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.AddCharacterCommand"}`

#### **Add a Character to the Inactive Party**[¶](#add-a-character-to-the-inactive-party "Permanent link")

This creates a new character and adds them to the inactive (reserve) party instead of the active party.

Code ScriptVisual Script

`[](#__codelineno-2-1)add_character($gv[0], active: false);`

`[](#__codelineno-3-1){"Data":{"AddToActiveParty":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Character":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IsGlobal":1,"IsLocal":0,"IsReflectedImmediately":0,"StoreID":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.AddCharacterCommand"}`

#### **Add a Character and Store the Unique Identifier**[¶](#add-a-character-and-store-the-unique-identifier "Permanent link")

This creates a new character, adds them to the active party with immediate scene reflection, and stores their unique identifier in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = add_character(1, immediate);`

`[](#__codelineno-5-1){"Data":{"AddToActiveParty":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Character":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Index":0,"IsGlobal":1,"IsLocal":0,"IsReflectedImmediately":1,"StoreID":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.AddCharacterCommand"}`