# Stop Music

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/03-stop-music/*

---

# Stop Music

## **Stop Music**[¶](#stop-music "Permanent link")

Stops the currently playing music track with an optional fade-out duration.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Fade-Out (milliseconds)

The duration in milliseconds over which the music fades out before stopping.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Stop Music Immediately**[¶](#stop-music-immediately "Permanent link")

Stops the currently playing music track without any fade-out.

Code ScriptVisual Script

`[](#__codelineno-0-1)stop_music();`

`[](#__codelineno-1-1){"Data":{"FadeOutDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.StopMusicCommand"}`

#### **Stop Music with a Fade-Out Duration**[¶](#stop-music-with-a-fade-out-duration "Permanent link")

Stops the currently playing music with a 500 millisecond fade-out.

Code ScriptVisual Script

`[](#__codelineno-2-1)stop_music(500);`

`[](#__codelineno-3-1){"Data":{"FadeOutDuration":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"500","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.StopMusicCommand"}`

#### **Stop Music with a Variable Fade-Out Duration**[¶](#stop-music-with-a-variable-fade-out-duration "Permanent link")

Stops the currently playing music with a fade-out duration stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-4-1)stop_music($gv[0]);`

`[](#__codelineno-5-1){"Data":{"FadeOutDuration":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.StopMusicCommand"}`