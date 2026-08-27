# Change Battler Position

*Источник: https://docs.rpg-architect.com/07-commands/14-battle/150-change-battler-position/*

---

# Change Battler Position

## **Change Battler Position**[¶](#change-battler-position "Permanent link")

Updates the position of a battler in the battle scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Battler Unique ID

The unique ID of the battler whose position will be changed.

[Variable or Value](../../../05-reference/variable-or-value/)

X

The X coordinate to set for the battler's position.

[Variable or Value](../../../05-reference/variable-or-value/)

X Enabled

When enabled, the X coordinate of the battler will be updated.

Toggle

Y

The Y coordinate to set for the battler's position.

[Variable or Value](../../../05-reference/variable-or-value/)

Y Enabled

When enabled, the Y coordinate of the battler will be updated.

Toggle

Z

The Z coordinate to set for the battler's position.

[Variable or Value](../../../05-reference/variable-or-value/)

Z Enabled

When enabled, the Z coordinate of the battler will be updated.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Change the X Position of a Battler**[¶](#change-the-x-position-of-a-battler "Permanent link")

This sets the X coordinate of the battler identified by Global Variable 0 to 5.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_battler_position($gv[0], x: 5);`

`[](#__codelineno-1-1){"Data":{"BattlerUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsXEnabled":1,"IsYEnabled":0,"IsZEnabled":0,"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattlerPositionCommand"}`

#### **Change All Position Coordinates of a Battler**[¶](#change-all-position-coordinates-of-a-battler "Permanent link")

This sets the X, Y, and Z coordinates of the specified battler to new positions.

Code ScriptVisual Script

`[](#__codelineno-2-1)change_battler_position($gv[0], x: 10, y: 2, z: 5);`

`[](#__codelineno-3-1){"Data":{"BattlerUniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"IsXEnabled":1,"IsYEnabled":1,"IsZEnabled":1,"X":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"10","VariableIndex":0,"Metadata":null},"Y":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"2","VariableIndex":0,"Metadata":null},"Z":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"5","VariableIndex":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Battle.ChangeBattlerPositionCommand"}`