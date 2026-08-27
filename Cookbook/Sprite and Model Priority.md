# Sprite and Model Priority

*Источник: https://docs.rpg-architect.com/03-cookbook/02-sprite-and-model-priority/*

---

# Sprite and Model Priority

## **Sprite and Model Priority**[¶](#sprite-and-model-priority "Permanent link")

Many things can alter or change a character's sprite or model in the engine. The priority is as follows:

1.  The character's defined , specified by the [Character](../../06-database/00-characters/00-characters/).
2.  The class sprite or model, specified in any [Class](../../06-database/00-characters/01-classes/).
3.  The equipment's sprite or model, specified in any [Equipment](../../06-database/02-items/02-equipment/).

> **Example**: Suppose a character, Henry, has a **Sprite / Model** specified and then equips some iron armor that also has a **Sprite / Model** defined for it. The hero will now be shown with the iron armor's **Sprite / Model**. If the armor is removed, the original **Sprite / Model** will now be displayed. Suppose Henry now has a class 'Wizard' applied and it has a **Sprite / Model** defined. Henry will now have the **Sprite / Model** as his visual. Further, assume that even with a class defined, Henry re-equips the iron armor -- the iron armor's **Sprite / Model** will now override the character and class **Sprite / Model**.
> 
> **Note**: If a [Change Character Model](../../07-commands/12-entity-and-vehicle/12-change-character-model/) command is used, it is only temporary. If the character changes classes, equipment, or anything else listed in the priority above, the character will have priority reset. This is by design.