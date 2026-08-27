# Graphics Post Processors

*Источник: https://docs.rpg-architect.com/05-reference/graphics-post-processor/*

---

# Graphics Post Processors

## **Graphics Post Processors**[¶](#graphics-post-processors "Permanent link")

Graphics Post Processors are visual effects applied to the rendered scene as a final pass. They can be stacked and conditionally enabled using [Conditions](../condition/). Post processors are configured on scene databases such as [Map Configuration](../../06-database/03-maps/00-configuration/), [Battle Configuration](../../06-database/07-battles/00-configuration/), [Title](../../06-database/10-system/20-title/), and [Game Over](../../06-database/10-system/25-game-over/).

* * *

## **Bloom**[¶](#bloom "Permanent link")

Bloom post-processing effect that adds a glow to bright areas of the scene.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Intensity

The strength of the bloom glow. Range: 0 to 5. Default: 1.

Number

Threshold

The brightness level above which bloom is applied. Range: 0 to 2. Default: 0.8.

Number

* * *

## **Cel Shading**[¶](#cel-shading "Permanent link")

Cel-shading post-processing effect that quantizes lighting into discrete bands and draws geometry-aware outlines using the depth and normal buffers.

## **Properties**[¶](#properties_1 "Permanent link")

#### **System**[¶](#system_1 "Permanent link")

Name

Explanation

Type

Intensity

The overall strength of the cel-shading effect. Range: 0 to 1. Default: 1.

Number

Levels

The number of discrete luminance bands. Range: 2 to 16. Default: 4.

Number

Offset

The smoothness of transitions between luminance bands. Range: 0 to 0.2. Default: 0.05.

Number

Size

The width of the edge outlines in texels. Range: 0.5 to 5. Default: 1.

Number

Threshold

The minimum edge strength to draw an outline. Range: 0.01 to 0.5. Default: 0.1.

Number

* * *

## **Chromatic Aberration**[¶](#chromatic-aberration "Permanent link")

Chromatic aberration post-processing effect that offsets RGB channels toward the screen edges.

## **Properties**[¶](#properties_2 "Permanent link")

#### **System**[¶](#system_2 "Permanent link")

Name

Explanation

Type

Intensity

The overall strength of the aberration. Range: 0 to 2. Default: 0.5.

Number

Offset

The pixel offset between RGB channels. Range: 0 to 10. Default: 1.

Number

* * *

## **Color Blindness**[¶](#color-blindness "Permanent link")

Color blindness post-processing effect that remaps confusable colors so players with a color vision deficiency can tell them apart.

## **Properties**[¶](#properties_3 "Permanent link")

#### **System**[¶](#system_3 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the correction, from a subtle nudge to a full remap. Range: 0 to 1. Default: 1.

Number

Type

The type of color vision deficiency to correct for. Range: 0 to 3. Default: 0.

Number

* * *

## **Color Grading**[¶](#color-grading "Permanent link")

Color grading post-processing effect that adjusts brightness, contrast, and saturation.

## **Properties**[¶](#properties_4 "Permanent link")

#### **System**[¶](#system_4 "Permanent link")

Name

Explanation

Type

Brightness

The overall brightness multiplier. Range: 0 to 3. Default: 1.

Number

Contrast

The contrast multiplier. Range: 0 to 3. Default: 1.

Number

Saturation

The color saturation multiplier. Range: 0 to 3. Default: 1.

Number

* * *

## **CRT**[¶](#crt "Permanent link")

CRT post-processing effect that simulates a cathode ray tube display with barrel distortion and scanlines.

## **Properties**[¶](#properties_5 "Permanent link")

#### **System**[¶](#system_5 "Permanent link")

Name

Explanation

Type

Curvature

The amount of barrel distortion. Range: 0 to 0.1. Default: 0.02.

Number

Intensity

The overall strength of the CRT effect. Range: 0 to 1. Default: 1.

Number

Size

The RGB sub-pixel separation distance. Range: 1 to 4. Default: 2.

Number

* * *

## **Depth of Field**[¶](#depth-of-field "Permanent link")

Depth of field post-processing effect that blurs areas outside of a focal range.

## **Properties**[¶](#properties_6 "Permanent link")

#### **System**[¶](#system_6 "Permanent link")

Name

Explanation

Type

Blur Size

The maximum radius of the blur in pixels. Range: 1 to 32. Default: 8.

Number

Focus Distance

The distance from the camera that is in perfect focus, in world units. Range: 0.1 to 100. Default: 10.

Number

Focus Range

The width of the in-focus band around the focus distance, in world units. Range: 0.1 to 50. Default: 5.

Number

Intensity

The overall strength of the blur effect. Range: 0 to 1. Default: 1.

Number

* * *

## **Dither**[¶](#dither "Permanent link")

