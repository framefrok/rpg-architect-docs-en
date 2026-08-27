# Alter Physics Properties

*Источник: https://docs.rpg-architect.com/07-commands/10-physics/01-alter-physics-properties/*

---

# Alter Physics Properties

## **Alter Physics Properties**[¶](#alter-physics-properties "Permanent link")

Modifies the physical properties of a physics object, including speed, size, gravity multiplier, and collision behavior.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Gravity Multiplier X

The X component of the gravity multiplier applied to the physics object.

[Variable or Value](../../../05-reference/variable-or-value/)

Gravity Multiplier X Enabled

Enables or disables the gravity multiplier X component for this command.

Toggle

Gravity Multiplier Y

The Y component of the gravity multiplier applied to the physics object.

[Variable or Value](../../../05-reference/variable-or-value/)

Gravity Multiplier Y Enabled

Enables or disables the gravity multiplier Y component for this command.

Toggle

Gravity Multiplier Z

The Z component of the gravity multiplier applied to the physics object.

[Variable or Value](../../../05-reference/variable-or-value/)

Gravity Multiplier Z Enabled

Enables or disables the gravity multiplier Z component for this command.

Toggle

Ignore Entity Collision

When enabled, the physics object will not collide with other entities.

[Switch or Value](../../../05-reference/switch-or-value/)

Ignore Entity Collision Enabled

Enables or disables the ignore entity collision property for this command.

Toggle

Ignore Obstacles

When enabled, the physics object will ignore collisions from terrain tags or tile collisions.

[Switch or Value](../../../05-reference/switch-or-value/)

Ignore Obstacles Enabled

Enables or disables the ignore obstacles property for this command.

Toggle

Ignores Gravity

When enabled, the physics object will not be affected by gravity.

[Switch or Value](../../../05-reference/switch-or-value/)

Ignores Gravity Enabled

Enables or disables the ignores gravity property for this command.

Toggle

Is Clipping

When enabled, the physics object will clip through other objects.

[Switch or Value](../../../05-reference/switch-or-value/)

Is Clipping Enabled

Enables or disables the clipping property for this command.

Toggle

Is Static

When enabled, the physics object becomes a static body that does not move.

[Switch or Value](../../../05-reference/switch-or-value/)

Is Static Enabled

Enables or disables the static body property for this command.

Toggle

Size X

The X component of the physics object's size.

[Variable or Value](../../../05-reference/variable-or-value/)

Size X Enabled

Enables or disables the size X component for this command.

Toggle

Size Y

The Y component of the physics object's size.

[Variable or Value](../../../05-reference/variable-or-value/)

Size Y Enabled

Enables or disables the size Y component for this command.

Toggle

Size Z

The Z component of the physics object's size.

[Variable or Value](../../../05-reference/variable-or-value/)

Size Z Enabled

Enables or disables the size Z component for this command.

Toggle

Speed X

The X component of the physics object's speed.

[Variable or Value](../../../05-reference/variable-or-value/)

Speed X Enabled

Enables or disables the speed X component for this command.

Toggle

Speed Y

The Y component of the physics object's speed.

[Variable or Value](../../../05-reference/variable-or-value/)

Speed Y Enabled

Enables or disables the speed Y component for this command.

Toggle

Speed Z

The Z component of the physics object's speed.

[Variable or Value](../../../05-reference/variable-or-value/)

Speed Z Enabled

Enables or disables the speed Z component for this command.

Toggle

Target

The physics object to target with this command.

[Physics Object Reference](../../../05-reference/physics-object-reference/)

Use As Delta Values

When enabled, the specified values are added to the current values. When disabled, the specified values replace the current values.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Change Entity Speed as Delta**[¶](#change-entity-speed-as-delta "Permanent link")

Increases the X speed of entity 0 by the value stored in global variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)alter_physics_properties(entity(0), speed_x: $gv[0]);`

`[](#__codelineno-1-1){"Data":{"GravityMultiplierX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IgnoreCollisions":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IgnoreGravity":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IgnoreObstacles":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsClipping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsIgnoreCollisionsEnabled":0,"IsIgnoreGravityEnabled":0,"IsIgnoreObstaclesEnabled":0,"IsClippingEnabled":0,"IsGravityMultiplierXEnabled":0,"IsGravityMultiplierYEnabled":0,"IsGravityMultiplierZEnabled":0,"IsSizeXEnabled":0,"IsSizeYEnabled":0,"IsSizeZEnabled":0,"IsSpeedXEnabled":1,"IsSpeedYEnabled":0,"IsSpeedZEnabled":0,"IsStaticEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SizeX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SizeY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SizeZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedX":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SpeedY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterPhysicsPropertiesCommand"}`

#### **Disable Gravity on an Entity**[¶](#disable-gravity-on-an-entity "Permanent link")

Makes entity 0 ignore gravity.

Code ScriptVisual Script

`[](#__codelineno-2-1)alter_physics_properties(entity(0), ignore_gravity: true);`

`[](#__codelineno-3-1){"Data":{"GravityMultiplierX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IgnoreCollisions":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IgnoreGravity":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":true,"SwitchIndex":0,"Metadata":null},"IgnoreObstacles":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsClipping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsDeltaOperation":1,"IsIgnoreCollisionsEnabled":0,"IsIgnoreGravityEnabled":1,"IsIgnoreObstaclesEnabled":0,"IsClippingEnabled":0,"IsGravityMultiplierXEnabled":0,"IsGravityMultiplierYEnabled":0,"IsGravityMultiplierZEnabled":0,"IsSizeXEnabled":0,"IsSizeYEnabled":0,"IsSizeZEnabled":0,"IsSpeedXEnabled":0,"IsSpeedYEnabled":0,"IsSpeedZEnabled":0,"IsStaticEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SizeX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SizeY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SizeZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterPhysicsPropertiesCommand"}`

#### **Set Entity Size Absolutely**[¶](#set-entity-size-absolutely "Permanent link")

Sets the size of entity 0 to exact values rather than adding to the current size, using the set flag.

Code ScriptVisual Script

`[](#__codelineno-4-1)alter_physics_properties(entity(0), size_x: $gv[0], size_y: $gv[1], set);`

`[](#__codelineno-5-1){"Data":{"GravityMultiplierX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"GravityMultiplierZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"1","VariableIndex":0,"Metadata":null},"IgnoreCollisions":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IgnoreGravity":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IgnoreObstacles":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsClipping":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"IsDeltaOperation":0,"IsIgnoreCollisionsEnabled":0,"IsIgnoreGravityEnabled":0,"IsIgnoreObstaclesEnabled":0,"IsClippingEnabled":0,"IsGravityMultiplierXEnabled":0,"IsGravityMultiplierYEnabled":0,"IsGravityMultiplierZEnabled":0,"IsSizeXEnabled":1,"IsSizeYEnabled":1,"IsSizeZEnabled":0,"IsSpeedXEnabled":0,"IsSpeedYEnabled":0,"IsSpeedZEnabled":0,"IsStaticEnabled":0,"IsStatic":{"IsGlobalSwitch":false,"IsLocalSwitch":false,"IsValue":true,"Value":false,"SwitchIndex":0,"Metadata":null},"SizeX":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"SizeY":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"SizeZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedX":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedY":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"SpeedZ":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Target":{"IsDoodad":0,"IsDoodadOrEntity":1,"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Physics.AlterPhysicsPropertiesCommand"}`