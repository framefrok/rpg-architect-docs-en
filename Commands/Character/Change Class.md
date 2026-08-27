# Change Class

*Источник: https://docs.rpg-architect.com/07-commands/06-character/03-change-class/*

---

# Change Class

## **Change Class**[¶](#change-class "Permanent link")

Adds, adjusts the rank of, or removes a class from a character.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Adjust Rank

When enabled, the operation adjusts the rank of the class. When disabled, the class is removed entirely.

Toggle

Class

The class to add, adjust, or remove.

[Class](../../../06-database/00-characters/01-classes/)

Rank

The rank value to set or adjust for the class.

[Variable or Value](../../../05-reference/variable-or-value/)

Remove

When enabled, the class is completely removed from the character.

Toggle

Target

The character to apply the operation to.

[Character](../../../06-database/00-characters/00-characters/)

Use As Delta Value

When enabled, the rank value is added to the current rank. When disabled, the rank is set to the specified value.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Add a Class to Party Member 0**[¶](#add-a-class-to-party-member-0 "Permanent link")

This adds the class at database index stored in Global Variable 0 to the first active party member with a default rank of 1.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_class(party(0), $gv[0]);`

`[](#__codelineno-1-1){"Data":{"Class":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsRankValue":1,"IsRemove":0,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeClassCommand"}`

#### **Set a Class Rank to a Specific Value**[¶](#set-a-class-rank-to-a-specific-value "Permanent link")

This sets the rank of the specified class on party member 0 to exactly 5, replacing the current rank.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_class(party(0), $gv[0], rank: 5, set);`

`[](#__codelineno-3-1){"Data":{"Class":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsDeltaOperation":0,"IsRankValue":1,"IsRemove":0,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeClassCommand"}`

#### **Remove a Class from a Character**[¶](#remove-a-class-from-a-character "Permanent link")

This completely removes the specified class from party member 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_class(party(0), $gv[0], remove);`

`[](#__codelineno-5-1){"Data":{"Class":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsRankValue":0,"IsRemove":1,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":1,"IsReferenceIndex":0,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Character.ChangeClassCommand"}`