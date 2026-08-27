# Set Master Volume

*Источник: https://docs.rpg-architect.com/07-commands/03-audio/20-set-master-volume/*

---

# Set Master Volume

## **Set Master Volume**[¶](#set-master-volume "Permanent link")

Adjusts the master volume level for either music or sound effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Music

When selected, the volume adjustment applies to the master music volume.

Toggle

Volume

The volume level to set. Ranges from 0 (silent) to 1 (full volume).

[Variable or Value](../../../05-reference/variable-or-value/)

## **Examples**[¶](#examples "Permanent link")

#### **Set Master Music Volume to Half**[¶](#set-master-music-volume-to-half "Permanent link")

Sets the master music volume to 50 percent.

Code ScriptVisual Script

`[](#__codelineno-0-1)set_master_volume(0.5, music);`

`[](#__codelineno-1-1){"Data":{"IsMusic":1,"Volume":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0.5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.SetMasterVolumeCommand"}`

#### **Set Master Sound Effect Volume from a Variable**[¶](#set-master-sound-effect-volume-from-a-variable "Permanent link")

Sets the master sound effect volume using a value stored in a global variable.

Code ScriptVisual Script

`[](#__codelineno-2-1)set_master_volume($gv[0], sfx);`

`[](#__codelineno-3-1){"Data":{"IsMusic":0,"Volume":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Audio.SetMasterVolumeCommand"}`