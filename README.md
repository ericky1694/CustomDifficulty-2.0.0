# Custom Difficulty

Custom Difficulty is a BepInEx 5 mod for Hollow Knight: Silksong that adds an in-game difficulty menu. It lets players tune combat, survivability, rewards, movement, presets, mutators, and challenge rules without editing configuration files by hand.

## Features

- Tune player health, healing, invincibility time, incoming damage, and one-hit mode.
- Tune Hornet damage, skill damage, Silk Spear damage, critical hits, and damage against bosses or common enemies.
- Adjust enemy and boss health and damage through safe damage-scaling hooks.
- Configure experimental shop prices, boss rewards, boss profiles, randomized enemy health, and boss-pressure mutators.
- Save, load, duplicate, rename, delete, reset, import, and export readable JSON presets.
- Use a live difficulty summary with an estimated rating: Very Easy, Easy, Normal, Hard, Extreme, or Chaotic.
- Compare each option with its default value, difference, supported range, status, and description.
- Mark options as favorites and search options by name, description, or category.
- Use special mutators such as No Healing, Double Damage, Glass Cannon, Rich World, Poor World, No Mercy, Boss Frenzy, and Extended Fights.
- Use the menu in Portuguese (Brazil), English, Spanish, French, German, Italian, Russian, Japanese, Korean, Simplified Chinese, and Traditional Chinese. Non-Portuguese translations are marked as AI-made in the menu.

Some settings are marked **Experimental** or **Reserved**. Experimental settings use safe hooks or heuristics and may vary by enemy, boss, shop, or scene. Reserved settings are saved in config and presets, but do not use active gameplay hooks yet.

## Requirements

- Hollow Knight: Silksong
- BepInEx 5 for Silksong: `silksong_modding-BepInExPack_Silksong-1.0.3` or newer

No other mods are required.

## Installation

### Mod Manager

Install the package through a Thunderstore-compatible mod manager. The required BepInEx package will be installed automatically.

### Manual Installation

1. Install BepInEx 5 for Hollow Knight: Silksong.
2. Extract this package into the game directory.
3. Confirm that `BepInEx/plugins/CustomDifficulty/CustomDifficulty.dll` exists.
4. Start the game once so BepInEx can create the configuration and preset folders.

## Controls

- `F8`: open or close the Custom Difficulty menu.
- `WASD` or arrow keys: move through categories and settings.
- `Left` / `Right` or `A` / `D`: decrease or increase the selected value.
- `Q` / `E`, `Page Up` / `Page Down`, or `Tab`: change category.
- `Enter` or `Space`: confirm the selected action.
- `R`: restore the selected setting to its default value.
- `F`: add or remove the selected option from Favorites.
- `/`: focus the search box.
- `Shift` or `Ctrl` while changing a value: use larger adjustment steps.
- `Esc` or right mouse button: close the menu and discard unapplied changes.

The menu key can be changed in the BepInEx configuration file.

## Presets

Saved presets are stored as readable JSON files in:

`BepInEx/config/CustomDifficulty/presets/`

The mod also creates:

- `BepInEx/config/CustomDifficulty/presets/imports/`
- `BepInEx/config/CustomDifficulty/presets/exports/`

To export a preset, tune the draft in the menu, enter a preset name, then use **Export Current** in the Presets category. To import a preset, put a `.json` file in the `imports` folder and use **Import Latest**.

Missing fields are filled with defaults. Unknown fields are ignored. Invalid JSON is rejected without crashing the game.

## Boss Profiles

The mod creates this editable file:

`BepInEx/config/CustomDifficulty/boss-profiles.json`

Boss Profiles are experimental. Enabled profiles are matched by internal object or component names when possible. When a boss is matched, the profile can affect boss health scaling, boss damage, and Hornet damage against that boss. Speed and healing fields are stored for future safer hooks.

## Configuration

All gameplay options can be configured from the in-game menu. Settings are also stored by BepInEx in:

`BepInEx/config/codex.silksong.custom-difficulty.cfg`

## Compatibility

This mod patches gameplay methods with Harmony. Mods that change the same health, damage, silk, currency, drop, shop, or movement methods may conflict.

The mod avoids unsafe permanent save edits. It stores its own configuration, presets, boss profiles, and safe base-health tracking data under the BepInEx config folder.

Back up save files before combining major gameplay mods.

## Author

Created by Erick.

## Version

`2.1.0`