Dither post-processing effect that applies ordered dithering using a 4x4 Bayer matrix.

## **Properties**[¶](#properties_7 "Permanent link")

#### **System**[¶](#system_7 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the dithering effect. Range: 0 to 1. Default: 1.

Number

Levels

The number of color levels per channel. Range: 2 to 32. Default: 8.

Number

Size

The scale of the dither pattern. Range: 1 to 8. Default: 1.

Number

* * *

## **Film Grain**[¶](#film-grain "Permanent link")

Film grain post-processing effect that adds a noise overlay to the scene.

## **Properties**[¶](#properties_8 "Permanent link")

#### **System**[¶](#system_8 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the grain noise. Range: 0 to 1. Default: 0.5.

Number

Size

The size of the grain particles. Range: 0.5 to 4. Default: 1.

Number

* * *

## **FXAA**[¶](#fxaa "Permanent link")

Fast Approximate Anti-Aliasing (FXAA) smooths jagged edges by detecting and blending high-contrast boundaries in the final image.

## **Properties**[¶](#properties_9 "Permanent link")

#### **System**[¶](#system_9 "Permanent link")

Name

Explanation

Type

Intensity

The overall strength of the anti-aliasing effect. Range: 0 to 1. Default: 1.

Number

Offset

The amount of sub-pixel blending applied to smooth edges. Range: 0 to 1. Default: 0.75.

Number

Threshold

The minimum contrast required to apply anti-aliasing. Range: 0.063 to 0.333. Default: 0.166.

Number

* * *

## **Gaussian Blur**[¶](#gaussian-blur "Permanent link")

Gaussian blur post-processing effect that applies a multi-pass blur to the scene.

## **Properties**[¶](#properties_10 "Permanent link")

#### **System**[¶](#system_10 "Permanent link")

Name

Explanation

Type

Blur Size

The radius of the blur in pixels. Range: 1 to 16. Default: 4.

Number

Intensity

The strength of the blur effect. Range: 0 to 1. Default: 1.

Number

* * *

## **Grayscale**[¶](#grayscale "Permanent link")

Grayscale post-processing effect that desaturates the scene to black and white.

## **Properties**[¶](#properties_11 "Permanent link")

#### **System**[¶](#system_11 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the desaturation. Range: 0 to 1. Default: 1.

Number

* * *

## **Heat Haze**[¶](#heat-haze "Permanent link")

Heat haze post-processing effect that creates a shimmering distortion.

## **Properties**[¶](#properties_12 "Permanent link")

#### **System**[¶](#system_12 "Permanent link")

Name

Explanation

Type

Amplitude

The strength of the wave displacement. Range: 0.001 to 0.05. Default: 0.01.

Number

Frequency

The frequency of the distortion waves. Range: 1 to 50. Default: 10.

Number

Intensity

The overall strength of the distortion. Range: 0 to 1. Default: 0.5.

Number

Speed

The speed of the distortion animation. Range: 0.1 to 10. Default: 1.

Number

* * *

## **Hue Shift**[¶](#hue-shift "Permanent link")

Hue shift post-processing effect that rotates the hue of all colors.

## **Properties**[¶](#properties_13 "Permanent link")

#### **System**[¶](#system_13 "Permanent link")

Name

Explanation

Type

Angle

The hue rotation angle in degrees. Range: 0 to 360. Default: 0.

Number

* * *

## **Invert**[¶](#invert "Permanent link")

Invert post-processing effect that negates the colors of the scene.

## **Properties**[¶](#properties_14 "Permanent link")

#### **System**[¶](#system_14 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the color inversion. Range: 0 to 1. Default: 1.

Number

* * *

## **Outline**[¶](#outline "Permanent link")

Outline post-processing effect that detects and draws edges using a Sobel filter.

## **Properties**[¶](#properties_15 "Permanent link")

#### **System**[¶](#system_15 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the edge overlay. Range: 0 to 1. Default: 1.

Number

Size

The scale of the edge detection kernel. Range: 0.5 to 3. Default: 1.

Number

Threshold

The minimum edge strength to detect. Range: 0 to 1. Default: 0.1.

Number

* * *

## **Pixelate**[¶](#pixelate "Permanent link")

Pixelate post-processing effect that reduces the effective resolution for a retro look.

## **Properties**[¶](#properties_16 "Permanent link")

#### **System**[¶](#system_16 "Permanent link")

Name

Explanation

Type

Size

The size of each pixel block. Range: 1 to 32. Default: 4.

Number

* * *

## **Posterize**[¶](#posterize "Permanent link")

Posterize post-processing effect that reduces the number of color levels.

## **Properties**[¶](#properties_17 "Permanent link")

#### **System**[¶](#system_17 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the posterization effect. Range: 0 to 1. Default: 1.

Number

Levels

The number of color levels per channel. Range: 2 to 32. Default: 8.

