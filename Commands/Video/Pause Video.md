# Pause Video

*Источник: https://docs.rpg-architect.com/07-commands/18-video/01-pause-video/*

---

# Pause Video

## **Pause Video**[¶](#pause-video "Permanent link")

Pauses a currently playing video by ID, or all videos at once.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Apply to All

Whether to pause all active videos instead of a specific one.

Toggle

ID

The ID of the video to use.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Pause a Specific Video**[¶](#pause-a-specific-video "Permanent link")

Pauses the video with the specified ID stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-0-1)pause_video($gv[0]);`

`[](#__codelineno-1-1){"Data":{"IsAll":0,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.PauseVideoCommand"}`

#### **Pause All Videos**[¶](#pause-all-videos "Permanent link")

Pauses all currently playing videos at once.

Code ScriptVisual Script

`[](#__codelineno-2-1)pause_video(all);`

`[](#__codelineno-3-1){"Data":{"IsAll":1,"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.PauseVideoCommand"}`