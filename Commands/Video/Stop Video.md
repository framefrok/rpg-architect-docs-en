# Stop Video

*Источник: https://docs.rpg-architect.com/07-commands/18-video/03-stop-video/*

---

# Stop Video

## **Stop Video**[¶](#stop-video "Permanent link")

Stops a currently playing video by ID, or all videos at once.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Apply to All

Whether to stop all active videos instead of a specific one.

Toggle

ID

The ID of the video to use.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Stop a Specific Video**[¶](#stop-a-specific-video "Permanent link")

Stops the video with the specified ID stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-0-1)stop_video($gv[0]);`

`[](#__codelineno-1-1){"Data":{"IsAll":0,"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.StopVideoCommand"}`

#### **Stop All Videos**[¶](#stop-all-videos "Permanent link")

Stops all currently playing videos at once.

Code ScriptVisual Script

`[](#__codelineno-2-1)stop_video(all);`

`[](#__codelineno-3-1){"Data":{"IsAll":1,"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Video.StopVideoCommand"}`