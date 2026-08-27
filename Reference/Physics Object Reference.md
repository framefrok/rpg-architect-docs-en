# Physics Object Reference

*Источник: https://docs.rpg-architect.com/05-reference/physics-object-reference/*

---

# Physics Object Reference

## **Physics Object Reference**[¶](#physics-object-reference "Permanent link")

RPG Architect enables access to physics objects through multiple methods, extending the [Actor Reference](../actor-reference/) system. Physics objects include entities, doodads, vehicles, and heroes.

*   **Party** — Access an active party member by index (0 for first, 1 for second, etc.).
*   **Entity** — Access an entity in the current scene by its ID.
*   **Doodad** — Access a doodad in the current scene by its placement order.
*   **Self** — Access the entity currently being scripted. No additional parameters needed.
*   **By Unique ID** — Access any physics-interactive object by its saved [Unique ID](../unique-id/). Every physics object in the engine has a Unique ID that can be stored in a [Variable](../variable/) for later reference.