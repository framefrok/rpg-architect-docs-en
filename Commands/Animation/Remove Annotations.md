# Remove Annotations

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/06-remove-annotations/*

---

# Remove Annotations

## **Remove Annotations**[¶](#remove-annotations "Permanent link")

Removes visual annotations from a specific actor or all entities.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

All Entities

Whether to remove annotations from all entities on the map.

Toggle

By Tag

Whether to only remove annotations that match a specific tag.

Toggle

Include Script-Page Annotations

Whether to also remove annotations that were added by a script page.

Toggle

Tag

The tag to match when removing annotations by tag.

[Variable or Value](../../../05-reference/variable-or-value/)

Target

The actor to remove annotations from.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Remove All Annotations from an Entity**[¶](#remove-all-annotations-from-an-entity "Permanent link")

Removes all visual annotations from entity 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)remove_annotations(entity(0));`

`[](#__codelineno-1-1){"Data":{"IsAllEntities":0,"IsByTag":0,"IncludeScriptAnnotations":0,"Tag":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.RemoveAnnotationsCommand"}`

#### **Remove All Annotations from All Entities**[¶](#remove-all-annotations-from-all-entities "Permanent link")

Removes all visual annotations from every entity on the map.

Code ScriptVisual Script

`[](#__codelineno-2-1)remove_annotations(all);`

`[](#__codelineno-3-1){"Data":{"IsAllEntities":1,"IsByTag":0,"IncludeScriptAnnotations":0,"Tag":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.RemoveAnnotationsCommand"}`

#### **Remove Annotations by Tag Including Script Annotations**[¶](#remove-annotations-by-tag-including-script-annotations "Permanent link")

Removes annotations matching a specific tag from all entities, including those added by script pages.

Code ScriptVisual Script

`[](#__codelineno-4-1)remove_annotations(all, tag: "my_tag", include_script);`

`[](#__codelineno-5-1){"Data":{"IsAllEntities":1,"IsByTag":1,"IncludeScriptAnnotations":1,"Tag":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"my_tag","VariableIndex":0,"Metadata":null},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.RemoveAnnotationsCommand"}`