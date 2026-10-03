# Changelog

## [1.0.2] - 2026-10-03

The repo now covers the whole SRD 2.0 rules text, and it is rebuilt directly from the PDF with
the 1.0.1 corrections made by the build itself. The rebuild also found and fixed the errors
listed under Fixed.

### Added

- **Using Adversaries** (`core_rules/Using Adversaries.md`, pages 93 to 96): the parts of an
  adversary stat block, the adversary types, example experiences and features, building balanced
  encounters with Battle Points, the stat block benchmarks by tier, and the list of adversaries by tier.
- **Using Environments** (`core_rules/Using Environments.md`, pages 158 and 159): the parts of an
  environment stat block, adapting environments to another tier, the benchmarks by tier, and the
  list of environments by tier.
- **Additional GM Guidance** (`core_rules/Additional GM Guidance.md`, pages 183 and 184): story beats,
  combat encounters, session rewards, the table of random combat objectives, downtime and projects,
  and the introduction to campaign frames.
- **The Witherwild campaign frame** (`campaign_frames/The Witherwild.md`, pages 184 to 189), in a new
  `campaign_frames/` folder with `campaign_frames.json`.
- **Supplemental Campaign Mechanics** (`core_rules/Supplemental Campaign Mechanics.md`, pages 190
  to 205): faction tracking, Everyday Hero starting equipment, feasts, and the grimdark,
  tech-based, western, colossal adversary, floating magic school, fairy tale, monster hunting and
  hex crawl campaign options, with all 17 of their tables.
- `core_rules.json` has a record for each of the four new rules files.

### Changed

- The README no longer lists these sections as left out, and LICENSE.md no longer says the repo
  leaves out parts of the SRD.

### Fixed

- **Double spaces after "ff".** 21 places in 18 files had two spaces after a word ending in
  "ff", left by the PDF's ligature glyphs: "Bite off  heads", "staff  member", "sniff  out" and
  others in adversaries and environments, with the same text in `adversaries.json` and
  `environments.json`.
- **Class connection questions.** In `classes.json`, the Druid and Ranger `connection` lists
  held rules text after the three questions: the Beastform options for the Druid and the
  companion rules for the Ranger. Each list now holds only its three questions.
- **Druid in `classes.json`.** The Wildtouch feature text began with four stray asterisks.
- **Headings that were plain text or italics.** Core Gameplay Loop, The Spotlight and Turn Order &
  Action Economy in Core Mechanics are now headings like the other sections in their font, as is
  Overplanning in GM Guidance. In Brawler and Martial Artist, the TIER 1 to TIER 4 stance labels
  are now headings. In Ranger and Wayfinder, Using Spellcast Rolls, Hope, and Experiences and
  Attacking with Your Companion are now headings, like the other companion sections.
- **List spacing in four domain cards.** Blighting Strike, Codex-touched, Death Grip and Force of
  Nature had a blank line between their list items. They now match the other domain cards.
- **Mixed Ancestry in `ancestry_rules.json`.** The text under each numbered step is now indented
  to match the Markdown.

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