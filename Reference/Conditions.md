# Conditions

*Источник: https://docs.rpg-architect.com/05-reference/condition/*

---

# Conditions

## **Conditions**[¶](#conditions "Permanent link")

Conditions are used to determine if a [Script](../script/) or other element can run, sometimes paired with an [Interaction](../interaction/). They are leveraged in [Commands](../../07-commands/) as well as in [Entity Scripts](../entity/). You may recognize them from other programs or programming languages as the elements that get tested in an 'if statement.'

Conditions are 'evaluated,' which means the engine checks for that condition before executing the script.

! **Example**: An example of a [Conditional](../../07-commands/15-control-flow/00-conditional-%28if-then-else%29/) would be a door that's locked. A condition on the door can check for the [key's presence](./#item-exists) in the player's inventory - and only then will the script run and the door open!

* * *

#### **Conditions**[¶](#conditions_1 "Permanent link")

*   [Any](#any)
*   [Battle Action Successful](#battle-action-successful)
*   [Character in Party](#character-in-party)
*   [Entity Direction](#entity-direction)
*   [Global Reference Switch](#global-reference-switch)
*   [Global Reference Variable](#global-reference-variable)
*   [Global Switch](#global-switch)
*   [Global Variable](#global-variable)
*   [Global Variable Tag](#global-variable-tag)
*   [Hero Direction](#hero-direction)
*   [Item Equipped](#item-equipped)
*   [Item Exists](#item-exists)
*   [Local Reference Switch](#local-reference-switch)
*   [Local Reference Variable](#local-reference-variable)
*   [Local Switch](#local-switch)
*   [Local Variable](#local-variable)
*   [Local Variable Tag](#local-variable-tag)
*   [Money](#money)
*   [Random Value](#random-value)
*   [Scene](#scene)
*   [Tile Tag Collision](#tile-tag-collision)

* * *

## **Any**[¶](#any "Permanent link")

Any conditions evaluate to true when at least one of the contained conditions is true.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Conditions

The conditions to evaluate.

[Condition](./)

* * *

## **Battle Action Successful**[¶](#battle-action-successful "Permanent link")

Battle Action Successful conditions evaluate to true when the battle action driving the action sequence succeeded.

* * *

## **Character in Party**[¶](#character-in-party "Permanent link")

Character in Party conditions validate that a character is present in the active or inactive party.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Active Party

Whether to check if the character is in the active party.

Toggle

Character Reference

The referenced character in the database.

[Character](../../06-database/00-characters/00-characters/)

Inactive Party

Whether to check if the character is in the inactive party.

Toggle

* * *

## **Entity Direction**[¶](#entity-direction "Permanent link")

Entity Direction conditions validate the direction an entity is or is not facing.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Direction

The direction.

[Direction](../direction/)

Is Not Direction

Whether the condition should be inverted.

Toggle

* * *

## **Global Reference Switch**[¶](#global-reference-switch "Permanent link")

Global Reference Switch conditions validate a [Reference Switch](../reference-switch-or-variable/) is or is not set.

> **Note**: The **Index** is pulled from the [Global Variables](../local-and-global-data/) as well as the actual value.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Comparison Global Switch Index

The index of the [Global Switch](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Switch Index

The index of the [Local Switch](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the switch.

Number

Value

The value to compare to.

Toggle

* * *

## **Global Reference Variable**[¶](#global-reference-variable "Permanent link")

Global Reference Variable conditions validate the value in a [Reference Variable](../reference-switch-or-variable/).

> **Note**: The **Index** is pulled from the [Global Variables](../local-and-global-data/) as well as the actual value.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the variable.

Number

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Global Switch**[¶](#global-switch "Permanent link")

Global Switch conditions validate the value in a global switch.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Comparison Global Switch Index

The index of the [Global Switch](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Switch Index

The index of the [Local Switch](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the switch.

Number

Value

The value to compare to.

Toggle

* * *

## **Global Variable**[¶](#global-variable "Permanent link")

Global Variable conditions validate the value in a global variable.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the variable.

Number

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Global Variable Tag**[¶](#global-variable-tag "Permanent link")

Compares a tag value stored in a global variable's dictionary against a target value.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the global variable to compare against, if valid.

Number

Comparison Local Variable Index

The index of the local variable to compare against, if valid.

Number

Index

The index of the variable containing the tag dictionary.

Number

Key

The key to look up in the variable's tag dictionary.

String

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Hero Direction**[¶](#hero-direction "Permanent link")

Hero Direction conditions validate the direction the leader of the party is or is not facing.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Direction

The direction.

[Direction](../direction/)

Is Not Direction

Whether the condition should be inverted.

Toggle

* * *

## **Item Equipped**[¶](#item-equipped "Permanent link")

Item Equipped conditions validate that a piece of equipment is currently equipped by a party member.

## **Properties**[¶](#properties_9 "Permanent link")

#### **System**[¶](#system_9 "Permanent link")

Name

Explanation

Type

Actor

The specific actor to check for the equipped item.

Any Party Member

Whether to check all active party members for the equipment.

Toggle

Equipment Reference

The referenced equipment in the database.

[Equipment](../../06-database/02-items/02-equipment/)

* * *

## **Item Exists**[¶](#item-exists "Permanent link")

Item Exists conditions validate that an item or equipment is contained in the inventory.

> **Note**: This is an expensive condition and can only be used in [Commands](../../07-commands/).

## **Properties**[¶](#properties_10 "Permanent link")

#### **System**[¶](#system_10 "Permanent link")

Name

Explanation

Type

Equipment

Whether the condition is looking for a piece of equipment, rather than an item.

Toggle

Equipment or Item Reference

The reference item or equipment in the database.

[Item](../../06-database/02-items/01-items/) or [Equipment](../../06-database/02-items/02-equipment/)

Item

Whether the condition is looking for an item.

Toggle

Quantity

The quantity of item or equipment needed.

Number

* * *

## **Local Reference Switch**[¶](#local-reference-switch "Permanent link")

Local Reference Switch conditions validate a [Reference Switch](../reference-switch-or-variable/) is or is not set.

> **Note**: The **Index** is pulled from the [Local Variables](../local-and-global-data/), while the actual value is pulled from [Local Switches](../local-and-global-data/).

## **Properties**[¶](#properties_11 "Permanent link")

#### **System**[¶](#system_11 "Permanent link")

Name

Explanation

Type

Comparison Global Switch Index

The index of the [Global Switch](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Switch Index

The index of the [Local Switch](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the switch.

Number

Value

The value to compare to.

Toggle

* * *

## **Local Reference Variable**[¶](#local-reference-variable "Permanent link")

Local Reference Variable conditions validate the value in a [Reference Variable](../reference-switch-or-variable/).

> **Note**: The **Index** is pulled from the [Local Variables](../local-and-global-data/), while the actual value is pulled from [Local Variables](../local-and-global-data/).

## **Properties**[¶](#properties_12 "Permanent link")

#### **System**[¶](#system_12 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the variable.

Number

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Local Switch**[¶](#local-switch "Permanent link")

Local Switch conditions validate the value in a local switch.

## **Properties**[¶](#properties_13 "Permanent link")

#### **System**[¶](#system_13 "Permanent link")

Name

Explanation

Type

Comparison Global Switch Index

The index of the [Global Switch](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Switch Index

The index of the [Local Switch](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the switch.

Number

Value

The value to compare to.

Toggle

* * *

## **Local Variable**[¶](#local-variable "Permanent link")

Local Variable conditions validate the value in a local variable.

## **Properties**[¶](#properties_14 "Permanent link")

#### **System**[¶](#system_14 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the variable.

Number

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Local Variable Tag**[¶](#local-variable-tag "Permanent link")

Compares a tag value stored in a local variable's dictionary against a target value.

## **Properties**[¶](#properties_15 "Permanent link")

#### **System**[¶](#system_15 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the global variable to compare against, if valid.

Number

Comparison Local Variable Index

The index of the local variable to compare against, if valid.

Number

Index

The index of the variable containing the tag dictionary.

Number

Key

The key to look up in the variable's tag dictionary.

String

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Money**[¶](#money "Permanent link")

Money conditions validate the currently held money against a value.

## **Properties**[¶](#properties_16 "Permanent link")

#### **System**[¶](#system_16 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Operand

The type of comparison to make.

Operator

Value

The value to compare against.

Number

* * *

## **Random Value**[¶](#random-value "Permanent link")

Random Value conditions validate a randomly generated number, specified by a minimum and maximum value, against another variable or value.

## **Properties**[¶](#properties_17 "Permanent link")

#### **System**[¶](#system_17 "Permanent link")

Name

Explanation

Type

Comparison Global Variable Index

The index of the [Global Variable](../local-and-global-data/) to compare to, if valid.

Number

Comparison Local Variable Index

The index of the [Local Variable](../local-and-global-data/) to compare to, if valid.

Number

Index

The index of the variable.

Number

Maximum Value

The maximum value to generate.

Number

Minimum Value

The minimum value to generate.

Number

Operator

The type of comparison to make.

Operator

Value

The value to compare against.

[Variable](../variable/)

* * *

## **Scene**[¶](#scene "Permanent link")

Scene conditions validate whether the current scene matches a particular scene type.

## **Properties**[¶](#properties_18 "Permanent link")

#### **System**[¶](#system_18 "Permanent link")

Name

Explanation

Type

Not Current Scene

Whether to check if the scene is **not** the current scene.

Toggle

Scene

The scene.

[Scene](../scene/)

* * *

## **Tile Tag Collision**[¶](#tile-tag-collision "Permanent link")

Tile Tag Collision conditions validate that the container of the script is interacting with a particular [Tile Tag](../../06-database/03-maps/02-tile-tags/).

## **Properties**[¶](#properties_19 "Permanent link")

#### **System**[¶](#system_19 "Permanent link")

Name

Explanation

Type

Tile Tag

The referenced tile tag in the database.

[Tile Tag](../../06-database/03-maps/02-tile-tags/)