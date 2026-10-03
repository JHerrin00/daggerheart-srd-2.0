# Daggerheart SRD 2.0

A Markdown and JSON version of the Daggerheart System Reference Document 2.0 (2026-08-25 release), with one file per entity. The folder layout and the JSON field names follow
[seansbox/daggerheart-srd](https://github.com/seansbox/daggerheart-srd).

## Contents

| Folder | Entries |
|---|---|
| `abilities/` | 210 domain cards |
| `adversaries/` | 264 |
| `ancestries/` | 25 |
| `ancestry_rules/` | 1 (Mixed Ancestry) |
| `armor/` | 69 |
| `beastforms/` | 24 |
| `campaign_frames/` | 1 (The Witherwild) |
| `classes/` | 13 |
| `communities/` | 15 |
| `consumables/` | 120 |
| `core_rules/` | 17 |
| `domains/` | 10 |
| `environments/` | 47 |
| `items/` | 120 |
| `subclasses/` | 26 |
| `transformations/` | 6 |
| `weapons/` | 315 (Combat Wheelchair is one file holding 12 wheelchairs) |

`.build/03_json/` contains one JSON file per category, written from the Markdown in these folders. Two details of the JSON follow from the SRD itself:

- Class records have no `suggested_armor`, `suggested_primary`, `suggested_secondary` or `suggested_traits` fields, because the SRD 2.0 class pages do not list them.
- Items and consumables each come from two loot tables (the Core Set and the Hope & Fear Expansion Set), both numbered 1 to 60, so roll numbers repeat within each category.

## Changes from the SRD text

The Markdown follows the PDF text. I have listed the places where it differs below.

**Format**

- Weapons, armor and beastforms carry a tier line to follow seansbox's format. Weapons also carry Primary or Secondary and Physical or Magical, for example `**_Tier 1_** _Primary_ _Physical_ _Weapon_`. Each value comes from the table the entry appears in. Again this was to mimic seansbox's excellent work.
- Armor stats are a bulleted list.
- Mixed Ancestry is in its own folder, `ancestry_rules/`, because it is a rules section and not one of the ancestries.
- The Witherwild campaign frame is in its own folder, `campaign_frames/`, because it is setting material and not a rules section.
- The optional weapons and armor in Supplemental Campaign Mechanics (Everyday Hero, Western and Monster Hunting equipment) stay as tables in `core_rules/Supplemental Campaign Mechanics.md`. They are not in `weapons/` or `armor/`, so the standard equipment lists stay as the SRD prints them.
- The roll options in Battle Box, Dragon Mother Mitera, Gobstalker, Supreme Demiurge Adonix, Demon Lord Berzug, Soul-Shattered Mage and Deadly Dungeon are on separate lines for readability.

**Names**

- The Witch subclasses are named Hedge Witch and Moon Witch. The SRD text says Hedge and Moon. The Witch class text markdown file matches the changes.

**Corrections**

- Typos and formatting slips from the PDF extraction are fixed, for example "terain" is now "terrain" in Terrible Lizard. The full list is in [CHANGELOG.md](CHANGELOG.md).

**Consolidations**

- The Combat Wheelchair rules and its twelve wheelchairs are one file, `weapons/Combat Wheelchair.md`, with a table for each tier.

## License & Legal

This repository includes materials from the Daggerheart System Reference Document 2.0, © Critical Role, LLC. All rights reserved. The SRD was created by Darrington Press and is licensed under the [Darrington Press Community Gaming (DPCGL) License](https://darringtonpress.com/license/). The original document is available at [daggerheart.com](https://www.daggerheart.com/).

This repository modifies the SRD. It converts the text to Markdown and JSON, corrects extraction errors, renames the Witch subclasses, and consolidates the Combat Wheelchair tables into one file. There are no previous modifications by others.

Daggerheart and all related marks are trademarks of Critical Role, LLC and used with permission. This project is unofficial. It is not affiliated with, endorsed, or sponsored by Critical Role or Darrington Press.

