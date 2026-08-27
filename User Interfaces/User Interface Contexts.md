# User Interface Contexts

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-context/*

---

# User Interface Contexts

## **User Interface Contexts**[¶](#user-interface-contexts "Permanent link")

Some [User Interfaces Types](../user-interface-type/) have the ability to natively display data from in-game, as well as [Filter](../../05-reference/filter/) on it to take a subset.

* * *

#### **Contexts**[¶](#contexts "Permanent link")

*   [Active and Inactive Party](#active-and-inactive-party)
*   [Active Party](#active-party)
*   [Battlers](#battlers)
*   [Data Entries](#data-entries)
*   [Inactive Party](#inactive-party)
*   [Inventory](#inventory)
*   [Save States](#save-states)
*   [Scheduled Actions](#scheduled-actions)
*   [Scheduling Battler Commands](#scheduling-battler-commands)
*   [Turn Order](#turn-order)

* * *

## **Active and Inactive Party**[¶](#active-and-inactive-party "Permanent link")

Active and Inactive Party context providers supply all active and inactive party members to the user interface.

* * *

## **Active Party**[¶](#active-party "Permanent link")

Active Party context providers supply all active party members to the user interface.

* * *

## **Battlers**[¶](#battlers "Permanent link")

Battlers context providers supply all battlers, active or inactive, to the user interface.

* * *

## **Data Entries**[¶](#data-entries "Permanent link")

Data Entries context providers supply all [Data Entries](../../06-database/04-data-entries/00-data-entries/) stored in the database to the user interface.

> **Note**: The results are not filtered by enabled state. Use a [Filter](../../05-reference/filter/) to sort on **IsEnabled** to limit results to only those that have conditions fulfilled.

* * *

## **Inactive Party**[¶](#inactive-party "Permanent link")

Inactive Party context providers supply all inactive party members to the user interface.

* * *

## **Inventory**[¶](#inventory "Permanent link")

Inventory context providers supply all inventory slots, whether filled or empty, to the user interface.

* * *

## **Save States**[¶](#save-states "Permanent link")

Save States context providers supply all save state slots, including empty ones, to the user interface.

* * *

## **Scheduled Actions**[¶](#scheduled-actions "Permanent link")

Scheduled Actions context providers supply all scheduled battle actions to the user interface.

* * *

## **Scheduling Battler Commands**[¶](#scheduling-battler-commands "Permanent link")

Scheduling Battler Commands context providers supply all grouped battle commands for the battler currently inputting their action.

* * *

## **Turn Order**[¶](#turn-order "Permanent link")

Turn Order context providers supply the battlers in the order they will act next to the user interface.