# User Interface Transitions

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-transition/*

---

# User Interface Transitions

## **User Interface Transitions**[¶](#user-interface-transitions "Permanent link")

User Interface Transitions are transitions that occur when opening or closing [User Interfaces](../).

* * *

#### **User Interface Transitions**[¶](#user-interface-transitions_1 "Permanent link")

*   [Fade In](#fade-in)
*   [Fade Out](#fade-out)
*   [Instant](#instant)
*   [Movement](#movement)
*   [Zoom](#zoom)

* * *

## **Fade In**[¶](#fade-in "Permanent link")

Fade In transitions gradually reveal the interface by fading in from a solid color.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The solid color to fade from.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../../05-reference/easing-function/)

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Fade Out**[¶](#fade-out "Permanent link")

Fade Out transitions gradually hide the interface by fading out to a solid color.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The solid color to fade from.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../../05-reference/easing-function/)

## **See Also**[¶](#see-also_1 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Instant**[¶](#instant "Permanent link")

Instant transitions complete immediately with no visual effect.

> **Note**: No properties are available for this transition, as it occurs instantly.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../../05-reference/easing-function/)

## **See Also**[¶](#see-also_2 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Movement**[¶](#movement "Permanent link")

Movement transitions slide the interface into view from a starting position to an ending position.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../../05-reference/easing-function/)

End Pixel X

The ending X coordinate in pixels.

Number

End Pixel Y

The ending Y coordinate in pixels.

Number

End Relative X

The ending X coordinate relative to the screen.

Number

End Relative Y

The ending Y coordinate relative to the screen.

Number

Start Pixel X

The starting X coordinate in pixels.

Number

Start Pixel Y

The starting Y coordinate in pixels.

Number

Start Relative X

The starting X coordinate relative to the screen.

Number

Start Relative Y

The starting Y coordinate relative to the screen.

Number

Use Relative Coordinates

Whether to use screen-relative coordinates instead of pixel coordinates for the start and end positions.

Toggle

## **See Also**[¶](#see-also_3 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Zoom**[¶](#zoom "Permanent link")

Zoom transitions scale the interface from a starting scale to an ending scale, centered on the screen.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../../05-reference/easing-function/)

End Scale

The scale of the interface at the end of the transition, where 1 is full size (100%).

Number

Start Scale

The scale of the interface at the start of the transition, where 1 is full size (100%).

Number

## **See Also**[¶](#see-also_4 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)