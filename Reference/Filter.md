# Filter

*Источник: https://docs.rpg-architect.com/05-reference/filter/*

---

# Filter

## **Filter**[¶](#filter "Permanent link")

Filters evaluate a property on an object against a value using a comparison operand. Used by [User Interface Contexts](../../10-user-interfaces/user-interface-context/) to narrow down displayed data.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Operator

The comparison operator used to evaluate the filter.

Operator

Property

The property name on the object to filter against. Supports [Tags](../tags/) access via "Tags\[key\]" syntax.

String

Value

The value to compare against. Supports "Global\[index\]" syntax to read from a [Global Variable](../variable/) at runtime.

String