---
description: "Auto-surface canon references when character/location names appear in text — Codex linking"
thinking: true
---

# Codex Link — Canon Auto-Surface

You are now in **Codex Link Mode** — automatically detecting and annotating every canon entity in the provided text. This is the Arcanea equivalent of NovelCrafter's Codex linking: no entity goes unverified.

## Input

**Text to scan:** $ARGUMENTS

If no arguments provided, ask:

> Paste a passage, scene, or outline. I will scan every name, location, and canon term and annotate it with established facts from the source files.

## Execution Protocol

### Step 1: Entity Detection

Read the provided text and extract ALL potential canon entities:

- **Character names** — Gods/Goddesses, Godbeasts, Luminors, Malachar, Lumina, Nero, Eldrians, Academy figures
- **Location names** — Shadowfen, Academy Houses, Gate names, realms, territories
- **Canon terms** — Elements (Fire, Water, Earth, Wind, Void, Spirit, Shadow), Gates, Frequencies, Magic Ranks, The Arc, Divine Bonds
- **Arcanea-specific vocabulary** — Arcane, Song, Mana, Anima, Vel'Tara, Starweave

### Step 2: Source Lookup (Priority Order)

For EACH detected entity, search these sources in order. Stop at the first authoritative hit:

1. **Primary**: `.arcanea/lore/CANON_LOCKED.md` — immutable truth
2. **Secondary**: `book/` — Library content (narrative detail, characterization)
3. **Tertiary**: `.arcanea/lore/` — gods-goddesses/, godbeasts/, guardians/, metadata.yaml
4. **Quaternary**: `apps/web/lib/` — config files, type definitions

Use Grep to search each source. For character names, also check alternate spellings and titles.

### Step 3: Annotation Output

Return the text with inline annotations. Format:

```
[EntityName] -> "established fact" (source: relative/path:line)
```

Group annotations by category:

```markdown
## Characters Found
- [Lyssandria] -> "God/Goddess of the Foundation Gate, 174 Hz, Earth/survival domain" (source: .arcanea/lore/CANON_LOCKED.md:42)
- [Kaelith] -> "Godbeast bonded to Lyssandria, Foundation Gate guardian" (source: .arcanea/lore/CANON_LOCKED.md:42)

## Locations Found
- [Shadowfen] -> "Where Malachar is sealed after his fall" (source: .arcanea/lore/CANON_LOCKED.md:89)

## Canon Terms Found
- [Starweave] -> "8th Gate, 852 Hz, Elara + Vaelith, perspective/transformation" (source: .arcanea/lore/CANON_LOCKED.md:49)

## Potential Issues
- [Thessara] -> WARNING: Non-canonical name. Canonical Godbeast for 8th Gate is Vaelith.
- [714 Hz] -> WARNING: Non-canonical frequency. Crown Gate is 741 Hz.
```

### Step 4: Consistency Report

After annotations, provide a summary:

```markdown
## Codex Link Summary
- Entities found: X
- Canon-verified: Y
- Warnings: Z
- Unknown entities: W (may be new — not in canon)
```

## Canon Quick Reference (for detection)

### Names to Watch
Gods/Goddesses: Lyssandria, Leyla, Draconia, Maylinn, Alera, Lyria, Aiyami, Elara, Ino, Shinkami
Godbeasts: Kaelith, Veloura, Draconis, Laeylinn, Otome, Yumiko, Sol, Vaelith, Kyuro, Source
Cosmic: Lumina, Nero, Malachar (Lumenbright)
Houses: Lumina, Nero, Pyros, Aqualis, Terra, Ventus, Synthesis

### Frequencies (must be exact)
174, 285, 396, 417, 528, 639, 741, 852, 963, 1111

### Common Errors to Flag
- "Shift" instead of "Starweave" (8th Gate)
- "Amaterasu" instead of "Source" (10th Godbeast)
- "Thessara" instead of "Vaelith" (8th Godbeast)
- 714 Hz instead of 741 Hz (Crown)
- Nero described as evil (Nero is NOT evil — Shadow is corrupted Void)
- "Light" as an element (Light is Fire's creation aspect)
- Maylinn with wrong element (Air, Heart Gate, 417 Hz)

## Rules

- NEVER fabricate canon facts. If an entity is not found in sources, say "Not in canon — may be new."
- ALWAYS read CANON_LOCKED.md before processing.
- Flag contradictions, do not silently correct them. The author decides.
- Include line numbers when possible for easy verification.
- If the text is not Arcanea-universe content, skip canon checks and note that entities appear to be original fiction.

## Begin

Scan the provided text now. Read CANON_LOCKED.md first, then detect, search, and annotate.
