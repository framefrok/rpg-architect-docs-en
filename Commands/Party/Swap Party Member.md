# Swap Party Member

*Источник: https://docs.rpg-architect.com/07-commands/08-party/03-swap-party-member/*

---

# Swap Party Member

## **Swap Party Member**[¶](#swap-party-member "Permanent link")

Exchanges the positions of two characters in the party.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add to Scene

Whether the change is immediately reflected in the current scene. When enabled, the party display on the map updates right away.

Toggle

Source

The first party member to swap.

[Actor Reference](../../../05-reference/actor-reference/)

Target

The second party member to swap with the source.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Swap Two Party Members**[¶](#swap-two-party-members "Permanent link")

This exchanges the positions of party member 0 and party member 1 in the party.

Code ScriptVisual Script

`[](#__codelineno-0-1)swap_party_member(party(0), party(1));`

`[](#__codelineno-1-1){"Data":{"IsReflectedImmediately":0,"Source":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.SwapPartyMemberCommand"}`

#### **Swap Two Party Members with Immediate Scene Update**[¶](#swap-two-party-members-with-immediate-scene-update "Permanent link")

This exchanges two party members and immediately updates the scene to reflect the change.

Code ScriptVisual Script

`[](#__codelineno-2-1)swap_party_member(party(0), party(1), immediate);`

`[](#__codelineno-3-1){"Data":{"IsReflectedImmediately":1,"Source":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":1,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.SwapPartyMemberCommand"}`