# Set Camera Type

*Источник: https://docs.rpg-architect.com/07-commands/11-map/105-set-camera-type/*

---

# Set Camera Type

## **Set Camera Type**[¶](#set-camera-type "Permanent link")

Changes the camera mode between 2D and 3D, and select the projection type for 3D cameras.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

2D

Whether the camera uses 2D mode.

Toggle

3D

Whether the camera uses 3D mode.

Toggle

First Person Mode

Whether the camera uses first person perspective in 3D mode.

Toggle

Orthographic Projection

Whether the camera uses orthographic projection in 3D mode.

Toggle

Perspective Projection

Whether the camera uses perspective projection in 3D mode.

Toggle

Reset to Default

Whether to reset the camera type to its default configuration.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Switch to 2D Camera Mode**[¶](#switch-to-2d-camera-mode "Permanent link")

This sets the camera to 2D mode.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_camera_type(2d);`

`[](#__codelineno-1-1){"Data":{"Is2D":1,"Is3D":0,"IsFirstPerson":0,"IsOrthographic":1,"IsPerspective":0,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraTypeCommand"}`

#### **Switch to 3D Camera with Perspective Projection**[¶](#switch-to-3d-camera-with-perspective-projection "Permanent link")

This sets the camera to 3D mode with perspective projection.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_camera_type(3d, perspective);`

`[](#__codelineno-3-1){"Data":{"Is2D":0,"Is3D":1,"IsFirstPerson":0,"IsOrthographic":0,"IsPerspective":1,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraTypeCommand"}`

#### **Switch to 3D Camera with First Person Mode**[¶](#switch-to-3d-camera-with-first-person-mode "Permanent link")

This sets the camera to 3D mode with first person perspective.

Code ScriptVisual Script

`[](#__codelineno-4-1)set_camera_type(3d, first_person);`

`[](#__codelineno-5-1){"Data":{"Is2D":0,"Is3D":1,"IsFirstPerson":1,"IsOrthographic":0,"IsPerspective":0,"IsReset":0,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraTypeCommand"}`

#### **Reset Camera Type to Default**[¶](#reset-camera-type-to-default "Permanent link")

This resets the camera type to its default configuration.

Code ScriptVisual Script

`[](#__codelineno-6-1)set_camera_type(reset);`

`[](#__codelineno-7-1){"Data":{"Is2D":0,"Is3D":1,"IsFirstPerson":0,"IsOrthographic":1,"IsPerspective":0,"IsReset":1,"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Map.MapCameraTypeCommand"}`