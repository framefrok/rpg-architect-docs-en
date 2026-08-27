# Pixel Perfect Rendering

*Источник: https://docs.rpg-architect.com/03-cookbook/04-2d-cookbook/pixel-perfect-rendering/*

---

# Pixel Perfect Rendering

## **Pixel Perfect Rendering**[¶](#pixel-perfect-rendering "Permanent link")

RPG Architect's engine runs natively in 3D, and can transpose views and visuals into 2D. Occasionally, some 3D rendering issues show due to rounding errors. When a rounding error occurs, a pixel is grabbed adjacent to the pixel that should render.

To avoid this, we can leverage a simple formula to make sure everything renders perfectly each time:

> **(Camera Distance x Scale) / 2**

These are configured under **Video Configuration \\ System** on the **Camera Distance** and **Scale** properties.

The result of the formula mentioned above will be the multiplier of your pixel size. It is important to note that **Camera Distance** is directly related to how "far" away things are rendered -- so it is important to ensure that it is high enough to achieve the effect you want. A list of examples of the scale applied to pixels is listed below:

Camera Distance

Scale

Pixel Multiplier

6

1

3

4

.5

1

10

.2

1

8

2

8