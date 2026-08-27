# Message Box

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-type/message-box/*

---

# Message Box

## **Message Box**[¶](#message-box "Permanent link")

Message Box types display text to the player.

> **Note**: For example, character dialogue, narration, or informing the player about an action.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Body Border Element

The element that wraps the body content.

[User Interface Element](../../user-interface-element/)

Body Element

The element that hosts the body content.

[User Interface Element](../../user-interface-element/)

Collate Messages

Whether or not to maintain the same message box between displaying messages.

Toggle

Header Border Element

The element that wraps the header content.

[User Interface Element](../../user-interface-element/)

Header Element

The element that hosts the header content.

[User Interface Element](../../user-interface-element/)

Pagination Strategy

The method of displaying more text when space runs out.

[Text Pagination Strategy](#text-pagination-strategy)

Pause Gameplay

Whether or not to pause gameplay from continuing while the message box is open.

Toggle

Portrait Element

The element that hosts the portrait.

[User Interface Element](../../user-interface-element/)

Prompt Element

The element that displays when a message is finished displaying.

[User Interface Element](../../user-interface-element/)

Shrink Body

Whether or not to fit the body border to the body content.

Toggle

Shrink Header

Whether or not to fit the header border to the header content.

Toggle

Tail Bottom Element

The picture element displayed as a tail pointing downward toward the target.

[User Interface Element](../../user-interface-element/)

Tail Left Element

The picture element displayed as a tail pointing left toward the target.

[User Interface Element](../../user-interface-element/)

Tail Right Element

The picture element displayed as a tail pointing right toward the target.

[User Interface Element](../../user-interface-element/)

Tail Top Element

The picture element displayed as a tail pointing upward toward the target.

[User Interface Element](../../user-interface-element/)

Vertical Pagination Speed

The vertical speed to use when paginating.

Number

#### **[Text Pagination Strategy](#text-pagination-strategy)**[¶](#text-pagination-strategy "Permanent link")

Name

Explanation

Clear Text

The text is completely cleared and the next set of lines is displayed.

Retain Line

The text scrolls up one line at a time, requiring confirmation to continue.

Retain Paragraph

The text scrolls up a full paragraph at a time, requiring confirmation to continue.