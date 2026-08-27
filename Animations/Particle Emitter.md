# Particle Emitter

*Источник: https://docs.rpg-architect.com/09-animations/animation-element/particle-emitter/*

---

# Particle Emitter

## **Particle Emitter**[¶](#particle-emitter "Permanent link")

Particle Emitter elements generate streams of particles inside an animation, with configurable spawn rates, effects, and lifetimes.

## **Properties**[¶](#properties "Permanent link")

#### **System**[¶](#system "Permanent link")

Name

Explanation

Type

Name

The name of this animation element. Used for identification in the timeline.

String

#### **Emitter**[¶](#emitter "Permanent link")

Name

Explanation

Type

Duration

The duration of the particle emitter in milliseconds. Controls how long new particles are spawned.

Number

Maximum Particles

The maximum number of particles that can exist at once. Limits memory and visual density.

Number

Minimum Particles

The minimum number of particles that are always active. The emitter spawns instantly to meet this floor.

Number

Particles Per Second

The rate at which new particles are spawned per second. Higher values create denser effects.

Number

#### **Particle Appearance**[¶](#particle-appearance "Permanent link")

Name

Explanation

Type

Color

The base color mask applied to each particle. Use to tint all particles from this emitter.

Color

Texture Region

The region of the source texture used for each particle. Use to select a portion of a sprite sheet.

Rectangle

Texture Source

The file path of the source texture image for each particle.

[Image](../../../05-reference/image/)

#### **Particle Effects**[¶](#particle-effects "Permanent link")

Name

Explanation

Type

Birth Effects

The effects applied when a particle is first spawned. Use to set initial position, velocity, or appearance.

[Particle Effect](../../particle-effect/)

Death Effects

The effects applied when a particle reaches the end of its lifetime. Use for fade-out or shrink effects.

[Particle Effect](../../particle-effect/)

Ongoing Effects

The effects applied each frame while a particle is alive. Use for movement, color shifts, or scaling over time.

[Particle Effect](../../particle-effect/)