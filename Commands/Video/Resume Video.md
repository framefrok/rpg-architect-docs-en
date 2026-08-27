# Resume Video

*Источник: https://docs.rpg-architect.com/07-commands/18-video/02-resume-video/*

---

# Resume Video

## **Resume Video**[¶](#resume-video "Permanent link")

Resumes a paused video by ID, or all videos at once.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Apply to All

Whether to resume all paused videos instead of a specific one.

Toggle

ID

The ID of the video to use.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Resume a Specific Video**[¶](#resume-a-specific-video "Permanent link")

Resumes the paused video with the specified ID stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-0-1)resume_video($gv[0]);`

`[](#__codelineno-1-1){"Data":{"IsAll":0,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.ResumeVideoCommand"}`

#### **Resume All Videos**[¶](#resume-all-videos "Permanent link")

Resumes all paused videos at once.

Code ScriptVisual Script

`[](#__codelineno-2-1)resume_video(all);`

`[](#__codelineno-3-1){"Data":{"IsAll":1,"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.ResumeVideoCommand"}`