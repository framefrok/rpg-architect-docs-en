# Add Battle Log

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/160-add-battle-log/*

---

# Add Battle Log

## **Add Battle Log**[¶](#add-battle-log "Permanent link")

Appends a message to the battle log during combat.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Message

The message to display in the battle log.

String

## **Examples**[¶](#examples "Permanent link")

#### **Add a Message to the Battle Log**[¶](#add-a-message-to-the-battle-log "Permanent link")

This appends a text message to the battle log during combat.

Code ScriptVisual Script

`[](#__codelineno-0-1)add_battle_log("The enemy is weakening!");`

`[](#__codelineno-1-1){"Data":{"Message":"The enemy is weakening!","Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.AddBattleLogCommand"}`