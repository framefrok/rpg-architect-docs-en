# Battle Action Results

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/battle-action-result/*

---

# Battle Action Results

## **Battle Action Results**[¶](#battle-action-results "Permanent link")

Battle Action Results represent the data outcome of a battle action, such as a statistic change, a status effect application, or a message. They are the counterpart to the visual [Action Sequence Result](../action-sequence-result/), which controls how results are displayed on screen.

* * *

#### **Battle Action Results**[¶](#battle-action-results_1 "Permanent link")

*   [Battle Counter Result](#battle-counter-result)
*   [Message Result](#message-result)
*   [State Result](#state-result)
*   [Statistics Result](#statistics-result)

* * *

## **Battle Counter Result**[¶](#battle-counter-result "Permanent link")

A battle action result that modifies the battle counter value on the target, used in counter-based battle systems.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Value

The value to apply to the battle counter.

Number

* * *

## **Message Result**[¶](#message-result "Permanent link")

A battle action result that displays a message without affecting any statistics or states.

* * *

## **State Result**[¶](#state-result "Permanent link")

A battle action result that applies or removes a status effect on the target.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Is Add

Whether the status effect is being added or removed.

Toggle

Statistics

The statistics associated with the status effect.

[Statistic](../../../06-database/05-statistics/01-statistics/)

Status Effect

The status effect to apply or remove.

[Status Effect](../../../06-database/05-statistics/03-status-effects/)

Success Formula

The formula that determines whether the status effect is successfully applied or removed.

[Formula](../../../05-reference/formulas/)

* * *

## **Statistics Result**[¶](#statistics-result "Permanent link")

A battle action result that modifies a statistic on the target, such as dealing damage to HP or restoring MP.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Formula Name

The formula name of the statistic to modify.

[Statistic](../../../06-database/05-statistics/01-statistics/)

Value

The value to apply to the statistic.

Number