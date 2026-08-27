# Change Character Model

*Источник: https://docs.rpg-architect.com/07-commands/12-entity-and-vehicle/12-change-character-model/*

---

# Change Character Model

## **Change Character Model**[¶](#change-character-model "Permanent link")

Changes the character model of an actor to a different sprite or model.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Character Model

The sprite or model to use as the character model for the target actor.

[Sprite or Model](../../../05-reference/sprite-or-model/)

Target

The actor whose character model will be changed.

[Actor Reference](../../../05-reference/actor-reference/)

## **Examples**[¶](#examples "Permanent link")

#### **Change Entity 0 Character Model**[¶](#change-entity-0-character-model "Permanent link")

This changes the character model of entity 0 to the specified model file.

Code ScriptVisual Script

`[](#__codelineno-0-1)change_character_model(entity(0), "Characters/Hero.gltf");`

`[](#__codelineno-1-1){"Data":{"CharacterModel":{"Animation":null,"BackfaceCullingMethod":0,"HueShift":0,"IsCycling":0,"IsModel":0,"Name":"Characters/Hero.gltf","SpriteBorderThickness":0,"SpriteDuration":100,"SpriteFrames":3,"SpriteLayers":{},"SpriteOrientation":4,"SpriteOrientedAroundCenter":1,"SpriteRegion":"0,0,0,0","UseSpriteLayers":0,"Scale":"1,1,1","Translation":"0,0,0"},"Target":{"Identifier":{"IsGlobalVariable":false,"IsLocalVariable":false,"IsValue":true,"Value":"0","VariableIndex":0,"Metadata":null},"IsEntity":1,"IsIdentifiedByUniqueID":0,"IsPartyMember":0,"IsSelf":0,"Metadata":null},"Metadata":null},"TypeName":"MAR.Game.RPGCore.Models.Scripts.Commands.Entity.EntityChangeCharacterModelCommand"}`