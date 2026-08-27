# Add Annotations

*Источник: https://docs.rpg-architect.com/07-commands/09-animation/05-add-annotations/*

---

# Add Annotations

## **Add Annotations**[¶](#add-annotations "Permanent link")

Attaches one or more visual annotations to a target actor.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Annotations

The list of annotations to add to the target actor.

[Annotation](../../../05-reference/annotation/)

Target

The actor to add annotations to.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Add a Sprite Annotation to an Entity**[¶](#add-a-sprite-annotation-to-an-entity "Permanent link")

Attaches a sprite annotation using a custom image to entity 0.

Code ScriptVisual Script

`[](#__codelineno-0-1)add_annotations(entity(0), [sprite("Content/Images/Sprite.png")]);`

`[](#__codelineno-1-1){"Data":{"Annotations":[{"$":"SpriteAnnotation","Height":1,"IsSpriteCycling":0,"Sprite":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":"Content/Images/Sprite.png","SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":1,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"StretchToDimensions":0,"Width":1,"Color":"1,1,1,1","Effects":[],"IsRecycling":1,"Offset":"0,0,0","PixelOffset":"0,0","Metadata":null}],"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.AddAnnotationsCommand"}`

#### **Add a Text Annotation to Self**[¶](#add-a-text-annotation-to-self "Permanent link")

Attaches a text annotation displaying a message to the current entity.

Code ScriptVisual Script

`[](#__codelineno-2-1)add_annotations(self, [text("Hello")]);`

`[](#__codelineno-3-1){"Data":{"Annotations":[{"$":"TextAnnotation","Font":{"Color":"1,1,1,1","DropShadowOffset":"1,1","DropShadowColor":"0,0,0,0","Family":0,"HorizontalAlignment":0,"IsBold":0,"IsItalic":0,"IsStrikethrough":0,"IsUnderlined":0,"Name":null,"Size":12,"UseDropShadow":0,"VerticalAlignment":2,"Metadata":null},"Text":"Hello","Color":"1,1,1,1","Effects":[],"IsRecycling":1,"Offset":"0,0,0","PixelOffset":"0,0","Metadata":null}],"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"","VariableIndex":0,"Metadata":null},"IsEntity":0,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":1,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Animation.AddAnnotationsCommand"}`