# Stop Background Effect

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/11-stop-background-effect/*

---

# Stop Background Effect

## **Stop Background Effect**[¶](#stop-background-effect "Permanent link")

Stops all active background effects or a specific one identified by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Fade-Out (milliseconds)

The duration in milliseconds over which the background effect fades out before stopping.

[Variable or Value](../../../05-reference/variable-or-value/)

Stop All

When enabled, all active background effects are stopped.

Toggle

Unique ID

The unique ID of the specific background effect instance to stop.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Stop All Background Effects**[¶](#stop-all-background-effects "Permanent link")

Stops all currently active background sound effects.

Code ScriptVisual Script

`[](#__codelineno-0-1)stop_bgfx();`

`[](#__codelineno-1-1){"Data":{"IsAll":1,"Value":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.StopBackgroundEffectCommand"}`

#### **Stop a Specific Background Effect by Unique ID**[¶](#stop-a-specific-background-effect-by-unique-id "Permanent link")

Stops a single background effect identified by a unique ID stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-2-1)stop_bgfx($gv[0]);`

`[](#__codelineno-3-1){"Data":{"IsAll":0,"Value":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.StopBackgroundEffectCommand"}`