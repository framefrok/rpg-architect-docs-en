# Play Sound Effect

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/00-play-sound-effect/*

---

# Play Sound Effect

## **Play Sound Effect**[¶](#play-sound-effect "Permanent link")

Plays a one-shot sound effect, specified directly or constructed from variables for dynamic audio.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Asset Name

The audio asset file name when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Pan

The stereo panning value when using variable mode. Ranges from -1 (left) to 1 (right).

[Variable or Value](../../../05-reference/variable-or-value/)

Pitch

The pitch adjustment when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Sound Effect

The sound effect asset to play.

[Sound Effect](../../../05-reference/sound-effect/)

Use Variable

When enabled, the sound effect is constructed from variable values instead of a direct asset reference.

Toggle

Volume

The playback volume when using variable mode. Ranges from 0 (silent) to 1 (full volume).

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Play a Sound Effect by Asset Reference**[¶](#play-a-sound-effect-by-asset-reference "Permanent link")

Plays a sound effect using a direct asset reference with default settings.

Code ScriptVisual Script

`[](#__codelineno-0-1)play_sfx({name: "Content/Audio/Hit.ogg"});`

`[](#__codelineno-1-1){"Data":{"IsVariable":0,"Value":{"IsPreventingMultiple":0,"Name":"Content/Audio/Hit.ogg","Pan":0,"Pitch":0,"Volume":1},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.SoundEffectCommand"}`

#### **Play a Sound Effect with Custom Volume and Pitch**[¶](#play-a-sound-effect-with-custom-volume-and-pitch "Permanent link")

Plays a sound effect at 80 percent volume with a pitch shift applied.

Code ScriptVisual Script

`[](#__codelineno-2-1)play_sfx({name: "Content/Audio/Hit.ogg", volume: 0.8, pitch: 0.5});`

`[](#__codelineno-3-1){"Data":{"IsVariable":0,"Value":{"IsPreventingMultiple":0,"Name":"Content/Audio/Hit.ogg","Pan":0,"Pitch":0.5,"Volume":0.8},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.SoundEffectCommand"}`

#### **Play a Sound Effect from Variables**[¶](#play-a-sound-effect-from-variables "Permanent link")

Plays a sound effect constructed from variable values with a custom name and volume.

Code ScriptVisual Script

`[](#__codelineno-4-1)play_sfx(name: $gv[0], volume: 0.5);`

`[](#__codelineno-5-1){"Data":{"IsVariable":1,"Value":{"IsPreventingMultiple":0,"Name":null,"Pan":0,"Pitch":0,"Volume":1},"VariableName":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.SoundEffectCommand"}`