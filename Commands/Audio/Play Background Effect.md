# Play Background Effect

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/10-play-background-effect/*

---

# Play Background Effect

## **Play Background Effect**[¶](#play-background-effect "Permanent link")

Plays a looping or one-shot background sound effect that persists across scenes until stopped.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Asset Name

The audio asset file name when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Background Effect

The background sound effect asset to play.

[Sound Effect](../../../05-reference/sound-effect/)

Fade In

The fade-in duration in milliseconds when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Loop Length

The loop length in milliseconds when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Loop Start

The loop start position in milliseconds when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Looping

Whether the background effect loops continuously when using variable mode.

[Switch or Value](../../../05-reference/switch-or-value/)

Offset (milliseconds)

The playback offset in milliseconds from which the background effect begins playing.

[Variable or Value](../../../05-reference/variable-or-value/)

Pan

The stereo panning value when using variable mode. Ranges from -1 (left) to 1 (right).

[Variable or Value](../../../05-reference/variable-or-value/)

Pitch

The pitch adjustment when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the background effect's unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Store ID

Whether to store the unique ID of the background effect instance in a variable for later reference.

Toggle

Use Variable

When enabled, the background effect is constructed from variable values instead of a direct asset reference.

Toggle

Volume

The playback volume when using variable mode. Ranges from 0 (silent) to 1 (full volume).

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Play a Background Effect by Asset Reference**[¶](#play-a-background-effect-by-asset-reference "Permanent link")

Plays a looping background sound effect using a direct asset reference.

Code ScriptVisual Script

`[](#__codelineno-0-1)play_bgfx({name: "Content/Audio/Rain.ogg"});`

`[](#__codelineno-1-1){"Data":{"IsVariable":0,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Value":{"IsPreventingMultiple":0,"Name":"Content/Audio/Rain.ogg","Pan":0,"Pitch":0,"Volume":1},"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayBackgroundEffectCommand"}`

#### **Play a Background Effect and Store Its Unique ID**[¶](#play-a-background-effect-and-store-its-unique-id "Permanent link")

Plays a background sound effect and stores its unique ID in global variable 0 for later reference.

Code ScriptVisual Script

`[](#__codelineno-2-1)$gv[0] = play_bgfx({name: "Content/Audio/Rain.ogg"});`

`[](#__codelineno-3-1){"Data":{"IsVariable":0,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":1,"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Value":{"IsPreventingMultiple":0,"Name":"Content/Audio/Rain.ogg","Pan":0,"Pitch":0,"Volume":1},"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayBackgroundEffectCommand"}`

#### **Play a Background Effect from Variables**[¶](#play-a-background-effect-from-variables "Permanent link")

Plays a background sound effect constructed from variable values with a fade-in and looping enabled.

Code ScriptVisual Script

`[](#__codelineno-4-1)play_bgfx(name: $gv[0], fade_in: 2000, is_looping: true);`

`[](#__codelineno-5-1){"Data":{"IsVariable":1,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Value":{"IsPreventingMultiple":0,"Name":null,"Pan":0,"Pitch":0,"Volume":1},"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2000","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayBackgroundEffectCommand"}`