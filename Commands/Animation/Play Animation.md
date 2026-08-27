# Play Animation

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/00-play-animation/*

---

# Play Animation

## **Play Animation**[¶](#play-animation "Permanent link")

Plays a database animation on the screen or on a specific actor.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animation

The index of the animation to play from the database.

[Variable or Value](../../../05-reference/variable-or-value/)

Result

The variable to store the animation unique ID in.

[Variable or Value](../../../05-reference/variable-or-value/)

Store ID

Whether to store the resulting animation unique ID in a variable.

Toggle

Target

The actor to play the animation on.

[Actor Reference](../../../05-reference/actor-reference/)

Use as Screen Animation

Whether to play the animation on the screen instead of targeting an actor.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Play Animation on the Screen**[¶](#play-animation-on-the-screen "Permanent link")

Plays database animation 3 as a screen animation.

Code ScriptVisual Script

`[](#__codelineno-0-1)$gv[0] = play_animation(3, screen);`

`[](#__codelineno-1-1){"Data":{"AnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsScreenAnimation":1,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.PlayAnimationCommand"}`

#### **Play Animation on a Specific Entity**[¶](#play-animation-on-a-specific-entity "Permanent link")

Plays database animation 3 on entity 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)play_animation(3, entity(0));`

`[](#__codelineno-3-1){"Data":{"AnimationIndex":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"3","VariableIndex":0,"Metadata":null},"IsScreenAnimation":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.PlayAnimationCommand"}`

#### **Play Animation on Self and Store the Unique Identifier**[¶](#play-animation-on-self-and-store-the-unique-identifier "Permanent link")

Plays database animation from global variable 1 on self and stores the unique ID in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-4-1)$gv[0] = play_animation($gv[1], self);`

`[](#__codelineno-5-1){"Data":{"AnimationIndex":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"IsScreenAnimation":0,"Result":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"StoreID":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.PlayAnimationCommand"}`