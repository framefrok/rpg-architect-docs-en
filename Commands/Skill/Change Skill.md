# Change Skill

*Источник: https://docs.rpg-architect.com/07-commands/07-skill/00-change-skill/*

---

# Change Skill

## **Change Skill**[¶](#change-skill "Permanent link")

Teaches or removes a skill from a hero.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add

When enabled, the skill will be taught to the hero. When disabled, the skill will be removed.

Toggle

Growth

The amount to adjust the growth of the skill.

[Variable or Value](../../../05-reference/variable-or-value/)

Hero

The hero to teach or remove the skill from.

[Character](../../../06-database/00-characters/00-characters/)

Rank

The rank to assign to the skill when teaching it.

[Variable or Value](../../../05-reference/variable-or-value/)

Skill

The skill to teach or remove.

[Skill](../../../06-database/01-skills/01-skills/)

## **Examples**[¶](#examples "Permanent link")

#### **Teach Skill 0 to Hero 0**[¶](#teach-skill-0-to-hero-0 "Permanent link")

This teaches skill 0 to hero 0 at the default rank of 1 with no additional growth.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_skill(hero(0), skill(0));`

`[](#__codelineno-1-1){"Data":{"Growth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IsAdd":1,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Skill":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.ChangeSkillCommand"}`

#### **Teach Skill 2 to Hero 1 at Rank 5 with Growth 10**[¶](#teach-skill-2-to-hero-1-at-rank-5-with-growth-10 "Permanent link")

This teaches skill 2 to hero 1 at rank 5 with 10 growth points applied.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_skill(hero(1), skill(2), rank: 5, growth: 10);`

`[](#__codelineno-3-1){"Data":{"Growth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IsAdd":1,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Skill":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.ChangeSkillCommand"}`

#### **Remove Skill 3 from Hero 0**[¶](#remove-skill-3-from-hero-0 "Permanent link")

This removes skill 3 from hero 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_skill(hero(0), skill(3), remove);`

`[](#__codelineno-5-1){"Data":{"Growth":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Hero":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"IsAdd":0,"Rank":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Skill":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.ChangeSkillCommand"}`