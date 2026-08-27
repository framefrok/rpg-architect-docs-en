# Collider

*Источник: https://docs.rpg-architect.com/05-reference/collider/*

---

# Collider

## **Collider**[¶](#collider "Permanent link")

Colliders are low-level collision detection shapes used by the physics engine. Each entity, doodad, or physics object can have a collider that defines its physical boundaries for collision detection and response.

Colliders work in three dimensions, where width, height, and depth correspond to the X, Y, and Z axes respectively.

## **Shapes**[¶](#shapes "Permanent link")

The following shapes are available for colliders:

Name

Explanation

Sphere

Defined by a single diameter. One of the fastest native shapes and ideal for characters. Collides uniformly in all directions.

Capsule

Defined by a diameter and a height. A capsule is a cylinder capped with hemispheres on each end. The total height is the cylinder portion plus the full diameter (one hemisphere radius on each end), so a capsule with diameter 0.2 and height 1.0 has an actual height of 1.2. One of the most efficient shapes and ideal for characters.

Cylinder

Defined by a diameter and a height. A circular cross-section extruded vertically.

Box

Defined by width, height, and depth. Best for static objects like walls, crates, and barriers. Not recommended for moving characters — corners can catch on geometry and produce unpredictable collisions.

Convex Hull

Defined by a set of 3D points that form a convex shape. Useful for irregular objects that don't fit standard primitives. Slower than primitive shapes.

Mesh

Defined by a triangle mesh. The most flexible shape but also the slowest. Suitable for complex static geometry.

> **Note**: Spheres and Capsules are the recommended shapes for characters and moving entities. They are the most efficient and behave predictably during movement.
> 
> **Note**: Boxes work poorly for characters that move around — corners catch on geometry and produce unpredictable collisions. Use Boxes for static obstacles like walls, crates, and barriers.