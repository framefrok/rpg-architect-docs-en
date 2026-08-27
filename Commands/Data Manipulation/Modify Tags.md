# Modify Tags

*Источник: https://docs.rpg-architect.com/07-commands/01-data-manipulation/100-modify-tags/*

---

# Modify Tags

## **Modify Tags**[¶](#modify-tags "Permanent link")

Adds, changes, or removes [Tags](../../../05-reference/tags/) on an object identified by its [Unique ID](../../../05-reference/unique-id/).

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Add Key

The variable-based key for the tag to add or update.

[Variable or Value](../../../05-reference/variable-or-value/)

Add Value

The variable-based value for the tag to add or update.

[Variable or Value](../../../05-reference/variable-or-value/)

Changed Tags

The tags to add or update on the target object. Each tag is a key-value pair.

[Tags](../../../05-reference/tags/)

Provider

The type of object whose tags will be modified, such as battlers, items, or skill slots.

[Tag Context Provider](../../../05-reference/tag-context-provider/)

Remove Key

The variable-based key for the tag to remove.

[Variable or Value](../../../05-reference/variable-or-value/)

Removed Tags

The tags to remove from the target object. Each entry specifies a tag key to delete.

[Tags](../../../05-reference/tags/)

Unique ID

The unique identifier of the object whose tags will be modified.

[Variable or Value](../../../05-reference/variable-or-value/)

Use Variables

When enabled, tag keys and values are read from variables instead of being specified as fixed values.

Toggle

## **Examples**[¶](#examples "Permanent link")

#### **Add a Tag to a Battler**[¶](#add-a-tag-to-a-battler "Permanent link")

This adds the tag "state" with value "poisoned" to the battler identified by the Unique ID stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)modify_tags(battlers, $gv[0], add: ["state": "poisoned"]);`

`[](#__codelineno-1-1){"Data":{"ChangedTags":{"state":"poisoned"},"ContextProvider":{"$":"BattlerTagContextProvider","Metadata":null},"IsVariableBased":0,"RemovedTags":{},"UniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"VariableAddKey":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableAddValue":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"VariableRemoveKey":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ModifyTagsCommand"}`

#### **Add and Remove Tags Using Variables**[¶](#add-and-remove-tags-using-variables "Permanent link")

This adds a tag with a key from Global Variable 1 and value from Global Variable 2, and removes a tag with a key from Global Variable 3, on an item identified by the Unique ID stored in Global Variable 0.

Code ScriptVisual Script

`[](#__codelineno-2-1)modify_tags(items, $gv[0], add_variable: { $gv[1], $gv[2] }, remove: $gv[3]);`

`[](#__codelineno-3-1){"Data":{"ChangedTags":{},"ContextProvider":{"$":"ItemBaseContextProvider","Metadata":null},"IsVariableBased":1,"RemovedTags":{},"UniqueID":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":0,"Metadata":null},"VariableAddKey":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":1,"Metadata":null},"VariableAddValue":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":2,"Metadata":null},"VariableRemoveKey":{"IsGlobalVariable":true,"IsLocalVariable":false,"IsValue":false,"Value":"","VariableIndex":3,"Metadata":null},"Index":0,"IndexEnd":null,"IsGlobal":1,"IsLocal":0,"IsOperandReference":0,"IsReference":0,"OperandGlobalIndex":null,"OperandLocalIndex":null,"Metadata":null},"TypeName":"MAR.Game.Shared.Models.Scripts.Commands.Data.ModifyTagsCommand"}`