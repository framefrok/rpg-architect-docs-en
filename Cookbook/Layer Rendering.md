# Layer Rendering

*Источник: https://docs.rpg-architect.com/03-cookbook/04-2d-cookbook/layer-rendering/*

---

# Layer Rendering

## **Layer Rendering**[¶](#layer-rendering "Permanent link")

RPG Architect has no limit on the number of map layers that can be rendered. In order to get the best results, it is highly recommended that you understand how layering works.

First and foremost, the **Camera Distance** indicates the number of units (re: Height) that will be displayed above the camera's current focal point.

> **Example**: If the **Camera Distance** is set at 10 and the Hero's feet are at Height 2, the engine will render up to Height 12.

Further, non-tiles (**Entities** and **Doodads**) will always render as the "last" item on any layer between whole numbers.

> **Example**: If a character is at a height of 2.4, they will render as the "last" item between 2 and 3. If another tile layer is displayed at 2.9, the character will still be drawn "above" it.

This allows for complex tile layers to be built using a "floor" tile and then other tiles that render slightly above the floor, for floating platforms high in the sky, for tall structures built with structure tiles, and so on.