# Result Modifier

*Источник: https://docs.rpg-architect.com/11-battles/01-action-sequences/action-sequence-element/result-modifier/*

---

# Result Modifier

## **Result Modifier**[¶](#result-modifier "Permanent link")

Result Modifier elements alter the numerical outcome of a battle action result using an operation and operand.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Action Result Type

The battle action result type to affect.

[Battle Action Result](../../battle-action-result/)

Apply to Target

Whether the result modifier applies to the target.

Toggle

Apply to User

Whether the result modifier applies to the user.

Toggle

Formula Name

The formula name to filter on.

[Variable or Value](../../../../05-reference/variable-or-value/)

Operation

The operation to perform on the result.

Operator

Start Time (milliseconds)

The time to start the sequence element at in milliseconds.

Number

Value

The value to apply on the result.

[Variable or Value](../../../../05-reference/variable-or-value/)

Wait to Complete

Whether this element must finish before the next element begins.

Toggle

#### **[Operation](#operation)**[¶](#operation "Permanent link")

Name

Explanation

\=

Replaces the current value with the specified value.

+

Adds the specified value to the current value.

\-

Subtracts the specified value from the current value.

\*

Multiplies the current value by the specified value.

÷

Divides the current value by the specified value.

%

Returns the remainder after dividing the current value by the specified value.