---
title: Global Functions
description: 
published: true
date: 2022-10-28T02:39:24.325Z
tags: reference, vscript
editor: markdown
dateCreated: 2022-10-28T02:23:09.270Z
---

# Global Functions

These functions are available in every script.

## void AddBranchLevelName(int, string) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Adds a level to the specified branche's list.

## void AddCoopCreditsName(string) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Adds a name to the coop credit's list.

## handle CreateProp(string, Vector, string, int)
Create a physics prop

## handle CreateSceneEntity(string)
Create a scene entity to play the specified scene.

## void DebugDrawBox(Vector, Vector, Vector, int, int, int, int, float)
Draw a debug overlay box

## void DebugDrawEntityText(int, int, string, float, int, int, int, int)
Draw debug overlay entity text

## void DebugDrawEntityTextAtPosition(Vector, int, string, float, int, int, int, int)
Draw a debug overlay entity text at position

## void DebugDrawGrid(Vector)
Draw debug overlay grid

## void DebugDrawLine(Vector, Vector, int, int, int, bool, float)
Draw a debug overlay box

## void DebugDrawScreenText(float, float, string, int, int, int, int, float)
Draw debug overlay screen text

## void DebugDrawText(Vector, string, bool, float)
Draw debug overlay text

## void DebugDrawTri(Vector, Vector, Vector, int, int, int, int, bool, float)
Draw a debug overlay triangle

## void DispatchParticleEffect(string, Vector, Vector)
Dispatches a one-off particle system

## bool DoIncludeScript(string, handle)
Execute a script (internal-only)

## function EntFire(target, action, value, delay, activator)
Generate and entity i/o event

## void EntFireByHandle(handle, string, string, float, handle, handle)
Generate and entity i/o event. First parameter is an entity instance.

## float FrameTime()
Get the time spent on the server in the last frame

## int GetBluePlayerIndex() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Player index of the blue player.

## int GetCoopBranchLevelIndex(int) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Given the 'branch' argument, returns the current chosen level.

## int GetCoopSectionIndex() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Section that the coop players have selected to load.

## int GetDeveloperLevel()

Gets the level of 'developer'

## int GetHighestActiveBranch() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Returns which branches should be available in the hub.

## int GetMapIndexInPlayOrder() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Determines which index (by order played) this map is. Returns -1 if entry is not found. -2 if this is not a known community map.

## string GetMapName()

Get the name of the map.

## int GetNumMapsPlayed() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Returns how many maps the player has played through.

## int GetOrangePlayerIndex() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Player index of the orange player.

## handle GetPlayer()

Returns the player (SP Only).

## float GetPlayerSilenceDuration(int)

Time that the specified player has been silent on the mic.

## void GivePlayerPortalgun() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Give player the portalgun.

## bool IsLevelComplete(int, int) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Returns true if the level in the specified branch is completed by either player.

## bool IsMultiplayer()

Is this a multiplayer game?

## bool IsPlayerLevelComplete(int, int, int) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Returns true if the level in the specified branch is completed by a specific player.

## bool LoopSinglePlayerMaps()

Run the single player maps in a continuous loop.

## void MarkMapComplete(string) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Marks a maps a complete for both players.

## void PrecacheMovie(string)

Precaches a named movie. Only valid to call within the entity's 'Precache' function called on mapspawn.

## float RandomFloat(float, float)
Generate a random floating point number within a range, inclusive

## int RandomInt(int, int)
Generate a random integer within a range, inclusive

## void RecordAchievementEvent(string, int)

Records achievement event or progress

## void RequestMapRating() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Pops up the map rating dialog for user input

## void ScriptShowHudMessageAll(string, float)

Show center print text message.

## bool ScriptSteamShowURL(string)

Bring up the steam overlay and shows the specified URL.  (Full address with protocol type is required, e.g. http://www.steamgames.com/)

## void SendToConsole(string)

Send a string to the console as a command

## void SendToConsoleServer(string)

Send a string that gets executed on the server as a ServerCommand

## void SendToPanorama(string, string) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Send an event to Panorama

## void SetDucking(string, string, float) ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Set the level of an audio ducking channel

## int SetMapAsPlayed() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Adds the current map to the play order and returns the new index therein. Returns -2 if this is not a known community map.

## void ShowMessage(string)
Print a hud message on all clients

## float Time()
Get the current server time

## handle TraceHull(Vector, Vector, Vector, Vector, int, handle, int)

Sweeps a hull along the specified line. Returns a CGameTrace with the trace result

## float TraceLine(Vector start, Vector end, handle hEntToIgnore)

given 2 points & ent to ignore, return fraction along line that hits world or models

## handle TraceLineEx(Vector start, Vector end, int collisionGrp, handle hEntToIgnore, int traceMask)

Given 2 points, ent to ignore, collision group and trace mask, returns a CGameTrace with the result

## handle TracePortalLine(Vector start, Vector end, int collisionGrp, handle hEntToIgnore, int traceMask)

Same as TraceLineEx, but will transform the trace based on any portals it passes through.

## bool TryDLC1InstalledOrCatch() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Tests if the DLC1 is installed for Try/Catch blocks.

## function UniqueString(string)

Generate a string guaranteed to be unique across the life of the script VM, with an optional root string. Useful for adding data to tables when not sure what keys are already in use in that table.

## void UpgradePlayerPortalgun() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Give player the portalgun.

## void UpgradePlayerPotatogun() ![p2ce-icon.png](/assets/p2ce-icon.png =18x)

Give player the portalgun.