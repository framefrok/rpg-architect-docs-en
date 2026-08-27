# Array

*Источник: https://docs.rpg-architect.com/05-reference/array/*

---

# Array

## **Array**[¶](#array "Permanent link")

Arrays are [Variables](../variable/) that contain more than a single value, accessed by an **Index**. In a way, this is analogous to how Variables and Switches work as well, as they require an **Index** (the Variable or Switch "Number") to access. Indices are zero-based, meaning that the first **Index** will be 0.

Any Variable can be an Array. For example, an Array containing the values `a`, `b`, and `255` would look like this:

Index

0

1

2

Value

a

b

255

Underneath the covers, Arrays are stored as a JSON-formatted array. The example above would be represented as:

`[](#__codelineno-0-1)["a", "b", 255]`