Number

* * *

## **Radial Blur**[¶](#radial-blur "Permanent link")

Radial blur post-processing effect that blurs outward from the center of the screen.

## **Properties**[¶](#properties_18 "Permanent link")

#### **System**[¶](#system_18 "Permanent link")

Name

Explanation

Type

Blur Size

The maximum blur distance from center. Range: 0.001 to 0.1. Default: 0.02.

Number

Intensity

The overall strength of the radial blur. Range: 0 to 1. Default: 0.5.

Number

* * *

## **Scanlines**[¶](#scanlines "Permanent link")

Scanlines post-processing effect that applies retro CRT-style horizontal lines.

## **Properties**[¶](#properties_19 "Permanent link")

#### **System**[¶](#system_19 "Permanent link")

Name

Explanation

Type

Intensity

The darkness of the scanlines. Range: 0 to 1. Default: 0.5.

Number

Spacing

The gap between scanlines in pixels. Range: 1 to 8. Default: 2.

Number

Width

The thickness of each scanline in pixels. Range: 1 to 4. Default: 1.

Number

* * *

## **Sepia**[¶](#sepia "Permanent link")

Sepia post-processing effect that applies a warm, aged tone to the scene.

## **Properties**[¶](#properties_20 "Permanent link")

#### **System**[¶](#system_20 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the sepia tone. Range: 0 to 1. Default: 1.

Number

* * *

## **Sharpen**[¶](#sharpen "Permanent link")

Sharpen post-processing effect that enhances edges using an unsharp mask.

## **Properties**[¶](#properties_21 "Permanent link")

#### **System**[¶](#system_21 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the sharpening effect. Range: 0 to 3. Default: 1.

Number

* * *

## **SMAA**[¶](#smaa "Permanent link")

Subpixel Morphological Anti-Aliasing (SMAA) detects edges using luminance contrast and performs neighborhood blending for high-quality anti-aliased output.

## **Properties**[¶](#properties_22 "Permanent link")

#### **System**[¶](#system_22 "Permanent link")

Name

Explanation

Type

Intensity

The overall strength of the anti-aliasing effect. Range: 0 to 1. Default: 1.

Number

Threshold

The minimum luminance contrast required to detect an edge. Range: 0.05 to 0.5. Default: 0.1.

Number

* * *

## **Tilt Shift**[¶](#tilt-shift "Permanent link")

Simulates a miniature or diorama look by selectively blurring areas above and below a configurable focus band.

## **Properties**[¶](#properties_23 "Permanent link")

#### **System**[¶](#system_23 "Permanent link")

Name

Explanation

Type

Blur Size

The maximum blur radius at the edges of the screen. Range: 0.5 to 10. Default: 3.

Number

Focus Distance

The vertical center of the sharp focus band. Range: 0 to 1. Default: 0.5.

Number

Focus Range

The width of the sharp focus band. Range: 0.05 to 0.8. Default: 0.2.

Number

Intensity

The overall strength of the tilt-shift effect. Range: 0 to 1. Default: 1.

Number

* * *

## **Underwater**[¶](#underwater "Permanent link")

Underwater post-processing effect that creates a wavy distortion with a blue-green tint.

## **Properties**[¶](#properties_24 "Permanent link")

#### **System**[¶](#system_24 "Permanent link")

Name

Explanation

Type

Amplitude

The strength of the wave displacement. Range: 0.001 to 0.03. Default: 0.005.

Number

Frequency

The frequency of the distortion waves. Range: 1 to 20. Default: 8.

Number

Intensity

The overall strength of the underwater effect. Range: 0 to 1. Default: 0.5.

Number

Speed

The speed of the wave animation. Range: 0.1 to 5. Default: 1.

Number

* * *

## **Vertical Scanlines**[¶](#vertical-scanlines "Permanent link")

Vertical scanlines post-processing effect that applies retro CRT-style vertical lines.

## **Properties**[¶](#properties_25 "Permanent link")

#### **System**[¶](#system_25 "Permanent link")

Name

Explanation

Type

Intensity

The darkness of the scanlines. Range: 0 to 1. Default: 0.5.

Number

Spacing

The gap between scanlines in pixels. Range: 1 to 8. Default: 2.

Number

Width

The thickness of each scanline in pixels. Range: 1 to 4. Default: 1.

Number

* * *

## **Vignette**[¶](#vignette "Permanent link")

Vignette post-processing effect that darkens the edges of the screen.

## **Properties**[¶](#properties_26 "Permanent link")

#### **System**[¶](#system_26 "Permanent link")

Name

Explanation

Type

Intensity

The strength of the darkening at the edges. Range: 0 to 2. Default: 0.5.

Number

Radius

How far the vignette extends from the edges. Range: 0 to 1. Default: 0.8.

Number