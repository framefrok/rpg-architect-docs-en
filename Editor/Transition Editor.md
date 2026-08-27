# Transition Editor

*Источник: https://docs.rpg-architect.com/04-editor/transition-editor/*

---

# Transition Editor

## **Transition Editor**[¶](#transition-editor "Permanent link")

The Transition Editor is where the animation between one screen and the next is configured — what the player sees as a scene arrives or leaves.

Transition chooses the effect, and the settings beneath it change to match what that effect needs. Duration sets how long it runs, and the [Easing Function](../easing-function-editor/) shapes how it progresses over that time rather than advancing evenly.

Enter and Exit are configured separately, so a screen can arrive one way and leave another.

The values a transition holds are documented under [Scene Transition](../../05-reference/scene-transition/).

![The Transition Editor](../media/img_40_transition-editor.png)

### ![1](../media/img_17_marker-01.png) Transition[¶](#transition "Permanent link")

Which effect plays. Everything below it follows from this choice.

### ![2](../media/img_18_marker-02.png) Settings[¶](#settings "Permanent link")

**The settings belong to the chosen transition**, so they are replaced when it changes - a fade asks for a colour and a duration, another effect asks for something else entirely. The full set for each is under [Scene Transition](../../05-reference/scene-transition/).

### ![3](../media/img_20_marker-03.png) Easing Function[¶](#easing-function "Permanent link")

Shapes how the transition progresses over its duration rather than advancing evenly - see [Easing Function Editor](../easing-function-editor/).

### ![4](../media/img_22_marker-04.png) Blend Mode[¶](#blend-mode "Permanent link")

How the transition's own drawing is composited over the scene beneath it.