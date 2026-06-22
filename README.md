# Custom Difficulty

Custom Difficulty is a BepInEx 5 mod for Hollow Knight: Silksong that adds an in-game menu for tuning combat, survivability, rewards, movement, and challenge rules without editing configuration files by hand.

## Features

- Change base health, healing, invincibility time, incoming damage, and one-hit mode.
- Tune base damage, skill damage, Silk Spear damage, critical hits, and damage against bosses or common enemies.
- Adjust enemy and boss health, damage, speed, aggression, attack cooldowns, and boss-fight healing rules.
- Modify currency, item drops, shop prices, boss rewards, and currency lost on death.
- Customize movement speed, jump height, dash cooldown, and silk or ability costs.
- Apply built-in difficulty presets or save your own combination of settings.
- Use the menu in Portuguese (Brazil), English, Spanish, and game-language fallback modes. Non-Portuguese translations are marked as AI-created in the menu.

Some settings are marked **Experimental** because their effect can vary between enemies, bosses, or game scenes.

## Requirements

- Hollow Knight: Silksong
- BepInEx 5 for Silksong: `silksong_modding-BepInExPack_Silksong-1.0.3` or newer

No other mods are required.

## Installation

### Mod manager

Install the package through a Thunderstore-compatible mod manager. The required BepInEx package will be installed automatically.

### Manual installation

1. Install BepInEx 5 for Hollow Knight: Silksong.
2. Extract this package into the game directory.
3. Confirm that `BepInEx/plugins/CustomDifficulty/CustomDifficulty.dll` exists.
4. Start the game once so BepInEx can create the configuration file.

## Controls

- `F8`: open or close the Custom Difficulty menu.
- `WASD` or arrow keys: move through categories and settings.
- `Left` / `Right` or `A` / `D`: decrease or increase the selected value.
- `Q` / `E`, `Page Up` / `Page Down`, or `Tab`: change category.
- `Enter` or `Space`: confirm the selected action.
- `R`: restore the selected setting to its default value.
- `Shift` or `Ctrl` while changing a value: use larger adjustment steps.
- `Esc` or right mouse button: close the menu and discard unapplied changes.

The menu key can be changed in the BepInEx configuration file.

## Configuration

All gameplay options can be configured from the in-game menu. Settings are also stored by BepInEx in:

`BepInEx/config/codex.silksong.custom-difficulty.cfg`

Use the menu's **System** category to apply changes, discard drafts, reset defaults, and change the menu language.

## Compatibility

This mod patches gameplay methods with Harmony. Mods that change the same health, damage, silk, currency, drop, or movement methods may conflict. Back up save files before combining major gameplay mods.

## Author

Created by Ericky.

## Version

`2.0.0`
