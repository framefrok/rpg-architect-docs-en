# Restore Character

*Источник: https://docs.rpg-architect.com/07-commands/06-character/02-restore-character/*

---

# Restore Character

## **Restore Character**[¶](#restore-character "Permanent link")

Resets a character's statistics to their maximum values and removes all status effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Clear Status Effects

When enabled, all status effects are removed from the character.

[Switch or Value](../../../05-reference/switch-or-value/)

Restore Statistics

When enabled, all statistics are restored to their maximum values.

[Switch or Value](../../../05-reference/switch-or-value/)

Target

The character to apply the operation to.

[Character](../../../06-database/00-characters/00-characters/)

## **Examples**[¶](#examples "Permanent link")

#### **Fully Restore Party Member 0**[¶](#fully-restore-party-member-0 "Permanent link")

This restores the first active party member's statistics to maximum and removes all status effects.

Code ScriptVisual Script

`[](#__codelineno-0-1)restore_character(party(0), true, true);`

`[](#__codelineno-1-1){"Data":{"IncludeStatistics":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.RestoreCharacterCommand"}`

#### **Restore Only Statistics for Hero 0**[¶](#restore-only-statistics-for-hero-0 "Permanent link")

This restores the statistics of database hero 0 to their maximum values without removing status effects.

Code ScriptVisual Script

`[](#__codelineno-2-1)restore_character(hero(0), true, false);`

`[](#__codelineno-3-1){"Data":{"IncludeStatistics":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.RestoreCharacterCommand"}`

#### **Remove Only Status Effects from Party Member 0**[¶](#remove-only-status-effects-from-party-member-0 "Permanent link")

This removes all status effects from the first active party member without restoring statistics.

Code ScriptVisual Script

`[](#__codelineno-4-1)restore_character(party(0), false, true);`

`[](#__codelineno-5-1){"Data":{"IncludeStatistics":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.RestoreCharacterCommand"}`