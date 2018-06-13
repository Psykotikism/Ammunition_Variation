# Ammunition Variation
An improved/remade version of the following plugins:

[[L4D] Varying Ammunition Reserves](https://forums.alliedmods.net/showthread.php?t=117200)

[[L4D2] Varying Ammunition Reserves (1.5.3)](https://forums.alliedmods.net/showthread.php?t=125570)

## License
Ammunition Variation: a L4D/L4D2 SourceMod Plugin
Copyright (C) 2017  Alfred "Crasher_3637/Psyk0tik" Llagas

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.

## About
Varies the ammunition count of guns periodically.

### What makes Ammunition Variation viable in Left 4 Dead/Left 4 Dead 2?
The plugin adds a little realism to the games by randomizing the ammunition each gun has. Nothing more, nothing less.

### New Features/Differences
- When disabled, all ammunition revert to default values.
- Enable/disable the plugin in certain game modes.
- Supports both Left 4 Dead games so it's a 2-in-1 revision of the original plugins.
- Doesn't support AtomicStryker's Gun Control plugin.
- Less code used.

### Requirements
Ammunition Variation was developed against SourceMod 1.8+.

### Installation
1. Delete files from old versions of the plugin.
2. Extract the folder inside the .zip file.
3. Place all the contents into their respective folders.
4. If prompted to replace or merge anything, click yes.
5. Load up Ammunition Variation.
  - Type ```sm_rcon sm plugins load ammunition_variation``` in console.
  - OR restart the server.
6. Customize Ammunition Variation (Config file generated on first load).

### Uninstalling/Upgrading to Newer Versions
1. Delete ammunition_variation.smx from addons/sourcemod/plugins folder.
2. Delete ammunition_variation.sp from addons/sourcemod/scripting folder.
3. Delete ammunition_variation.cfg from cfg/sourcemod folder.
4. Follow the Installation guide above. (Only for upgrading to newer versions.)

### Disabling
1. Move ammunition_variation.smx to plugins/disabled folder.
2. Unload Ammunition Variation.
  - Type ```sm_rcon sm plugins unload ammunition_variation``` in console.
  - OR restart the server.

## Configuration Variables (ConVars/CVars)
```
// Maximum ammo count for Assault rifles.
// -
// Default: "360"
av_assaultrifle_max "360"

// Minimum ammo count for Assault rifles.
// -
// Default: "180"
av_assaultrifle_min "180"

// Maximum ammo count for Automatic shotguns.
// -
// Default: "90"
av_autoshotgun_max "90"

// Minimum ammo count for Automatic shotguns.
// -
// Default: "45"
av_autoshotgun_min "45"

// The ammunition count for guns change every time this many seconds passes.
// -
// Default: "60.0"
av_changedelay "60.0"

// Disable the plugin in these game modes.
// (Empty: None)
// (Not empty: Disabled in these game modes, separated by commas with no spaces.)
// -
// Default: ""
av_disabledgamemodes ""

// Enable the plugin?
// (0: OFF)
// (1: ON)
// -
// Default: "1"
av_enable "1"

// Enable the plugin in these game modes.
// (Empty: All)
// (Not empty: Enabled in these game modes, separated by commas with no spaces.)
// -
// Default: ""
av_enabledgamemodes ""

// Maximum ammo count for Grenade launchers.
// -
// Default: "10"
av_grenadelauncher_max "10"

// Minimum ammo count for Grenade launchers.
// -
// Default: "5"
av_grenadelauncher_min "5"

// Maximum ammo count for Hunting rifles.
// -
// Default: "150"
av_huntingrifle_max "150"

// Minimum ammo count for Hunting rifles.
// -
// Default: "80"
av_huntingrifle_min "80"

// Maximum ammo count for M60s.
// -
// Default: "150"
av_m60_max "150"

// Minimum ammo count for M60s.
// -
// Default: "80"
av_m60_min "80"

// Maximum ammo count for Shotguns.
// -
// Default: "56"
av_shotgun_max "56"

// Minimum ammo count for Shotguns.
// -
// Default: "28"
av_shotgun_min "28"

// Maximum ammo count for SMGs.
// -
// Default: "480"
av_smg_max "480"

// Minimum ammo count for SMGs.
// -
// Default: "240"
av_smg_min "240"

// Maximum ammo count for Sniper rifles.
// -
// Default: "180"
av_sniperrifle_max "180"

// Minimum ammo count for Sniper rifles.
// -
// Default: "90"
av_sniperrifle_min "90"
```

## Questions You May Have
> If you have any questions that aren't addressed below, feel free to message me or post on this [thread](https://forums.alliedmods.net/showthread.php?t=308211).

1. How do I enable/disable the plugin in certain game modes?
You must specify the game modes in the av_enabledgamemodes and av_disabledgamemodes convars.

Here are some scenarios and their outcomes:
- Scenario 1
```
av_enabledgamemodes "" // The plugin is enabled in all game modes.
av_disabledgamemodes "coop" // The plugin is disabled in Campaign mode.

Outcome: The plugin works in every game mode except in Campaign mode.
```
- Scenario 2
```
av_enabledgamemodes "coop" // The plugin is enabled in only Campaign mode.
av_disabledgamemodes "" // The plugin is not disabled at all.

Outcome: The plugin works only in Campaign mode.
```
- Scenario 3
```
av_enabledgamemodes "coop,versus" // The plugin is enabled in only Campaign and Versus modes.
av_disabledgamemodes "coop" // The plugin is disabled in Campaign mode.

Outcome: The plugin works only in Versus mode.
```

# Contact Me
If you wish to contact me for any questions, concerns, suggestions, or criticism, I can be found here:
- [AlliedModders Forum](https://forums.alliedmods.net/member.php?u=181166)
- [Steam](https://steamcommunity.com/profiles/76561198056665335)

# 3rd-Party Revisions Notice
If you would like to share your own revisions of this plugin, please rename the files! I do not want to create confusion for end-users and it will avoid conflict and negative feedback on the official versions of my work. If you choose to keep the same file names for your revisions, it will cause users to assume that the official versions are the source of any problems your revisions may have. This is to protect you (the reviser) and me (the developer)! Thank you!

# Donate
- [Donate to SourceMod](https://www.sourcemod.net/donate.php)

Thank you very much! :)
