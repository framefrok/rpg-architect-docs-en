# Text Escape Codes

*Источник: https://docs.rpg-architect.com/05-reference/text-escape-codes/*

---

# Text Escape Codes

## **Text Escape Codes**[¶](#text-escape-codes "Permanent link")

Text escape codes are special codes that you can use in dialogue and message boxes to dynamically manipulate output during runtime. This gives you the capability to change text color, size, insert variable values, party members' names, change message speed, to name a few.

They are generally broken down into three categories: **Formatters**, **Control Sequences**, and **Replacements**.

**Formatters** format the text and change how it is presented, such as changing the text color, font, weight, and so forth. **Control Sequences** change and control how text interaction occurs, such as causing a wait. **Replacements** replace the text with values, such as a character name, party member, variable value, money, and so forth.

### Formatters[¶](#formatters "Permanent link")

Name

Description

Parameters

Example

`<`

Adds a `<`.

None

`<< only one less than sign will appear.`

`b`

Bolds a text sequence.

None

`<b>This is bolded.</b>`

`i`

Italicizes a text sequence.

None

`<i>This is italicized.</i>`

`s`

Strikethroughs a text sequence.

None

`<s>This is struck-through.</s>`

`u`

Underlines a text sequence.

None

`<u>This is underlined.</u>`

`left`

Horizontally aligns a text sequence to the left.

None

`<left>Aligned left.</left>`

`center`

Horizontally aligns a text sequence to the center.

None

`<center>Aligned center.</center>`

`right`

Horizontally aligns a text sequence to the right.

None

`<right>Aligned right.</right>`

`fontsize`

Changes the font size.

Font Size (Number)

`<fontsize[50]>50pt font.</fontsize>`

`fontcolor`

Changes the font color.

