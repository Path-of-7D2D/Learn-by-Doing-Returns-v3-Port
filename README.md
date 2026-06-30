# Learn By Doing Returns

Learn By Doing Returns is a 7 Days To Die V3.0 XML-only port of IzPrebuilt's deprecated Learn By Doing overhaul.

It moves progression away from pure learn-by-looting pressure and back toward action-based skill growth. Combat, crafting, resource, physical, and barter skills increase as the player uses the related playstyle, while the existing magazine ecosystem is reshaped to support the new progression.

Built for **7 Days To Die V3.0 "Dead Hot Summer"**.

## Features

- Replaces the vanilla progression tree with a custom Learn By Doing progression layout.
- Adds action-skill tracking through XML buffs and CVars.
- Levels weapon skills from combat use, including melee, archery, pistols, shotguns, rifles, and automatic rifles.
- Levels utility skills from related actions, including barter, engineering, science, armor, athletics, survivalism, mining, salvaging, and scavenging.
- Reworks skill magazines into supporting books that award experience and skill progress instead of being the only path forward.
- Adds custom skill magazines for Speech, Athletics, and Scavenging.
- Rebalances loot and trader skill-magazine pools around the new categories.
- Updates recipe, block, item, trader, quest, buff, and UI display hooks needed by the overhaul.
- Ports the old skill-window layout adjustment to V3 `XUi_InGame` without replacing the full V3 skill UI.
- XML-only. No DLL required.

## Requirements

- 7 Days To Die V3.0.

Easy Anti-Cheat can stay enabled because this is an XML-only modlet.

## Installation

1. Download the latest `LearnByDoingReturns-*.zip` from the [GitHub Releases](https://github.com/Path-of-7D2D/Learn-by-Doing-Returns-v3-Port/releases) page.
2. Extract the release zip.
3. Copy the `1A-LearnByDoingReturns` folder into your `Mods` folder:

```text
7 Days To Die/Mods/1A-LearnByDoingReturns/
```

The folder is installed correctly when this file exists:

```text
7 Days To Die/Mods/1A-LearnByDoingReturns/ModInfo.xml
```

## Multiplayer

Install the mod on the server and every connecting client. This mod changes progression definitions, item definitions, loot pools, localization, icons, recipes, and skill UI behavior, so mismatched installs can cause missing items, mismatched unlocks, or inconsistent progression display.

## Compatibility

This is a broad progression overhaul and may conflict with mods that heavily change:

- `progression.xml`
- `buffs.xml`
- `items.xml`
- `loot.xml`
- `traders.xml`
- `recipes.xml`
- `blocks.xml`
- `XUi_InGame/windows.xml` skill windows

Small XML mods that add unrelated recipes or items are more likely to work, but anything that replaces the vanilla progression tree or skill magazine system should be reviewed carefully.

## Testing

1. Install `1A-LearnByDoingReturns` into the game's `Mods` folder.
2. Start or load a V3 test world.
3. Confirm the game log shows `Loaded Mod: IzPLearnByDoing (3.0.0)`.
4. Open the Skills screen and confirm the custom category list displays correctly.
5. Use several weapon and utility actions and confirm related skills can progress.
6. Check loot, trader inventories, and quest rewards for the revised skill magazine set.

## Nexus Media

Nexus-ready artwork is included under `media/nexus/`:

- `learn-by-doing-returns-header-1400x400.jpg`
- `learn-by-doing-returns-thumbnail-1920x1080.jpg`

## Releasing

The release workflow is manual. Run the `Release` GitHub Action with a `version_tag` such as `v3.0.0` or `3.0.0`.

The workflow validates the deployable `1A-LearnByDoingReturns` folder, creates a `LearnByDoingReturns-<version>.zip`, generates release notes with `Path-of-7D2D/Changelog-Generator`, and publishes the GitHub release.

## Credits

Original Learn By Doing mod by IzPrebuilt. This repository is an unofficial V3.0 maintenance port made after the original mod was deprecated and opened for community continuation.
