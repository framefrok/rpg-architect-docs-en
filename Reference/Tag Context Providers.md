# Tag Context Providers

*Источник: https://docs.rpg-architect.com/05-reference/tag-context-provider/*

---

# Tag Context Providers

## **Tag Context Providers**[¶](#tag-context-providers "Permanent link")

Tag Context Providers supply [Tags](../tags/) to [User Interfaces](../../06-database/09-user-interfaces/00-user-interfaces/) at runtime. They read data from game objects and expose it as key-value tag pairs that [User Interface Elements](../../10-user-interfaces/user-interface-element/) can display using templated values.

Providers are also used by the [Modify Tags](../../07-commands/01-data-manipulation/100-modify-tags/) command to add, change, or remove tags on objects identified by their [Unique ID](../unique-id/) (or, for variable-backed providers, by variable index).

* * *

#### **Tag Context Providers**[¶](#tag-context-providers_1 "Permanent link")

*   [Battler](#battler)
*   [Entity](#entity)
*   [Global Variable](#global-variable)
*   [Item](#item)
*   [Local Variable](#local-variable)
*   [Party](#party)
*   [Save State](#save-state)
*   [Skill Slot](#skill-slot)

* * *

## **Battler**[¶](#battler "Permanent link")

Provides [Tags](../tags/) from a battler in combat, such as name, statistics, status effects, and battle state.

* * *

## **Entity**[¶](#entity "Permanent link")

Provides [Tags](../tags/) from an entity instance on the current map or battle scene, such as an NPC, door, treasure chest, or other interactive map object.

* * *

## **Global Variable**[¶](#global-variable "Permanent link")

Reads and writes [Tags](../tags/) stored as serialized JSON inside a [Global Variable](../local-and-global-data/)'s value, identified by the variable's index.

* * *

## **Item**[¶](#item "Permanent link")

Provides [Tags](../tags/) from an item or equipment instance in the party's inventory, such as name, quantity, type, and custom tags.

* * *

## **Local Variable**[¶](#local-variable "Permanent link")

Reads and writes [Tags](../tags/) stored as serialized JSON inside a [Local Variable](../local-and-global-data/)'s value, identified by the variable's index.

* * *

## **Party**[¶](#party "Permanent link")

Provides [Tags](../tags/) from a hero in the party (outside of battle), such as name, class, statistics, and equipment.

* * *

## **Save State**[¶](#save-state "Permanent link")

Provides [Tags](../tags/) from a saved game state, such as save date, playtime, party members, and location. Writes flush to disk.

* * *

## **Skill Slot**[¶](#skill-slot "Permanent link")

Provides [Tags](../tags/) from a skill slot in a party member's skill list, such as name, type, and rank.