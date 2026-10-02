# Changelog

## [1.0.1] - 2026-10-01

Corrections found by checking every file against a character-level extraction of
the SRD 2.0 PDF, cross-checked with OCR of the page images and the PDF layout.

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
  item's name. For example, Minor Health Potion read "**Potion** Clear 1d4 HP."
- **Text from the wrong place.** 11 entries ended with a table header or the next section's
  heading and intro, including Thistlebow, Fusion Gloves, Belt of Unity, Augur’s Relic and Stardrop.
- **Broken paragraphs.** 53 paragraphs and list items were split in two mid-sentence
  (for example, Arcana-touched, the ancestry descriptions, the Duality Dice outcomes in Core Mechanics).
- **Markdown and spacing.** 48 fixes: asterisks that showed up in places they didn't belong,
  two Ranger headings that did not render, stray spaces ("Staff :", "quaff s", "off -guard"),
  and leftover PDF tabs and bullets.
- **Headings.** 101 section headings were plain text, mostly in the core rules and the
  rest in Druid, Ranger, Brawler and their subclasses.
- **Tables.** 12 tables were flattened into loose lines, including Fear per scene, action difficulty tables and the Witch's commune results.
- **Emphasis.** 3 labels were missing their bold or italic, including "Core Gameplay Loop"
  and Striking Serpent's "Mark a Stress".
- **Stray text.** Making Moves ended with "ADVERSARIES AND", the first line of the next
  chapter's title.

### Added

- Improved Shadowblade, Advanced Shadowblade and Legendary Shadowblade (tiers 2–4 of the
  magic weapon tables), which were missing from the initial extraction.

### Changed

- JSON in `.build/03_json/` updated to match the corrected Markdown.

## [1.0.0] - 2026-09-30

- First release: SRD 2.0 in Markdown and JSON.