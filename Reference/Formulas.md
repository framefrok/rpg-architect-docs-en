# Formulas

*Источник: https://docs.rpg-architect.com/05-reference/formulas/*

---

# Formulas

## **Formulas**[¶](#formulas "Permanent link")

RPG Architect includes a formula engine for creating custom formulas when working with [Statistics](../../06-database/05-statistics/01-statistics/), [Skills](../../06-database/01-skills/01-skills/), and related systems.

Success formulas operate on a scale of 0–100, where 100 guarantees success. The engine generates a random whole number between 0–99; if this number falls below the calculated result, the action succeeds.

## **Constants**[¶](#constants "Permanent link")

Name

Explanation

e

Euler's number (2.71828...).

pi

Pi (3.14159...).

## **Functions**[¶](#functions "Permanent link")

Name

Explanation

abs(x)

Absolute value. abs(-5) returns 5.

acos(x)

Arc cosine (inverse cosine).

acot(x)

Arc cotangent (inverse cotangent).

asin(x)

Arc sine (inverse sine).

atan(x)

Arc tangent (inverse tangent).

avg(...)

Arithmetic mean of the provided values.

ceiling(x)

Rounds up to the nearest integer. ceiling(1.2) returns 2.

cos(x)

Cosine.

dice(x, n)

Rolls x dice with n sides and returns the total.

dicepool(x, n, t)

Rolls x dice with n sides, counting rolls that meet or exceed the target t.

floor(x)

Rounds down to the nearest integer. floor(1.7) returns 1.

global(index)

Retrieves a global variable as a floating point value. Shorthand for globalfloat.

globalfloat(index)

Retrieves a global variable as a floating point value.

globalint(index)

Retrieves a global variable as an integer.

globalswitch(index)

Retrieves a global switch value (1 for true, 0 for false).

if(condition, true, false)

Returns the true value if the condition is non-zero, otherwise the false value.

lastfloat()

Returns the last generated formula result as a floating point value.

lastint()

Returns the last generated formula result as an integer.

local(index)

Retrieves a local variable on the current entity as a floating point value.

log10(x)

Base-10 logarithm.

loge(x)

Natural logarithm.

logn(base, x)

Logarithm with a custom base.

max(...)

Maximum value of the provided values.

median(...)

Middle value of the provided values.

min(...)

Minimum value of the provided values.

pow(base, exp)

Raises base to the power of exp. pow(2, 3) returns 8.

random()

Returns a random number between 0.0 and 1.0.

ref\_global(index)

Reads the value of global variable at index, then uses that value as an index to read a second global variable. Enables indirect/dynamic variable access.

ref\_local(index)

Reads the value of local variable at index, then uses that value as an index to read a second local variable. Enables indirect/dynamic variable access.

sin(x)

Sine.

sqrt(x)

Square root. sqrt(4) returns 2.