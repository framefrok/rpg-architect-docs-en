# Set Camera Target

*Источник: https://docs.rpg-architect.com/07-commands/11-map/110-set-camera-target/*

---

# Set Camera Target

## **Set Camera Target**[¶](#set-camera-target "Permanent link")

Changes what the camera follows, such as an actor, a fixed coordinate, or the default party target.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Fix Position to Coordinate

Whether the camera is locked to a fixed coordinate position.

Toggle

Follow Actor

Whether the camera follows a specific actor.

Toggle

Reset Target

Whether to reset the camera target to the default party member.

Toggle

Target

The actor for the camera to follow.

[Actor Reference](../../../05-reference/actor-reference/)

X

The X coordinate for the fixed camera position.

[Variable or Value](../../../05-reference/variable-or-value/)

Y

The Y coordinate for the fixed camera position.

[Variable or Value](../../../05-reference/variable-or-value/)

Z

The Z coordinate for the fixed camera position.

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Camera to Follow Entity 0**[¶](#set-camera-to-follow-entity-0 "Permanent link")

This sets the camera to follow the actor referenced by entity index 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_camera_target(entity(0));`

`[](#__codelineno-1-1){"Data":{"IsFixedPositionTarget":0,"IsResetTarget":0,"IsTargetingActorReference":1,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraSetTargetCommand"}`

#### **Set Camera to a Fixed Position**[¶](#set-camera-to-a-fixed-position "Permanent link")

This locks the camera to a fixed coordinate position at (5, 0, 10).

Code ScriptVisual Script

`[](#__codelineno-2-1)set_camera_target(5, 0, 10);`

`[](#__codelineno-3-1){"Data":{"IsFixedPositionTarget":1,"IsResetTarget":0,"IsTargetingActorReference":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraSetTargetCommand"}`

#### **Reset Camera Target to Default Party Member**[¶](#reset-camera-target-to-default-party-member "Permanent link")

This resets the camera target back to the default, following the lead party member.

Code ScriptVisual Script

`[](#__codelineno-4-1)set_camera_target(reset);`

`[](#__codelineno-5-1){"Data":{"IsFixedPositionTarget":0,"IsResetTarget":1,"IsTargetingActorReference":0,"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraSetTargetCommand"}`