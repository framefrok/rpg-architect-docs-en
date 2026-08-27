# Menus

*Источник: https://docs.rpg-architect.com/04-editor/menus/*

---

# Menus

## **Menus**[¶](#menus "Permanent link")

The menu bar runs across the top of the editor: **File**, **Editor**, **Macros**, **Tools**, and **Help**. Every entry on each of them is listed below, grouped by the menu it belongs to, with its keyboard shortcut where it has one.

Two of the menus are not fixed lists. **Macros** shows _Configure Macros_ followed by every macro you have set to appear there, so its contents are whatever the project defines - a macro can be set to appear in the menu, in the toolbar, in both, or in neither. **File** likewise grows a _Recents_ and a _Favorites_ submenu from the projects you have opened and saved.

> **Note**: Force Height Visibility and Force Region Visibility are mutually exclusive - turning one on turns the other off.

## **File**[¶](#file "Permanent link")

Name

Explanation

Shortcut

New Project

Creates a new project.

Ctrl+N

Open Project

Opens an existing project.

Ctrl+O

Save Project

Saves the current project.

Ctrl+S

Save Project As

Saves the current project to a new location, leaving the original untouched.

Close Project

Closes the current project and returns the editor to its empty state.

Recents

The projects opened most recently, and an entry to clear that history. It changes as you work.

Favorites

A fixed set of slots you fill yourself. An empty slot saves the current project into it; a filled one can be loaded, replaced, or cleared. Unlike Recents, it only changes when you say so.

Launch Pad

Opens the Launch Pad welcome hub.

Exit

Closes the editor.

Alt+F4

## **Editor**[¶](#editor "Permanent link")

Name

Explanation

Shortcut

Undo

Removes recent changes from the map.

Ctrl+Z

Redo

Reapplies recent changes to the map.

Ctrl+Y

Advanced Mode

Exposes the finer map editing controls. Unavailable while the map editor is in 3D mode.

Ctrl+A

Grid

Draws the tile grid.

Ctrl+G

Show Screen Frame

Overlays the area the player will actually see.

Ctrl+Shift+F

Layer Assist Mode

Fades the layers either side of the active one.

Ctrl+L

Object Grid Assist

Locks doodads, entities and the like to the nearest whole tile rather than placing them freely.

Ctrl+D

Collision Visualization

Draws every collision on the current layer.

Ctrl+I

Force Height Visibility

Keeps height drawn on the current layer rather than only while its tool is in use. Turning this on turns Force Region Visibility off.

Ctrl+H

Force Region Visibility

Keeps the region drawn on the current layer. Turning this on turns Force Height Visibility off.

Ctrl+R

Force Shape Visibility

Keeps the shape drawn on the current layer.

Ctrl+P

Rebuild All Map Caches

Rebuilds the mesh cache for every map in the project.

Rebuild All Minimaps

Rebuilds the exported minimap image for every map in the project.

Editor Settings

Opens the settings dialog, the light theme toggle, and the editor's own language options - see [Editor Settings](../editor-settings/).

## **Macros**[¶](#macros "Permanent link")

Name

Explanation

Shortcut

Configure Macros

Opens the macro editor, where each macro is given a name, an icon, and the process it launches.

## **Tools**[¶](#tools "Permanent link")

Name

Explanation

Shortcut

Database

Opens the [Database](../database/) window, where most of a game's content is configured.

F8

Open Project Directory

Opens the project's own folder.

F12

Import Resource Packages

Opens the resource package importer.

Publish Game

Builds a distributable copy of the game.

F6

Run Test Game

Runs a test version of the current project without publishing it first.

F5

## **Help**[¶](#help "Permanent link")

Name

Explanation

Shortcut

Leave Feedback

Opens the feedback survey.

Open Documentation

Opens this documentation.

Open Forum

Opens the forums.

Open Tutorials

Opens the tutorial material.

Discord

Opens the Discord server.

About

Shows the version of the editor currently running - worth checking before reporting a problem.