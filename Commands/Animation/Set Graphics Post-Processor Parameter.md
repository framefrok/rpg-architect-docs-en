# Set Graphics Post-Processor Parameter

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/63-set-graphics-post-processor-parameter/*

---

# Set Graphics Post-Processor Parameter

## **Set Graphics Post-Processor Parameter**[¶](#set-graphics-post-processor-parameter "Permanent link")

Sets a named parameter (such as intensity) on a runtime post-processing effect, referenced by its unique ID as returned by Add Graphics Post-Processor. The change can be applied instantly or eased over time.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Easing Function

The easing function that controls how the parameter transitions to its target value over time. Leave it instant to set the value immediately.

[Easing Function](../../../05-reference/easing-function/)

Parameter

The name of the parameter to set, such as intensity.

[Variable or Value](../../../05-reference/variable-or-value/)

Run Asynchronously

Whether the transition runs asynchronously, allowing subsequent commands to execute without waiting.

Toggle

Unique ID

The unique ID of the runtime post-processing effect to adjust.

[Variable or Value](../../../05-reference/variable-or-value/)

Value

The value to set the parameter to.

[Variable or Value](../../../05-reference/variable-or-value/)

## **See Also**[¶](#see-also "Permanent link")

*   [Easing Function Editor](../../../04-editor/easing-function-editor/)