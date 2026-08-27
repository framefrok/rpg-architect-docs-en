# Restore Party

*Источник: https://docs.rpg-architect.com/07-commands/08-party/10-restore-party/*

---

# Restore Party

## **Restore Party**[¶](#restore-party "Permanent link")

Restores all party members to full health and removes status effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Clear Status Effects

Whether to remove all status effects from party members.

[Switch or Value](../../../05-reference/switch-or-value/)

Include Inactive Members

Whether to also restore inactive (reserve) party members.

[Switch or Value](../../../05-reference/switch-or-value/)

Restore Statistics

Whether to restore statistics such as health and mana to their maximum values.

[Switch or Value](../../../05-reference/switch-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Fully Restore the Entire Party**[¶](#fully-restore-the-entire-party "Permanent link")

This restores all party members, including inactive members, to full health and removes all status effects.

Code ScriptVisual Script

`[](#__codelineno-0-1)restore_party(true, true, true);`

`[](#__codelineno-1-1){"Data":{"IncludeInactiveMembers":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeStatistics":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.RestorePartyCommand"}`

#### **Restore Only Active Party Members**[¶](#restore-only-active-party-members "Permanent link")

This restores only the active party members to full health and removes status effects, excluding inactive members.

Code ScriptVisual Script

`[](#__codelineno-2-1)restore_party(false, true, true);`

`[](#__codelineno-3-1){"Data":{"IncludeInactiveMembers":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeStatistics":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.RestorePartyCommand"}`

#### **Restore Party Using Global Switches**[¶](#restore-party-using-global-switches "Permanent link")

This restores the party with all three options controlled by Global Switches 0, 1, and 2.

Code ScriptVisual Script

`[](#__codelineno-4-1)restore_party($gs[0], $gs[1], $gs[2]);`

`[](#__codelineno-5-1){"Data":{"IncludeInactiveMembers":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":0,"Metadata":null},"IncludeStatistics":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":1,"Metadata":null},"IncludeStatus":{"IsGlobalSwitch":true,"IsLocalSwitch":false,"IsValue":false,"Value":false,"SwitchIndex":2,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Party.RestorePartyCommand"}`