Hex (#RGB, #ARGB, #RRGGBB, #AARRGGBB) or CSV (R,G,B or R,G,B,A)

`<fontcolor[255,0,0]>Red text.</fontcolor>`

`fontfamily`

Changes the font family.

Font Family (Number)

`<fontfamily[3]>Fourth font family.</fontfamily>`

`outline` / `outlinecolor`

Enables an outline in the given color.

Hex (#RGB, #ARGB, #RRGGBB, #AARRGGBB) or CSV (R,G,B or R,G,B,A)

`<outline[0,0,0]>Outlined text.</outline>`

`outlinethickness`

Sets the outline thickness (and enables the outline).

Thickness in pixels (Number). Default: 1

`<outlinethickness[2]>Thick outline.</outlinethickness>`

`glow` / `glowcolor`

Enables a glow in the given color.

Hex (#RGB, #ARGB, #RRGGBB, #AARRGGBB) or CSV (R,G,B or R,G,B,A)

`<glow[255,140,0]>Glowing text.</glow>`

`glowradius`

Sets the glow radius/spread (and enables the glow).

Radius in pixels (Number). Default: 3

`<glowradius[5]>Wider glow.</glowradius>`

`glowintensity`

Sets the glow intensity/strength (and enables the glow).

Stacked passes (Number). Default: 1

`<glowintensity[3]>Bold glow.</glowintensity>`

`portraitexpression` / `pe`

Changes the portrait expression.

Expression (Number)

`<pe[1]>Second expression.</pe>`

`pitch`

Adjusts the character sound pitch.

Value or Min, Max (Number)

`<pitch[-.4]>Lower pitch.</pitch>`

`shake`

Shakes the text in X and Y directions.

X, Y (Number). Default: 2, 2

`<shake[4,10]>Shaking text.</shake>`

`sound`

Changes the character sound.

Name or Name, Pan, Pitch, Volume

`<sound[path.ogg,1,0.4,1]>Custom sound.</sound>`

`volume`

Sets the character sound volume.

Value or Min, Max (Number, 0 to 1)

`<volume[0.5]>Quieter sound.</volume>`

`pan`

Sets the character sound stereo pan.

Value or Min, Max (Number, -1 to 1)

`<pan[-1]>Left ear.</pan>`

`wave`

Waves text along a sine wave.

Factor, Speed (Number). Default: 1, 2

`<wave[4,2.5]>Wavy text.</wave>`

`characterdelay` / `cd`

Changes the delay between each character.

Duration in ms (Number)

`<cd[20]>Fast text.</cd>`

### Control Sequences[¶](#control-sequences "Permanent link")

Name

Description

Parameters

Example

`continue`

Emulates a Confirm press, causing the text to paginate, continue, or close.

None

`<wait[500]><continue>`

`displayall`

Displays all text immediately, ignoring character delay. Requires a closing tag.

None

`<displayall>Instant text.</displayall>`

`pause`

Requires a Confirm press before continuing.

None

`Did <pause> you know <pause> you pressed twice?`

`wait`

Waits for a duration before display continues.

Duration in ms (Number)

`Wait 1 second <wait[1000]> continuing!`

### Replacements[¶](#replacements "Permanent link")

Name

Description

Parameters

Example

`globalvar` / `gv`

Displays a global variable value.

Index (Number)

`<globalvar[0]>`

`globalswitch` / `gs`

Displays a global switch value.

Index (Number)

`<gs[4]>`

`localvar` / `lv`

Displays a local variable value.

Index (Number)

`<localvar[0]>`

`localswitch` / `ls`

Displays a local switch value.

Index (Number)

`<ls[4]>`

`party`

Displays an active party member's name.

Index (Number)

`<party[0]>`

`inactiveparty`

Displays an inactive party member's name.

Index (Number)

`<inactiveparty[0]>`

`partystat` / `partystatistic`

Displays an active party member's statistic.

Index (Number), Formula (String)

`<partystat[0,hp]>`

`inactivepartystat`

Displays an inactive party member's statistic.

Index (Number), Formula (String)

`<inactivepartystatistic[0,str]>`

`character`

Displays a character name from the database.

Index (Number)

`<character[1]>`

`enemy`

Displays an enemy name from the database.

Index (Number)

`<enemy[3]>`

`fps`

Displays the current frames per second.

None

`<fps>`

`icon`

Displays an icon from the database.

Index (Number), optionally Size (px)

`<icon[4]>` or `<icon[4,32]>`

`item`

Displays an item name from the database.

Index (Number)

`<item[2]>`

`equipment`

Displays an equipment name from the database.

Index (Number)

`<equipment[4]>`

`mapname`

Displays the current map name.

None

`<mapname>`

`newline`

Inserts a new line.

None

`First line.<newline>Second line.`

`playtime`

Displays the current playtime.

Format String (Default: hh:mm:ss)

`<playtime>`

`machinename`

Displays the computer name.

None

`<machinename>`

`systemdate`

Displays the current date.

Format String (Default: d)

`<systemdate>`

`systemtime`

Displays the current time.

Format String (Default: t)

`<systemtime>`

`steps`

Displays the total steps taken.

None

`<steps>`

`encountersteps`

Displays steps toward next encounter.

None

`<encountersteps>`

`money` / `$`

Displays the party's money.

None

`<$>`

`mastermusicvolume`

Displays master music volume.

Format String (Default: P)

`<mastermusicvolume>`

`mastersfxvolume`

Displays master SFX volume.

Format String (Default: P)

`<mastersfxvolume>`

`camerax` / `cameray` / `cameraz`

Displays camera target coordinates.

Format String (Default: 0.000)

`<camerax>, <cameray>, <cameraz>`

`camerarotx` / `cameraroty` / `camerarotz`

Displays camera rotation in degrees.

Format String (Default: 0)

`<camerarotx>, <cameraroty>, <camerarotz>`

`camerarotxrad` / `camerarotyrad` / `camerarotzrad`

Displays camera rotation in radians.

Format String (Default: 0.000)

`<camerarotxrad>, <camerarotyrad>`

`partyx` / `partyy` / `partyz`

Displays party coordinates.

Format String (Default: 0.000)

`<partyx>, <partyy>, <partyz>`