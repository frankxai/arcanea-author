---
description: "Generate a complete novella outline from a single concept — draft zero inception sprint"
thinking: true
---

# Draft Zero — Inception Sprint

You are now in **Draft Zero Mode** — generating a complete novella skeleton from a single concept in one parallel burst. This is rough, fast, and meant to be refined. Think of it as the creative equivalent of a prototype: get the shape right, polish later through the Seven-Pass revision.

## Input

**Concept:** $ARGUMENTS

If no arguments provided, ask:

> Give me a single concept, theme, or "what if" question. One sentence is enough. I will generate a complete novella outline — premise, structure, characters, beat sheet, and opening scene — in one sprint.

## Execution: Four Parallel Agents

Fire ALL four agents in a SINGLE message with MULTIPLE Task tool calls. Do NOT wait between them — launch simultaneously.

### Agent Dispatch

```
Task(subagent_type="Story Architect", prompt="[see below]")
Task(subagent_type="Character Psychologist", prompt="[see below]")
Task(subagent_type="World Architect", prompt="[see below]")
Task(subagent_type="Explore", prompt="[see below]")
```

### Agent 1: Story Architect — Structure

Build the full narrative skeleton using The Arc cycle.

**Deliver:**

```markdown
## Premise
[One paragraph. What is this story ABOUT — not plot, but meaning.]

## The Arc
- **Potential**: What exists before the story begins. The dormant seed.
- **Manifestation**: The inciting event. What comes into being.
- **Experience**: The middle. What is lived, struggled with, learned.
- **Dissolution**: What must end, break, or transform.
- **Evolved Potential**: The new state. Not a return — an evolution.

## Three-Act Structure
### Act I — Awakening (Chapters 1-3)
[Setup, inciting incident, first threshold]

### Act II — Crucible (Chapters 4-9)
[Rising action, midpoint reversal, dark night, climactic approach]

### Act III — Transformation (Chapters 10-12)
[Climax, resolution, new equilibrium]

## 12-Chapter Beat Sheet
| Ch | Title | Beat | POV | Arc Phase | Emotional Note |
|----|-------|------|-----|-----------|----------------|
| 1  |       |      |     |           |                |
| 2  |       |      |     |           |                |
| ... | ... | ... | ... | ... | ... |
| 12 |       |      |     |           |                |
```

### Agent 2: Character Psychologist — Characters

Create five Character Diamonds. Each diamond captures the essential tension that makes a character interesting.

**Deliver:**

```markdown
## Character Diamonds (5)

### [Name] — [Role]
- **Want**: What they pursue consciously
- **Need**: What they actually require (often opposite of Want)
- **Wound**: The formative injury driving their behavior
- **Lie**: The false belief they hold because of the Wound
- **Truth**: What they must learn (or refuse to learn)
- **Voice**: How they speak — cadence, vocabulary, verbal tics
- **Arc**: Where they start -> where they end (or fail to reach)

[Repeat for all 5 characters]

### Relationship Map
[How these five characters connect, conflict, and catalyze each other]
```

### Agent 3: World Architect — Setting

Build the world this story inhabits. If the concept is Arcanea-universe, align with canon. If original, create fresh.

**Deliver:**

```markdown
## World Brief

### Setting in One Image
[A single vivid image that captures the world's essence]

### Rules
[3-5 rules that make this world different. What works differently here?]

### Geography
[Key locations the story visits, with sensory anchors for each]

### Culture
[Social structures, beliefs, tensions relevant to the plot]

### Magic/Technology System
[How power works in this world — costs, limits, consequences]

### Sensory Palette
[Dominant colors, textures, sounds, smells of this world]
```

### Agent 4: Explore — Canon Verification

ONLY runs if the concept references Arcanea universe content.

**Deliver:**

```markdown
## Canon Check

### Entities Referenced
[List every Arcanea entity the concept touches]

### Canon Facts
[Relevant established facts from CANON_LOCKED.md]

### Constraints
[What the other agents MUST respect to stay canonical]

### Opportunities
[Unexplored canon territory this story could develop]
```

Search paths: `.arcanea/lore/CANON_LOCKED.md`, `book/`, `.arcanea/lore/`

If the concept is NOT Arcanea-universe, this agent returns:
```
Canon check: Not applicable — original fiction concept.
```

## After All Agents Return

### Synthesis Phase

Combine the four outputs into a single cohesive document:

```markdown
# DRAFT ZERO: [Working Title]

## Premise
[From Story Architect]

## Characters
[From Character Psychologist — condensed]

## World
[From World Architect — condensed]

## The Arc
[From Story Architect]

## 12-Chapter Beat Sheet
[From Story Architect, enriched with character arcs and world details]

## Canon Notes
[From Explore, if applicable]
```

### Opening Scene Draft

Write the first 500-800 words of Chapter 1. This is draft zero — raw, energetic, imperfect. Prioritize:
- A first line that earns the second line
- Grounding the reader in body and place (not exposition)
- Introducing the protagonist through action or perception, not description
- Establishing voice immediately
- Ending on a hook that pulls into Chapter 2

### Quality Standards for Draft Zero

This is NOT a polished outline. It IS:
- **Fast** — generated in one burst, not agonized over
- **Complete** — every structural element present, even if rough
- **Honest** — marks uncertainty with [TBD] rather than papering over gaps
- **Alive** — characters have contradictions, the plot has genuine tension
- **Refinable** — ready for the Seven-Pass revision (structural, character, scene, dialogue, prose, continuity, polish)

This is NOT:
- **Final** — it will change significantly
- **Detailed** — scenes are beats, not full outlines
- **Perfect** — rough edges are features, not bugs

## Voice Rules

- No "delve", "tapestry", "nestled", "myriad", "beacon"
- Active voice, specific verbs, concrete nouns
- Elevated but accessible — mythic but grounded
- Every sentence earns its place

## Begin

Fire all four agents NOW with the concept: $ARGUMENTS
