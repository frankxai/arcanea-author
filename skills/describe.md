---
description: "Generate five sensory expansions (sight, sound, smell, taste, touch) for any scene element"
thinking: true
---

# Describe — Sensory Expansion Tool

You are now in **Describe Mode** — generating concrete, specific sensory detail for a scene element. This is the Arcanea equivalent of Sudowrite's Describe tool: five senses, no abstraction, no AI filler.

## Input

**Scene element:** $ARGUMENTS

If no arguments provided, ask:

> Give me a moment, object, place, or sensation. I will expand it across all five senses — sight, sound, smell, taste, touch — with concrete, specific detail.

## Execution Protocol

### Step 1: Canon Check (Arcanea Content Only)

If the element references Arcanea universe content (Gates, Guardians, Elements, locations):
- Read `.arcanea/lore/CANON_LOCKED.md` for canonical facts
- Search `book/` for existing descriptions of this element
- Align sensory detail with the element's canonical associations

**Element-Sense Mapping** (use as starting palette, not constraint):

| Element | Dominant Senses | Signature Materials |
|---------|----------------|---------------------|
| Fire | Sight (light, color), Touch (heat) | Gold, copper, ember, obsidian |
| Water | Sound (flow), Touch (wet, cool) | Silver, crystal, pearl, tide-worn stone |
| Earth | Touch (texture, weight), Smell (soil) | Stone, wood, moss, iron, clay |
| Wind | Sound (whisper, howl), Touch (pressure) | Feather, silk, glass, mist |
| Void | Taste (absence), Touch (numbness) | Onyx, ink, velvet, starless cloth |
| Spirit | Sight (luminance), Sound (resonance) | White gold, diamond, aurora, breath |

### Step 2: Generate Five Expansions

For the given element, produce exactly five sensory descriptions:

```markdown
## [Element Name] — Sensory Expansion

**Sight** — [1-2 sentences. What does it look like? Color, movement, light, shadow, shape.]

**Sound** — [1-2 sentences. What does it sound like? Volume, texture, rhythm, what it resembles.]

**Smell** — [1-2 sentences. What does it smell like? Sharp, sweet, metallic, organic? What memory does it evoke?]

**Taste** — [1-2 sentences. What would it taste like, or what taste does the air carry? Can be metaphorical if the element is not edible.]

**Touch** — [1-2 sentences. What does it feel like against skin? Temperature, texture, pressure, weight.]
```

### Step 3: Bonus Expansion (Optional)

If the element is rich enough, add one of these:

- **Sixth Sense** — The feeling it creates in the body. Dread, warmth, vertigo, calm. Not emotion — physical sensation.
- **Memory** — What this element reminds you of. A single, sharp associative image.
- **Absence** — What you would notice if this element were suddenly gone.

## Quality Standards

### ALWAYS
- Concrete nouns over abstract ones ("cedar smoke" not "pleasant aroma")
- Specific verbs ("hissed", "pooled", "crackled" not "was" or "seemed")
- Unexpected but accurate comparisons ("the light had the texture of old linen")
- Sensory detail that does double duty — reveals character, mood, or world alongside sensation
- Active constructions

### NEVER
- "Delve", "tapestry", "nestled", "myriad", "beacon", "symphony of"
- Purple prose or overwriting — every word earns its place
- Generic descriptions that could apply to anything ("a beautiful sight")
- Synesthesia cliches ("loud colors", "sharp silence") unless genuinely earned
- Lists of adjectives without grounding nouns

### Voice
- Elevated but accessible
- Precise but not clinical
- Sensual but not overwrought
- The reader should feel the thing, not admire the description

## Examples

**Input:** "The Foundation Gate opening"

**Sight** — Stone splits along a seam that was never visible, revealing a gap of absolute darkness that swallows the torchlight whole. The edges of the crack glow the dull orange of iron fresh from the forge.

**Sound** — A low grinding, felt more than heard, like a millstone turning in the earth beneath your feet. Then silence so complete your own heartbeat becomes the loudest thing in the chamber.

**Smell** — Mineral dust and deep groundwater, the scent of caves that have never known wind. Underneath it, something older — the faint copper tang of stone that remembers being molten.

**Taste** — The air goes dry and metallic, coating the tongue like you have been chewing on a copper coin. Swallowing does nothing to clear it.

**Touch** — The floor vibrates once, a single pulse that travels up through boot leather into bone. The temperature drops three degrees in the space of a breath, and the hairs on your forearms stand.

---

**Input:** $ARGUMENTS

Generate five sensory expansions now.
