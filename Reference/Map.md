# Map

*Источник: https://docs.rpg-architect.com/05-reference/map/*

---

# Map

## **Map**[¶](#map "Permanent link")

Maps define explorable areas with tile-based or pixel-based terrain, lighting, entities, scripts, and camera settings. Each map has its own layers, tilesets, music, and transition effects.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

ID

The ID of the map.

Number

Name

The name of the map.

String

#### **Appearance**[¶](#appearance "Permanent link")

Name

Explanation

Type

Background Color

The background color of the map.

Color

Background Music

The background music of the map.

[Music](../music/)

Height

The height of the map in tiles.

Number

Tileset

The tileset used in the map.

[Tileset](../../06-database/03-maps/01-tilesets/)

Width

The width of the map in tiles.

Number

Wrap Horizontal

Whether the map wraps horizontally.

Toggle

Wrap Vertical

Whether the map wraps vertically.

Toggle

#### **Camera**[¶](#camera "Permanent link")

Name

Explanation

Type

Distance

The overridden distance of the camera if applicable.

Number

Field of View

The overridden field of view of the camera if applicable.

Number

Offset X

The overridden offset of the camera from its target along the X axis if applicable.

Number

Offset Y

The overridden offset of the camera from its target along the Y axis if applicable. Increase this to raise the viewpoint, such as the eye height in first-person mode.

Number

Offset Z

The overridden offset of the camera from its target along the Z axis if applicable.

Number

Pitch

The overridden pitch of the camera if applicable.

Number

Render Distance

The overridden render distance of the camera if applicable.

Number

Reset to Default

Whether to reset the camera to the default values.

Toggle

Roll

The overridden roll of the camera if applicable.

Number

Scale

The overridden scale of the camera if applicable.

Number

Yaw

The overridden yaw of the camera if applicable.

Number

#### **Lighting**[¶](#lighting "Permanent link")

Name

Explanation

Type

Ambient Color

The ambient light color of the map.

Color

Directional Color

The directional light color of the map.

Color

Directional Light Direction

The direction of the directional light of the map.

Vector

Enable

Whether lighting is enabled on the map.

Toggle

#### **Physics**[¶](#physics "Permanent link")

Name

Explanation

Type

Tile-Based Movement

Whether the map uses tile-based movement.

Toggle

#### **Scripts**[¶](#scripts "Permanent link")

Name

Explanation

Type

Enter Map

The script to execute when entering the map.

[Script](../script/)

Exit Map

The script to execute when exiting the map.

[Script](../script/)

Load Map

The script to execute when the map loads, before the enter transition is displayed.

[Script](../script/)

Ongoing Map

The script to execute in the background of the map.

[Script](../script/)

Override Enter Map

Whether to override the enter script defined in the database.

Toggle

Override Exit Map

Whether to override the exit script defined in the database.

Toggle

Override Load Map

Whether to override the load script defined in the database.

Toggle

Override Ongoing Map

Whether to override the ongoing script defined in the database.

Toggle

#### **User Interfaces**[¶](#user-interfaces "Permanent link")

Name

Explanation

Type

Is Main Menu Enabled?

Whether the main menu is available on the map.

Toggle

Loading Screen

The user interface to use for the loading screen for the scene.

[User Interface](../../06-database/09-user-interfaces/00-user-interfaces/)

Main Menu

The main menu user interface to use on the map.

[User Interface](../../06-database/09-user-interfaces/00-user-interfaces/)

Minimap

The minimap user interface displayed on the map.

[User Interface](../../06-database/09-user-interfaces/00-user-interfaces/)

#### **Wind**[¶](#wind "Permanent link")

Name

Explanation

Type

Enable Wind

Whether wind is enabled on the map. When enabled, wind-eligible sprites sway based on the map's wind direction, strength, and gust settings.

Toggle

Wind Direction

The direction the wind blows. Combined with Wind Strength to determine the sway force on wind-eligible sprites.

Vector

Wind Gust Amplitude

The amplitude of wind gusts. 0 is steady wind, 1 is fairly choppy, 2 or more is stormy.

Number

Wind Gust Frequency

How fast wind gusts cycle, in cycles per second. Lower values are slow rolling gusts; higher values are staccato.

Number

Wind Strength

The strength of the wind, measured in tile scales of sway at full effect. 0 keeps everything still even when wind is enabled.

Number