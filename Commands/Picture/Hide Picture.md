# Hide Picture

*Источник: https://docs.rpg-architect.com/07-commands/17-picture/02-hide-picture/*

---

# Hide Picture

## **Hide Picture**[¶](#hide-picture "Permanent link")

Removes a displayed picture from screen by its ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

ID

The ID of the picture to use.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Hide a Picture by Literal Identifier**[¶](#hide-a-picture-by-literal-identifier "Permanent link")

This removes the picture with ID 1 from the screen.

Code ScriptVisual Script

`[](#__codelineno-0-1)hide_picture(1);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.HidePictureCommand"}`

#### **Hide a Picture Using a Variable Reference**[¶](#hide-a-picture-using-a-variable-reference "Permanent link")

This removes the picture whose ID is stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)hide_picture($gv[0]);`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Picture.HidePictureCommand"}`