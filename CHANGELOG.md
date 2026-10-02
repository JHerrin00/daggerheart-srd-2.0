# Changelog

## [1.0.1] - 2026-10-01

Corrections found by checking every file against a character-level extraction of
the SRD 2.0 PDF, cross-checked with OCR of the page images, and by comparing headings,
lists, tables and emphasis with the PDF layout.

### Fixed

- **Wrong values.** Extraction script misread these values. 
  - Minion (6): Apprentice Assassin, Conscript, Cult Initiate, Fungispunj Sporeling, Treant Sapling
  - Minion (7): Giant Recruit
  - Horde (1d6+3): Archer Squadron · Horde (1d6+1): Flock of Feather Fiends ·
    Horde (2d6+2): Night Children · Horde (2d6): Vampire Bat Swarm ·
    Horde (2d6+5): Ghastly Legion, Wyrmlings, Zombie Legion
  - Hallowed Choir: Horde (6/HP)
  - Fire Titan Warlord, Colossus Crafter: Countdown (6)
  - Burning Heart of the Woods, Choking Ash: Countdown (Loop 6)
- **Environment names.** `Workshop` is now `Alchemist’s Abandoned Workshop`, and
  `City of Portals` is now `Convergence, the City of Portals`.
- **Evolutions.** Each evolution is now its own feature, not text appended to the feature
  above it: Mountain Troll, Vampire Lord, Phoenix, Roc, Cephilith Titan, Supreme Demiurge Adonix.
- **Item and consumable descriptions.** 95 descriptions began with the last word(s) of the
  item's name.  For example, Minor Health Potion read "**Potion** Clear 1d4 HP."
- **Text from the wrong place.** 11 entries ended with a table header or the next section's
  heading and intro, including Thistlebow, Fusion Gloves, Belt of Unity, Augur’s Relic and Stardrop.
- **Broken paragraphs.** 53 paragraphs and list items were split in two mid-sentence
  (for example, Arcana-touched, the ancestry descriptions, the Duality Dice outcomes in Core Mechanics).
- **Markdown and spacing.** 48 fixes: asterisks that showed up in places they didn't belong, headings that did not render, stray spaces
  ("Staff :", "quaff s", "off -guard"), and leftover PDF tabs and bullets.
- **Headings.** 101 section headings were plain lines of text and now render as headings,
  at levels that follow the PDF's heading styles. Most are in the core rules; the rest are in
  Druid, Ranger, Brawler and their subclasses.
- **Tables.** 12 tables had been flattened into loose lines and are Markdown tables again:
  Fear per scene, the six action difficulty tables (Agility to Knowledge), dynamic countdown
  advancement and average costs in Making Moves, the Witch's commune results, the Moon Witch's
  lunar phases, and the Warlock's sphere of influence examples.
- **Emphasis.** "Core Gameplay Loop" and "Turn Order & Action Economy" are italic as printed,
  and Striking Serpent's "Mark a Stress" is bold.
- **Stray text.** Removed "ADVERSARIES AND" (the first line of the next chapter's title) from
  the end of Making Moves.

### Added

- Improved Shadowblade, Advanced Shadowblade and Legendary Shadowblade were missing from initial extraction. 

### Changed

- JSON in `.build/03_json/` updated to match the corrected Markdown.

## [1.0.0] - 2026-09-30

- First release: SRD 2.0 in Markdown and JSON.
