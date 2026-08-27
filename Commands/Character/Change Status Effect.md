# Change Status Effect

*Источник: https://docs.rpg-architect.com/07-commands/06-character/01-change-status-effect/*

---

# Change Status Effect

## **Change Status Effect**[¶](#change-status-effect "Permanent link")

Adds or removes a status effect from a character.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add

When enabled, the status effect is applied to the character. When disabled, the status effect is removed.

Toggle

Force

When enabled with Remove, permanently suppresses the status effect on the target. When enabled with Add, permanently asserts it. Bypasses persistence either way — works even when a Class, Character, or Equipment trait table would otherwise dictate the result.

Toggle

Remove

When enabled, the status effect is removed from the character.

Toggle

Status Effect

The status effect to add or remove.

[Status Effect](../../../06-database/05-statistics/03-status-effects/)

Target

The character to apply the operation to.

[Character](../../../06-database/00-characters/00-characters/)

## **Examples**[¶](#examples "Permanent link")

#### **Apply a Status Effect to Party Member 0**[¶](#apply-a-status-effect-to-party-member-0 "Permanent link")

This applies the status effect at database index stored in Global Variable 0 to the first active party member.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_status(party(0), $gv[0]);`

`[](#__codelineno-1-1){"Data":{"IsAdd":1,"IsForceful":0,"IsRemove":0,"StatusEffect":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeStatusCommand"}`

#### **Remove a Status Effect from a Character**[¶](#remove-a-status-effect-from-a-character "Permanent link")

This removes the status effect at database index 2 from the first active party member.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_status(party(0), 2, remove);`

`[](#__codelineno-3-1){"Data":{"IsAdd":0,"IsForceful":0,"IsRemove":1,"StatusEffect":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeStatusCommand"}`