# Sprite Rig

*Источник: https://docs.rpg-architect.com/05-reference/sprite-rig/*

---

# Sprite Rig

## **Sprite Rig**[¶](#sprite-rig "Permanent link")

A Sprite Rig lets a sprite bend, stretch, and squash to create animation its frames alone can't produce. You place control points on the sprite and move them across keyframes, and the image follows along, smoothly blending from one pose to the next. Rigs are set on an [Enemy](../../06-database/06-enemies/00-enemies/)'s appearance, and each animation can be tied to a [Battle Pose](../../06-database/07-battles/10-battle-poses/) so the right motion plays for the right pose.

> **Note**: Authoring is done in the **Sprite Rigging** tab on the Enemy editor. Place control points on the sprite preview, mark the outline points to define the silhouette, and add keyframes on the timeline to capture each pose snapshot.
> 
> **Note**: Keyframe transitions use the same [Easing Function](../easing-function/) type as the rest of the editor — the easing on a keyframe governs how the _previous_ keyframe blends into it, so the easing on the first keyframe of a non-looping animation is irrelevant.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Animations

The animations defined on this rig. Each one is attached to a [Battle Pose](../../06-database/07-battles/10-battle-poses/) so it plays when that pose is active; the animation with no pose set is the default.

Control Points

The control points that drive the deformable mesh.

Vector