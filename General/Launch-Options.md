---
title: Launch Options
description: Commonly used launch options
published: true
date: 2022-10-26T19:24:57.017Z
tags: engine, reference
editor: markdown
dateCreated: 2022-10-26T07:07:06.456Z
---

# Launch Options

This document only lists Chaos Source-specific launch options, for a full list
of launch options, please see
[the Valve Developer Wiki page](https://developer.valvesoftware.com/wiki/Command_Line_Options).

| Option                   | Description                                                                                                |
| ------------------------ | ---------------------------------------------------------------------------------------------------------- |
| -mountmod <path>         | Specifies the mod to launch the game with. Must be an absolute path                                        |
| -nogamemount             | Do not mount any games/mods specified in the gameinfo mounts block or mounts.kv                            |
| -nocustommount           | Do not mount any folders specified in gameinfo which contain wildcards (\* or ?), usually "custom" folders |
| -legacyui                | Launches the game with the old VGUI GameUI                                                                 |
| -dev                     | Developer mode                                                                                             |
| -dx11                    | Launch game with DirectX 11 shaderapi. On Linux, this will launch dx11 with dxvk. This option is default.                          |
| -dx9 | Launch the game with DirectX 9. On Linux this will launch the game with D9VK. 
| -multirun/-allowmultiple | Disables the creation of the source engine mutex, and allows the game to start even if one already exists  |

## Linux-specific options (Not available on Windows)

The following options are only available on Linux currently.

| Option         | Description                                                                                          |
| -------------- | ---------------------------------------------------------------------------------------------------- |
| -nomousegrab   | Forbids the game from grabbing the mouse                                                             |
| -exclusivefs   | Run game with non-desktop friendly fullscreen. This will resize your display resolution (Deprecated) |
| -noexclusivefs | Run game with desktop friendly fullscreen, which is the default regardless (Deprecated)              |

## Hammer Options

| Option      | Description                                                 |
| ----------- | ----------------------------------------------------------- |
| -winecompat | Runs hammer with some workarounds for wine bugs and behavior differences |
