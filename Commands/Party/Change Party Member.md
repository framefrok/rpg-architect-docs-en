# Change Party Member

*Источник: https://docs.rpg-architect.com/07-commands/08-party/02-change-party-member/*

---

# Change Party Member

## **Change Party Member**[¶](#change-party-member "Permanent link")

Moves a character between the active and inactive party.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add to Scene

Whether the change is immediately reflected in the current scene. When enabled, the party display on the map updates right away.

Toggle

Target

The party member to move between the active and inactive party.

[Actor Reference](../../../05-reference/actor-reference/)

To Active

Whether to move the target character to the active party.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Move a Party Member to the Inactive Party**[¶](#move-a-party-member-to-the-inactive-party "Permanent link")

This moves party member 0 from the active party to the inactive (reserve) party.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_party_member(party(0));`

`[](#__codelineno-1-1){"Data":{"IsActive":0,"IsReflectedImmediately":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.ChangePartyMemberCommand"}`

#### **Move a Party Member to the Active Party**[¶](#move-a-party-member-to-the-active-party "Permanent link")

This moves party member 0 to the active party.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_party_member(party(0), active);`

`[](#__codelineno-3-1){"Data":{"IsActive":1,"IsReflectedImmediately":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.ChangePartyMemberCommand"}`

#### **Move a Party Member to Active with Immediate Scene Update**[¶](#move-a-party-member-to-active-with-immediate-scene-update "Permanent link")

This moves party member 0 to the active party and immediately updates the scene to reflect the change.

Code ScriptVisual Script

`[](#__codelineno-4-1)change_party_member(party(0), active, immediate);`

`[](#__codelineno-5-1){"Data":{"IsActive":1,"IsReflectedImmediately":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.ChangePartyMemberCommand"}`