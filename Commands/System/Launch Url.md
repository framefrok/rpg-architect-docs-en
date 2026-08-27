# Launch Url

*Источник: https://docs.rpg-architect.com/07-commands/20-system/201-launch-url/*

---

# Launch Url

## **Launch Url**[¶](#launch-url "Permanent link")

Opens a web address in the player's default browser.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

URL

The web address to open in the player's default browser.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Open a Website**[¶](#open-a-website "Permanent link")

Opens a specific web address in the player's default browser.

Code ScriptVisual Script

`[](#__codelineno-0-1)launch_url("https://www.example.com");`

`[](#__codelineno-1-1){"Data":{"Url":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"https://www.example.com","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.LaunchUrlCommand"}`

#### **Open a URL from a Variable**[¶](#open-a-url-from-a-variable "Permanent link")

Opens the web address stored in global variable 0 in the player's default browser.

Code ScriptVisual Script

`[](#__codelineno-2-1)launch_url($gv[0]);`

`[](#__codelineno-3-1){"Data":{"Url":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.System.LaunchUrlCommand"}`