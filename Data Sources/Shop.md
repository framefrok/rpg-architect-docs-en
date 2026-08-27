# Shop

*Источник: https://docs.rpg-architect.com/08-data-sources/shop/*

---

# Shop

## **Shop**[¶](#shop "Permanent link")

Shop data sources get information about a shop.

## **Properties**[¶](#properties "Permanent link")

#### **Properties**[¶](#properties_1 "Permanent link")

Name

Explanation

Type

Name

The name of the shop.

String

Buy Item Count

The number of items.

Number

Buy Item Unique ID

The unique ID of the shop item at a current position.

[Unique ID](../../05-reference/unique-id/)

Sell Item Count

The number of items the player can sell.

Number

Sell Item Unique ID

The unique ID of the sell item at a current position.

[Unique ID](../../05-reference/unique-id/)

Buy Modifier

The buy modifier for the shop.

Number

Sell Modifier

The sell modifier for the shop.

Number

Currency

The currency amount.

Number

Currency Variable Index

The variable index for the currency, if using a variable.

Number

Category Count

The number of categories.

Number

Category Unique ID

The unique ID of the category at the current position.

[Unique ID](../../05-reference/unique-id/)

Item Array - Unique ID

The items in an array.

[Array](../../05-reference/array/)

Category Array - Unique ID

The categories in an array.

[Array](../../05-reference/array/)

#### **Flags**[¶](#flags "Permanent link")

Name

Explanation

Type

Is Buying Allowed

Whether buying is allowed.

Toggle

Is Selling Allowed

Whether selling is allowed.

Toggle

Is Using Money For Currency

Whether the currency is sourced from .

Toggle

Is Using Variable For Currency

Whether the currency is sourced from a variable.

Toggle

Is Using Local Variable For Currency

Whether the currency is sourced from a local variable.

Toggle

Is Using Global Variable For Currency

Whether the currency is sourced from a global variable.

Toggle