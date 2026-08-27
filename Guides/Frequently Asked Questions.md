# Frequently Asked Questions

*Источник: https://docs.rpg-architect.com/02-guides/02-faq/*

---

# Frequently Asked Questions

## **Frequently Asked Questions**[¶](#frequently-asked-questions "Permanent link")

### **General Questions**[¶](#general-questions "Permanent link")

#### **What platforms does RPG Architect support?**[¶](#what-platforms-does-rpg-architect-support "Permanent link")

The editor for RPG Architect has been released on x86-64 Windows, Mac OSX, and Linux. The editor is primarily developed and tested on Windows, with some testing on OSX and Ubuntu. While there isn't active development on non-Windows platform, it should perform the same. If there are issues, please contact us immediately through our support channels.

The game engine for RPG Architect currently runs and has been tested on Windows, Mac OSX, and Linux. Support for console and mobile platforms will occur after release.

Console/Mobile platform support will become a priority (potentially before leaving Early Access), if a game is finished and is ready.

Android support is planned via wasm.

#### **How will console and mobile support work?**[¶](#how-will-console-and-mobile-support-work "Permanent link")

You will need to have proof that you are a console/mobile developer. Once acquired, you will be given access to build your game for the appropriate platform.

#### **What kind of hardware does RPG Architect run on?**[¶](#what-kind-of-hardware-does-rpg-architect-run-on "Permanent link")

RPG Architect should easily run on anything in the last 15 years.

Before release into Early Access, RPG Architect was tested with an unoptimized build on a laptop from 2009 with a dual-core processor, 2GB of RAM, a 5400 RPM hard drive, an "integrated" (re: no) graphics card, and Windows 8. These are below the specifications required for Windows 8. The editor ran fairly smoothly and the engine was able to run a 3D scene with dynamic lighting/shadows, 20 entities, and several animated layers at a stable 30-45 FPS.

Everything has become more optimized since then, so it is likely it would run even better on that older hardware.

#### **When will RPG Architect be released from early access?**[¶](#when-will-rpg-architect-be-released-from-early-access "Permanent link")

When it's ready. The goal is Q4 2026.

#### **I'd like to request a key for RPG Architect.**[¶](#id-like-to-request-a-key-for-rpg-architect "Permanent link")

Great!

I'm happy to provide one when it is mutually beneficial and you meet the requirements. Please be sure to watch the [Tutorials](../05-tutorials/) to get a feel for what the engine is capable of and how to use it. Once you have a good feel for RPG Architect's capabilities and usability, feel free to make a request with what you're dreaming to build or are offering in terms of resources/influences, and how it will benefit RPG Architect (**include links/proof to any media/influential presence**)

Your request should be thoughtful, persuasive, and show a clear understanding of what RPG Architect is capable of from your research. Use of AI-generated content is explicitly prohibited.

### **Technical Questions**[¶](#technical-questions "Permanent link")

#### **What is RPG Architect written in?**[¶](#what-is-rpg-architect-written-in "Permanent link")

C# and .NET. The editor utilizes AvaloniaUI. The Desktop, iOS, and Console engines leverage FNA. The Android engine utilizes MonoGame.

#### **What kind of lighting does RPG Architect support?**[¶](#what-kind-of-lighting-does-rpg-architect-support "Permanent link")

Lighting is visible in 2D and 3D scenes with [Dynamic Lighting](../../06-database/10-system/00-video-configuration/) enabled. There is support for one directional light (e.g. the sun/moon/whatever you want to use) and several omni-directional lights (spheres) or sliced lights (similar to omni-directional, but limited in angle/direction). The directional light is the only light that will actually generate shadows.

#### **What kind of scripting does RPG Architect allow for?**[¶](#what-kind-of-scripting-does-rpg-architect-allow-for "Permanent link")

The primary scripting in editor is a visual scripting language composed of [Commands](../../07-commands/). As a secondary goal, RPG Architect will allow for C# plugins to be installed to enhance features.

#### **How do plugins work in RPG Architect?**[¶](#how-do-plugins-work-in-rpg-architect "Permanent link")

> **Disclaimer**: This information is subject to change. Plugin support is in pre-alpha.

The low level engine of RPG Architect is actually agnostic to games and serves only to render, capture input, play audio, and so forth; RPG Architect is essentially a "plugin" to this engine with specific instructions on how to load. Everything in RPG Architect is a Core (with RPG Architect itself being one as well), and Cores are synonymous with Plugins. RPG Architect, itself, has a MAR.Game.RPGCore.Interfaces.dll that has our native types and interfaces, which can essentially be overridden with custom C# code. The lower level engine, then, creates a dependency mapping that allows you to specify whether to overwrite behavior or enhance it, as available. The order in which Plugins are installed will impact how they behave.

Support is extremely experimental at this point and not recommended or officially supported. This will be expanded upon after Early Access.