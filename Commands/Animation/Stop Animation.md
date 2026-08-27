# Stop Animation

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/02-stop-animation/*

---

# Stop Animation

## **Stop Animation**[¶](#stop-animation "Permanent link")

Stops and removes a running animation from the screen or an actor by its unique ID.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animation Unique ID

The unique ID of the animation to stop.

[Variable or Value](../../../05-reference/variable-or-value/)

Is Screen Animation

Whether the animation to stop is a screen animation instead of an actor animation.

Toggle

Target

The actor to stop the animation on.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Stop a Screen Animation by Unique Identifier**[¶](#stop-a-screen-animation-by-unique-identifier "Permanent link")

Stops the screen animation whose unique ID is stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)stop_animation($gv[0], screen);`

`[](#__codelineno-1-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsScreenAnimation":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.StopAnimationCommand"}`

#### **Stop an Animation on an Entity**[¶](#stop-an-animation-on-an-entity "Permanent link")

Stops the animation on entity 0 whose unique ID is stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)stop_animation($gv[0], entity(0));`

`[](#__codelineno-3-1){"Data":{"ID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsScreenAnimation":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.StopAnimationCommand"}`