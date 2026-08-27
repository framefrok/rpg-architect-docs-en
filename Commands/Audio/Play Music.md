# Play Music

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/01-play-music/*

---

# Play Music

## **Play Music**[¶](#play-music "Permanent link")

Begins playback of a music track, specified directly or constructed from variables for dynamic selection.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Asset Name

The audio asset file name when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

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

Whether the music loops continuously when using variable mode.

[Switch or Value](../../../05-reference/switch-or-value/)

Music

The music asset to play.

[Music](../../../05-reference/music/)

Offset (milliseconds)

The playback offset in milliseconds from which the music begins playing.

[Variable or Value](../../../05-reference/variable-or-value/)

Pan

The stereo panning value when using variable mode. Ranges from -1 (left) to 1 (right).

[Variable or Value](../../../05-reference/variable-or-value/)

Pitch

The pitch adjustment when using variable mode.

[Variable or Value](../../../05-reference/variable-or-value/)

Use Variable

When enabled, the music track is constructed from variable values instead of a direct asset reference.

Toggle

Volume

The playback volume when using variable mode. Ranges from 0 (silent) to 1 (full volume).

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Play a Music Track by Asset Reference**[¶](#play-a-music-track-by-asset-reference "Permanent link")

Plays a music track using a direct asset reference with default settings.

Code ScriptVisual Script

`[](#__codelineno-0-1)play_music({name: "Content/Audio/BattleTheme.ogg"});`

`[](#__codelineno-1-1){"Data":{"IsVariable":0,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Value":{"FadeIn":"00:00:00","IsLooping":1,"LoopLength":null,"LoopStart":null,"Name":"Content/Audio/BattleTheme.ogg","Pan":0,"Pitch":0,"Position":"00:00:00","Volume":1},"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayMusicCommand"}`

#### **Play a Music Track with Playback Offset**[¶](#play-a-music-track-with-playback-offset "Permanent link")

Plays a music track starting at 5000 milliseconds into the track.

Code ScriptVisual Script

`[](#__codelineno-2-1)play_music({name: "Content/Audio/BattleTheme.ogg"}, 5000);`

`[](#__codelineno-3-1){"Data":{"IsVariable":0,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5000","VariableIndex":0,"Metadata":null},"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"Value":{"FadeIn":"00:00:00","IsLooping":1,"LoopLength":null,"LoopStart":null,"Name":"Content/Audio/BattleTheme.ogg","Pan":0,"Pitch":0,"Position":"00:00:00","Volume":1},"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayMusicCommand"}`

#### **Play Music from Variables with Custom Settings**[¶](#play-music-from-variables-with-custom-settings "Permanent link")

Plays a music track constructed from variable values with a custom name, volume, and looping enabled.

Code ScriptVisual Script

`[](#__codelineno-4-1)play_music(name: $gv[0], volume: 0.8, is_looping: true);`

`[](#__codelineno-5-1){"Data":{"IsVariable":1,"Offset":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SwitchIsLooping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"Value":null,"VariableFadeIn":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableLoopLength":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableLoopStart":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableName":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"VariablePan":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariablePitch":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"VariableVolume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.8","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.PlayMusicCommand"}`