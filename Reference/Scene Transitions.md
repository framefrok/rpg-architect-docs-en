# Scene Transitions

*Источник: https://docs.rpg-architect.com/05-reference/scene-transition/*

---

# Scene Transitions

## **Scene Transitions**[¶](#scene-transitions "Permanent link")

Scene Transitions are screen transitions that occur when switching between [Scenes](../scene/) or Maps.

> **Note**: These can also be manually run using the [Show Screen](../../07-commands/09-animation/50-show-screen/) and [Hide Screen](../../07-commands/09-animation/51-hide-screen/) commands.

* * *

#### **Scene Transitions**[¶](#scene-transitions_1 "Permanent link")

*   [Fade In](#fade-in)
*   [Fade Out](#fade-out)
*   [Gradient Wipe In](#gradient-wipe-in)
*   [Gradient Wipe Out](#gradient-wipe-out)
*   [Horizontal Shutter In](#horizontal-shutter-in)
*   [Horizontal Shutter Out](#horizontal-shutter-out)
*   [Instant](#instant)
*   [Shatter](#shatter)
*   [Vertical Shutter In](#vertical-shutter-in)
*   [Vertical Shutter Out](#vertical-shutter-out)
*   [Zoom](#zoom)

* * *

## **Fade In**[¶](#fade-in "Permanent link")

Fade In transitions gradually reveal the scene by fading in from a solid color.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The solid color that the scene fades in from. Defaults to black.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Fade Out**[¶](#fade-out "Permanent link")

Fade Out transitions gradually obscure the scene by fading out to a solid color.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The solid color that the scene fades out to. Defaults to black.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_1 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Gradient Wipe In**[¶](#gradient-wipe-in "Permanent link")

Gradient Wipe In transitions reveal the scene using a gradient image to control the wipe pattern.

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

[Easing Function](../easing-function/)

Gradient Image

The gradient image that controls the wipe pattern. Brighter pixels reveal or hide first.

[Image](../image/)

## **See Also**[¶](#see-also_2 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Gradient Wipe Out**[¶](#gradient-wipe-out "Permanent link")

Gradient Wipe Out transitions hide the scene using a gradient image to control the wipe pattern.

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

[Easing Function](../easing-function/)

Gradient Image

The gradient image that controls the wipe pattern. Brighter pixels reveal or hide first.

[Image](../image/)

## **See Also**[¶](#see-also_3 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Horizontal Shutter In**[¶](#horizontal-shutter-in "Permanent link")

Horizontal Shutter In transitions close a solid-color shutter inward from the left and right edges of the screen.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The color of the shutter.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_4 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Horizontal Shutter Out**[¶](#horizontal-shutter-out "Permanent link")

Horizontal Shutter Out transitions open a solid-color shutter outward toward the left and right edges of the screen.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The color of the shutter.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_5 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Instant**[¶](#instant "Permanent link")

Instant transitions complete immediately with no visual effect between scenes.

> **Note**: No properties are available for this transition, as it occurs instantly.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_6 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Shatter**[¶](#shatter "Permanent link")

Shatter transitions break the scene into random glass shards that spin and fall away, revealing black.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Crack Color

The color of the fracture lines drawn along shard edges when Show Crack Lines is enabled.

Color

Depth Tumble

When enabled, shards burst outward with an eased pop and subtly scale as they tumble, adding depth.

Toggle

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

Gravity

A multiplier on the downward pull applied to shards as they fly apart. 0 disables falling.

Number

Impact Beat

When enabled, the cracked scene holds and shudders with a brief flash before the shards fly apart.

Toggle

Origin X

The horizontal point the shatter radiates from, where 0 is the left edge and 1 is the right edge.

Number

Origin Y

The vertical point the shatter radiates from, where 0 is the top edge and 1 is the bottom edge.

Number

Per-Shard Shading

When enabled, shards fade individually as they travel and flicker with a facet glint as they tumble.

Toggle

Piece Count

The number of glass shards the screen breaks into.

Number

Randomize Origin

When enabled, the impact point is chosen randomly each time the transition plays.

Toggle

Seed

The random seed for the shatter. 0 breaks differently each play; any other value locks in a repeatable pattern.

Number

Show Crack Lines

When enabled, fracture lines are drawn along shard edges so the break reads as cracked glass.

Toggle

Spin

A multiplier on how much each shard tumbles as it flies away. 0 disables spinning.

Number

Spread

A multiplier on how fast shards fly outward from the impact origin.

Number

## **See Also**[¶](#see-also_7 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Vertical Shutter In**[¶](#vertical-shutter-in "Permanent link")

Vertical Shutter In transitions close a solid-color shutter inward from the top and bottom edges of the screen.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The color of the shutter.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_8 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Vertical Shutter Out**[¶](#vertical-shutter-out "Permanent link")

Vertical Shutter Out transitions open a solid-color shutter outward toward the top and bottom edges of the screen.

## **Properties**[¶](#properties_9 "Permanent link")

#### **System**[¶](#system_9 "Permanent link")

Name

Explanation

Type

Blend Mode

The blend mode used when compositing the transition to the screen.

BlendMode

Color

The color of the shutter.

Color

Duration

The duration of the transition in milliseconds.

Number

Easing Function

The easing function to determine the progress of the transition.

[Easing Function](../easing-function/)

## **See Also**[¶](#see-also_9 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)

* * *

## **Zoom**[¶](#zoom "Permanent link")

Zoom transitions scale the scene from a starting scale to an ending scale, centered on the screen.

## **Properties**[¶](#properties_10 "Permanent link")

#### **System**[¶](#system_10 "Permanent link")

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

[Easing Function](../easing-function/)

End Scale

The scale of the scene at the end of the transition, where 1 is full size (100%).

Number

Start Scale

The scale of the scene at the start of the transition, where 1 is full size (100%).

Number

## **See Also**[¶](#see-also_10 "Permanent link")

*   [Easing Function Editor](../../04-editor/easing-function-editor/)