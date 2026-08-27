# Actor Reference

*Источник: https://docs.rpg-architect.com/05-reference/actor-reference/*

---

# Actor Reference

## **Actor Reference**[¶](#actor-reference "Permanent link")

RPG Architect supports accessing actors (entities, vehicles, heroes, and more) in a multitude of ways, largely based on the [Variable or Value](../variable-or-value/) construct.

*   **Party** is used to access a member of the active party. The first party member would be accessed by 0, the second by 1, and so forth.
*   **Entity** is used to access an entity in a scene, if valid. The value corresponds to the entity ID.
*   **Self** is used to access the entity that is currently being scripted. No further parameters are needed.
*   **By Unique ID** is a powerful construct that allows you to save the unique ID of an entity, vehicle, hero, and so forth -- and then access it. Every physics-interactive object in the engine has a Unique ID.