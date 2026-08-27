# Remove Character

*Источник: https://docs.rpg-architect.com/07-commands/08-party/01-remove-character/*

---

# Remove Character

## **Remove Character**[¶](#remove-character "Permanent link")

Deletes a character from the party entirely, removing them from both the active and inactive party lists.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Target

The party member to remove from the party.

[Actor Reference](../../../05-reference/actor-reference/)

Update Scene

Whether the scene is immediately updated after removing the character. When enabled, the party display on the map updates right away.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Remove Party Member 0 from the Party**[¶](#remove-party-member-0-from-the-party "Permanent link")

This removes the first active party member from the party entirely.

Code ScriptVisual Script

`[](#__codelineno-0-1)remove_character(party(0));`

`[](#__codelineno-1-1){"Data":{"IsReflectedImmediately":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.RemoveCharacterCommand"}`

#### **Remove a Character by Unique Identifier with Immediate Scene Update**[¶](#remove-a-character-by-unique-identifier-with-immediate-scene-update "Permanent link")

This removes the party member identified by the unique identifier stored in Global Variable 0 and immediately updates the scene.

Code ScriptVisual Script

`[](#__codelineno-2-1)remove_character(uid($gv[0]), immediate);`

`[](#__codelineno-3-1){"Data":{"IsReflectedImmediately":1,"Target":{"Identifier":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":1,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.RemoveCharacterCommand"}`