# Clear Pictures

*Источник: https://docs.rpg-architect.com/07-commands/17-picture/03-clear-pictures/*

---

# Clear Pictures

## **Clear Pictures**[¶](#clear-pictures "Permanent link")

Removes all displayed pictures from screen.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

ID

The ID of the picture to use.

[Variable or Value](../../../05-reference/variable-or-value/)

Include Persisted Pictures

Whether to also clear pictures that persist between scenes.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Clear All Non-Persistent Pictures**[¶](#clear-all-non-persistent-pictures "Permanent link")

This removes all currently displayed pictures from the screen, excluding those that persist between scenes.

Code ScriptVisual Script

`[](#__codelineno-0-1)clear_pictures();`

`[](#__codelineno-1-1){"Data":{"IncludeStatic":0,"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ClearPicturesCommand"}`

#### **Clear All Pictures Including Persistent Ones**[¶](#clear-all-pictures-including-persistent-ones "Permanent link")

This removes all currently displayed pictures from the screen, including those that persist between scenes.

Code ScriptVisual Script

`[](#__codelineno-2-1)clear_pictures(include_static);`

`[](#__codelineno-3-1){"Data":{"IncludeStatic":1,"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.ClearPicturesCommand"}`