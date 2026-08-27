# Variable Manipulators

*Источник: https://docs.rpg-architect.com/05-reference/variable-manipulator/*

---

# Variable Manipulators

## **Variable Manipulators**[¶](#variable-manipulators "Permanent link")

Variable Manipulators are auxiliary methods that can be used on [Variables](../variable/) to alter their value. They are leveraged by the [Variable Manipulation](../../07-commands/01-data-manipulation/10-variable-manipulation/) command.

> **Note**: Variable Manipulators offer more than mathematical functions, as they can do scene calculations (e.g. **Screen to World**), array operations (e.g. **Pop From Array**), and more.

* * *

#### **Variable Manipulators**[¶](#variable-manipulators_1 "Permanent link")

*   [Absolute Value](#absolute-value)
*   [Arccosine](#arccosine)
*   [Arcsine](#arcsine)
*   [Arctangent](#arctangent)
*   [Cast to Floating Point](#cast-to-floating-point)
*   [Cast to Integer](#cast-to-integer)
*   [Ceiling](#ceiling)
*   [Cosine](#cosine)
*   [Exponent](#exponent)
*   [Floor](#floor)
*   [From Array](#from-array)
*   [Length](#length)
*   [Logarithm](#logarithm)
*   [Lowercase](#lowercase)
*   [Pop](#pop)
*   [Pop From Array](#pop-from-array)
*   [Push To Array](#push-to-array)
*   [Replace](#replace)
*   [Round](#round)
*   [Screen to World Coordinates](#screen-to-world-coordinates)
*   [Sine](#sine)
*   [Substring](#substring)
*   [Tangent](#tangent)
*   [To Array](#to-array)
*   [Trim](#trim)
*   [Uppercase](#uppercase)
*   [World to Screen Coordinates](#world-to-screen-coordinates)

* * *

## **Absolute Value**[¶](#absolute-value "Permanent link")

Absolute Value manipulators apply the absolute value to the variable.

* * *

## **Arccosine**[¶](#arccosine "Permanent link")

Arccosine manipulators calculate the arccosine of the specified value.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **Arcsine**[¶](#arcsine "Permanent link")

Arcsine manipulators calculate the arcsine of the specified value.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **Arctangent**[¶](#arctangent "Permanent link")

Arctangent manipulators calculate the arctangent of the specified value.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **Cast to Floating Point**[¶](#cast-to-floating-point "Permanent link")

Cast to Floating Point manipulators cast a variable to a floating point.

* * *

## **Cast to Integer**[¶](#cast-to-integer "Permanent link")

Cast to Integer manipulators cast a variable to an integer.

* * *

## **Ceiling**[¶](#ceiling "Permanent link")

Ceiling manipulators round a variable up to the nearest integer.

* * *

## **Cosine**[¶](#cosine "Permanent link")

Cosine manipulators calculate the cosine of the specified value.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **Exponent**[¶](#exponent "Permanent link")

Exponent manipulators raise the variable to a specified power.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Power

The exponent to use on the variable.

[Variable or Value](../variable-or-value/)

* * *

## **Floor**[¶](#floor "Permanent link")

Floor manipulators round a variable down to the nearest integer.

* * *

## **From Array**[¶](#from-array "Permanent link")

From Array manipulators join an array back into a string.

> **Note**: The default **Separator** is a space.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Separator

The separator used to stitch the array into a string.

[Variable or Value](../variable-or-value/)

* * *

## **Length**[¶](#length "Permanent link")

Length manipulators calculate the length of the value in the variable.

* * *

## **Logarithm**[¶](#logarithm "Permanent link")

Logarithm manipulators calculate the log value of the variable.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Log Base

The logarithmic base to use when calculating log values.

[Variable or Value](../variable-or-value/)

* * *

## **Lowercase**[¶](#lowercase "Permanent link")

Lowercase manipulators convert a string to lowercase.

* * *

## **Pop**[¶](#pop "Permanent link")

Pop manipulators remove the last character from a string.

* * *

## **Pop From Array**[¶](#pop-from-array "Permanent link")

Pop From Array manipulators remove an element at a specified index from an array.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Destination

The destination to pop the value into.

[Variable or Value](../variable-or-value/)

Index

The index in the array.

[Variable or Value](../variable-or-value/)

* * *

## **Push To Array**[¶](#push-to-array "Permanent link")

Push To Array manipulators insert a value into an array at a specified index.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Index

The index in the array.

[Variable or Value](../variable-or-value/)

Operand

The value to push into the array.

[Variable or Value](../variable-or-value/)

* * *

## **Replace**[¶](#replace "Permanent link")

Replace manipulators substitute matching text within a string.

## **Properties**[¶](#properties_9 "Permanent link")

#### **System**[¶](#system_9 "Permanent link")

Name

Explanation

Type

Replacement

The replacement value.

[Variable or Value](../variable-or-value/)

Search

The search value.

[Variable or Value](../variable-or-value/)

* * *

## **Round**[¶](#round "Permanent link")

Round manipulators round the variable to the specified number of digits.

## **Properties**[¶](#properties_10 "Permanent link")

#### **System**[¶](#system_10 "Permanent link")

Name

Explanation

Type

Digits

The number of digits to round to.

[Variable or Value](../variable-or-value/)

* * *

## **Screen to World Coordinates**[¶](#screen-to-world-coordinates "Permanent link")

Screen to World Coordinates manipulators convert variables from screen space to world space.

> **Note**: This has multiple inputs or outputs.

## **Properties**[¶](#properties_11 "Permanent link")

#### **System**[¶](#system_11 "Permanent link")

Name

Explanation

Type

Screen Depth

The screen's depth-coordinate.

[Variable or Value](../variable-or-value/)

Screen X

The screen's x-coordinate.

[Variable or Value](../variable-or-value/)

Screen Y

The screen's y-coordinate.

[Variable or Value](../variable-or-value/)

World X

The world's x-coordinate output.

[Variable](../variable/)

World Y

The world's y-coordinate output.

[Variable](../variable/)

World Z

The world's z-coordinate output.

[Variable](../variable/)

* * *

## **Sine**[¶](#sine "Permanent link")

Sine manipulators calculate the sine of the specified value.

## **Properties**[¶](#properties_12 "Permanent link")

#### **System**[¶](#system_12 "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **Substring**[¶](#substring "Permanent link")

Substring manipulators extract a portion of a string by index and length.

## **Properties**[¶](#properties_13 "Permanent link")

#### **System**[¶](#system_13 "Permanent link")

Name

Explanation

Type

Index

The index to start the substring at.

[Variable or Value](../variable-or-value/)

Length

The length of the substring to acquire.

[Variable or Value](../variable-or-value/)

* * *

## **Tangent**[¶](#tangent "Permanent link")

Tangent manipulators calculate the tangent of the specified value.

## **Properties**[¶](#properties_14 "Permanent link")

#### **System**[¶](#system_14 "Permanent link")

Name

Explanation

Type

Degrees

Whether to use degrees.

Toggle

Measurement

The measurement to operate on.

[Variable or Value](../variable-or-value/)

Radians

Whether to use radians.

Toggle

* * *

## **To Array**[¶](#to-array "Permanent link")

To Array manipulators convert a string into an array of characters.

* * *

## **Trim**[¶](#trim "Permanent link")

Trim manipulators remove whitespace from the beginning and end of a string.

* * *

## **Uppercase**[¶](#uppercase "Permanent link")

Uppercase manipulators convert a string to uppercase.

* * *

## **World to Screen Coordinates**[¶](#world-to-screen-coordinates "Permanent link")

World to Screen Coordinates manipulators convert variables from world space to screen space.

> **Note**: This has multiple inputs or outputs.

## **Properties**[¶](#properties_15 "Permanent link")

#### **System**[¶](#system_15 "Permanent link")

Name

Explanation

Type

Screen X

The screen's x-coordinate output.

[Variable](../variable/)

Screen Y

The screen's y-coordinate output.

[Variable](../variable/)

World X

The world's x-coordinate.

[Variable or Value](../variable-or-value/)

World Y

The world's y-coordinate.

[Variable or Value](../variable-or-value/)

World Z

The world's z-coordinate.

[Variable or Value](../variable-or-value/)