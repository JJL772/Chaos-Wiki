---
title: ConVar Defaults
description: ConVar defaults system
published: true
date: 2022-10-28T01:27:21.111Z
tags: engine, modding
editor: markdown
dateCreated: 2022-10-28T01:27:21.111Z
---

# ConVar Defaults

Chaos ships with a system to modify the default values of ConVars at runtime. This allows mods and games to change various game defaults and settings at runtime rather than needing to recompile the engine with new changes.

When the engine is initialized, it will look for `cfg/cvar_defaults.cfg` or `cfg/cvar_defaults.kv3` under the `MOD` search path.

If you're creating a mod, you **must** make sure to include `cvar_defaults.cfg` or add P2CE as a `MOD` searchpath in gameinfo. Otherwise you may run into issues involving game movement, rendering, etc.

## Example `cvar_defaults.cfg`

The format for `cvar_defaults.cfg` is identical to any other `.cfg` file that you can exec.
Here's the `cvar_defaults.cfg` that we ship with P2CE:

```c
// client
cl_csm_auto_entity 0
cl_detaildist 1024
cl_detailfade 400
fov_viewmodel 54

// hud
hud_fastswitch 0

// mouse defaults
m_customaccel 0
m_customaccel_scale 0.04
m_customaccel_max 0
m_customaccel_exponent 1.3

// materialsystem
mat_accelerate_adjust_exposure_down 3
mat_vignette_enable 0

// server
sv_friction 4
sv_stopspeed 100
sv_accelerate 10
sv_allowupload 1
sv_alternateticks 1
sv_air_max_wishspeed 60
sv_phys_props_block_movers 1
sv_allow_legacy_cmd_execution_from_client 1
sv_client_keyvalues_data_ratelimit_bytes 8192
sv_airaccelerate 10

// scene
scene_useactorpitch 0

// render
r_physpropstaticlighting 0
r_sequence_old_order 1
r_portal_fastpath 0

// misc
zoom_sensitivity_ratio_joystick 0.5
zoom_sensitivity_ratio_mouse 0.5
sv_max_allowed_net_graph 2

locator_background_border_color 268435456
locator_background_border_thickness 3
locator_background_color 100663296
locator_background_style 0
locator_lerp_rest 2
locator_start_at_crosshair 0
locator_target_offset_x 0
locator_target_offset_y 0

// Enable current selected paint hud
cl_hud_paint_gun_powers_indicator_show_current 1

// Discord rich presence
cl_richpresence_discord_client_id 747154846817452045
cl_richpresence_enable 1

// Temorary testing to gather feedback from testers
portal_clone_displacements 1

//
// All lines below here are temporary fixes to avoid problematic codepaths
//

// Force full depth pass to avoid buggy depth resolve on ATI/Intel in dx9. No noticeable performance change.
mat_resolveFullFrameDepth 2

// Prevent blobulator from using matsys thread for drawing, causes deadlocking. No noticeable performance change.
r_threaded_blobulator 0

```