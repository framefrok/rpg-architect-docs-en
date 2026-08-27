# Minimap

*Источник: https://docs.rpg-architect.com/10-user-interfaces/user-interface-type/minimap/*

---

# Minimap

## **Minimap**[¶](#minimap "Permanent link")

Minimap types render the current map's minimap into a designated element, allowing frames and text to be composed around it.

> **Note**: Functions like an overlay; assign a Picture element as the minimap and add other elements around it.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Always Center Player

Keeps the player centered in follow mode so the map slides beneath them at the edges, instead of the map stopping and the marker drifting toward the edge.

Framing Mode

How the minimap image is framed: fit the whole map, or follow the player with a zoomed crop.

Mask Image

An image whose alpha clips the minimap into a shape, such as a circle. Opaque areas keep the minimap and transparent areas are cut away to reveal what is behind it.

[Image](../../../05-reference/image/)

Mask Rotates With Map

Rotates the mask together with the map when following the camera. Enable it for a symmetrical mask such as a circle; disable it to keep an asymmetric mask like a star upright while the map turns beneath it.

Minimap Element

The element whose control is replaced with the rendered minimap.

[User Interface Element](../../user-interface-element/)

Rotate With Player

Rotates the minimap to follow the camera so the view direction points up. Applies to 3D maps only; 2D maps stay flat with north up.

Zoom

The zoom factor applied when following the player. Higher values show a smaller, more zoomed-in area.

Number

#### **[Minimap Framing Mode](#minimap-framing-mode)**[¶](#minimap-framing-mode "Permanent link")

Name

Explanation

Fit Whole

Fits the entire minimap image into the element.

Follow Player

Shows a cropped, zoomed region of the minimap centered on the player.