# Comment

*Источник: https://docs.rpg-architect.com/07-commands/15-control-flow/100-comment/*

---

# Comment

## **Comment**[¶](#comment "Permanent link")

Allows notes or documentation to be added within a script for organizational purposes.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Comment

The comment text to display within the script for documentation or note-taking purposes.

String

## **Examples**[¶](#examples "Permanent link")

#### **Add a Single Line Comment**[¶](#add-a-single-line-comment "Permanent link")

This adds a comment to the script for documentation purposes. Comments are ignored during execution.

Code ScriptVisual Script

`[](#__codelineno-0-1)// This is a comment`

`[](#__codelineno-1-1){"Data":{"Comment":"This is a comment","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.CommentCommand"}`

#### **Add a Multi-Line Comment**[¶](#add-a-multi-line-comment "Permanent link")

This adds a multi-line comment spanning two lines. Each line is prefixed with the comment marker.

Code ScriptVisual Script

`[](#__codelineno-2-1)// First line of the comment [](#__codelineno-2-2)// Second line of the comment`

`[](#__codelineno-3-1){"Data":{"Comment":"First line of the comment\r\nSecond line of the comment","Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Flow.CommentCommand"}`