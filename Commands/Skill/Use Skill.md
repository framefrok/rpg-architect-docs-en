# Use Skill

*Источник: https://docs.rpg-architect.com/07-commands/07-skill/01-use-skill/*

---

# Use Skill

## **Use Skill**[¶](#use-skill "Permanent link")

Activates a skill from a hero's skill slot, targeting either a specific hero or the entire party.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Hero

The hero to target with the skill.

[Character](../../../06-database/00-characters/00-characters/)

Hero

When enabled, the skill targets a specific hero. When disabled, the skill targets all party members.

Toggle

Result

The switch to store whether the skill use succeeded.

[Switch or Value](../../../05-reference/switch-or-value/)

Skill

The skill slot to use.

[Skill](../../../06-database/01-skills/01-skills/)

Store Results

When enabled, the result of using the skill is stored in a switch.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Use a Skill Slot on Hero 0**[¶](#use-a-skill-slot-on-hero-0 "Permanent link")

This activates skill slot 0 targeting hero 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)use_skill(skill_slot(0), hero(0));`

`[](#__codelineno-1-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SkillSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"StoreResults":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"UseOnEntireParty":0,"UseOnHero":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.UseSkillCommand"}`

#### **Use a Skill Slot on the Entire Party**[¶](#use-a-skill-slot-on-the-entire-party "Permanent link")

This activates skill slot 0 targeting all members of the active party.

Code ScriptVisual Script

`[](#__codelineno-2-1)use_skill(skill_slot(0), all);`

`[](#__codelineno-3-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SkillSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"StoreResults":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":0,"IsUniqueID":1,"Metadata":null},"UseOnEntireParty":1,"UseOnHero":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.UseSkillCommand"}`

#### **Use a Skill Slot on Hero 2 and Store the Result**[¶](#use-a-skill-slot-on-hero-2-and-store-the-result "Permanent link")

This activates skill slot 1 targeting hero 2 and stores whether the skill use succeeded in Global Switch 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gs[0] = use_skill(skill_slot(1), hero(2));`

`[](#__codelineno-5-1){"Data":{"Result":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"SkillSlot":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"StoreResults":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"IsInstanceIndex":0,"IsReferenceIndex":1,"IsUniqueID":0,"Metadata":null},"UseOnEntireParty":0,"UseOnHero":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Skill.UseSkillCommand"}`