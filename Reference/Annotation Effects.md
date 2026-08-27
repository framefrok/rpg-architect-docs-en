# Annotation Effects

*Источник: https://docs.rpg-architect.com/05-reference/annotation-effect/*

---

# Annotation Effects

## **Annotation Effects**[¶](#annotation-effects "Permanent link")

Annotation Effects alter and modify [Annotations](../annotation/), allowing for animation.

> **Note**: Annotation Effects have **Start** and **Duration** properties, which control where the effect will occur.

* * *

#### **Annotation Effects**[¶](#annotation-effects_1 "Permanent link")

*   [Color](#color)
*   [Font](#font)
*   [Movement](#movement)
*   [Negative Value](#negative-value)
*   [Number Formatter](#number-formatter)
*   [Text](#text)
*   [Wait](#wait)

* * *

## **Color**[¶](#color "Permanent link")

Color effects change the color of the annotation.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Color

The color to apply to the annotation.

Color

Duration

The duration of the effect in milliseconds.

Number

Start

The starting time of the effect in milliseconds.

Number

* * *

## **Font**[¶](#font "Permanent link")

Font effects change the font of any text in the annotation.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Font

The font to apply to the annotation's text, replacing its current font settings.

[Font](../font/)

Start

The starting time of the effect in milliseconds.

Number

* * *

## **Movement**[¶](#movement "Permanent link")

Movement effects change the position of the annotation over time.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Start

The starting time of the effect in milliseconds.

Number

#### **Acceleration**[¶](#acceleration "Permanent link")

Name

Explanation

Type

Acceleration

The acceleration applied to the annotation's velocity each second, in world-space units.

Vector

#### **Velocity**[¶](#velocity "Permanent link")

Name

Explanation

Type

Velocity

The initial velocity of the annotation in world-space units per second.

Vector

* * *

## **Negative Value**[¶](#negative-value "Permanent link")

Negative Value effects multiply any numeric values displayed in the annotation by -1.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Start

The starting time of the effect in milliseconds.

Number

* * *

## **Number Formatter**[¶](#number-formatter "Permanent link")

Number Formatter effects apply different sub-effects depending on whether the annotation's text is a positive, negative, zero, or non-numeric value.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Negative Effects

The effects to apply if the number is negative.

[Annotation Effect](./)

Null Effects

The effects to apply if no number is provided.

[Annotation Effect](./)

Positive Effects

The effects to apply if the number is positive.

[Annotation Effect](./)

Start

The starting time of the effect in milliseconds.

Number

Zero Effects

The effects to apply if the number is zero.

[Annotation Effect](./)

* * *

## **Text**[¶](#text "Permanent link")

Text effects replace the displayed string content of a text annotation when activated.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Start

The starting time of the effect in milliseconds.

Number

Text

The replacement text to display when this effect activates. Supports localization.

String

* * *

## **Wait**[¶](#wait "Permanent link")

Wait effects create a delay and extend the length of the annotation's effect sequence.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Duration

The duration of the effect in milliseconds.

Number

Start

The starting time of the effect in milliseconds.

Number