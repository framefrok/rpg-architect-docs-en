# Set Scheduling Battler

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/90-set-scheduling-battler/*

---

# Set Scheduling Battler

## **Set Scheduling Battler**[¶](#set-scheduling-battler "Permanent link")

Designates a battler as the scheduling battler, exposing their available commands so actions can be added to the queue. Primarily used in script-based battles to request input from a specific battler. The script suspends on this command while the battler makes their selection and resumes once the scheduling battler is cleared. Call with no argument (or an empty unique ID) to clear the scheduling battler.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battler Unique ID

The unique ID of the battler to set as the scheduling battler. Provide an empty value to clear the scheduling battler.

[Variable or Value](../../../05-reference/variable-or-value/)

Run Battle Program

When enabled, an enemy battler runs its battle program to schedule an action automatically instead of being set up for input.

Toggle