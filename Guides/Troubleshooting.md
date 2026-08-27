# Troubleshooting

*Источник: https://docs.rpg-architect.com/02-guides/04-troubleshooting/*

---

# Troubleshooting

## **Troubleshooting**[¶](#troubleshooting "Permanent link")

#### **How do I find my Editor logs?**[¶](#how-do-i-find-my-editor-logs "Permanent link")

*   An **Editor.log** will be present in the install directory for RPG Architect. You can find it by browsing to where Steam downloaded and installed RPG Architect to.

![editor-log-1](../media/img_4_editor-log-1.png "editor-log-1")

Context click on **RPG Architect**, then click **Properties**.

![editor-log-2](../media/img_5_editor-log-2.png "editor-log-2")

Click **Installed Files**, then click **Browse...**

![editor-log-3](../media/img_6_editor-log-3.png "editor-log-3")

**Editor.log** will be in this directory.

#### **How do I find my Engine logs?**[¶](#how-do-i-find-my-engine-logs "Permanent link")

An **Engine.log** will be present in the root folder of your game project. It lives in the same directory as the Content folder and your project file.

![engine-log-1](../media/img_7_engine-log-1.png "engine-log-1")

Click on the **Folder** icon in the RPG Architect toolbar.

![engine-log-2](../media/img_8_engine-log-2.png "engine-log-2")

**Engine.log** will be in this directory.

#### **RPG Architect's editor will not load my game.**[¶](#rpg-architects-editor-will-not-load-my-game "Permanent link")

Please check for diagnostic errors that are logged to Editor.log in the RPG Architect application directory or your project root directory, alongside the RPG.project file.

#### **RPG Architect will not run my game in test mode.**[¶](#rpg-architect-will-not-run-my-game-in-test-mode "Permanent link")

Please share a zipped copy of your project with support staff on the [Discord #support](https://discord.com/channels/798403733628518451/798404049329717259) channel.

#### **RPG Architect displays a blank screen when I run my game in test mode.**[¶](#rpg-architect-displays-a-blank-screen-when-i-run-my-game-in-test-mode "Permanent link")

By default, RPG Architect will try to render a title screen, even if no title menu has been set. You will need to either:

*   Toggle the **Skip Title** property under [Database \\ System \\ Title](../../06-database/10-system/20-title/).
*   Specify the **Menu** property under [Database \\ System \\ Title](../../06-database/10-system/20-title/).

#### **RPG Architect's test mode opens and then closes.**[¶](#rpg-architects-test-mode-opens-and-then-closes "Permanent link")

This is because RPG Architect uses Vulkan the rendering pipeline now, as the modern default of FNA and SDL. You can enable the legacy mode (Open GL) under **Editor** \\ **Editor Settings** \\ **Edit Settings** under the **Debugging Settings** category with the toggle **Legacy Video Mode**.

![LegacyVideoMode](../media/img_9_LegacyVideoMode.png "LegacyVideoMode")