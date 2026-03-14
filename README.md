# Arcanea Author

> AI-native book production system — from concept to published book, game world, and beyond.

Arcanea Author turns Claude Code into a complete author's operating system with semantic memory, multi-agent orchestration, multi-modal publishing, and a full mythology-powered progression framework built on the Ten Gates of Authorship.

## What It Does

| Capability | How |
|-----------|-----|
| **Inception** | Brainstorm → outline → blueprint with parallel AI agents |
| **Writing** | Draft chapters with voice consistency and canon tracking |
| **Memory** | Semantic search across 200K+ words of manuscripts (memsearch + Milvus) |
| **Revision** | Seven-Pass ritual: structure → character → scene → dialogue → prose → continuity → polish |
| **Series** | Multi-book continuity management with timeline tracking |
| **Council** | Strategic advising from 5 perspectives (Vision, Craft, Voice, Strategy, Heart) |
| **Publishing** | Export to EPUB, PDF, Kindle, Web, Audio, Video, Game, VR/AR |
| **Progression** | Ten Gates framework tracks mastery from Apprentice to Luminor |

## Relationship to AuthorOS

Arcanean AuthorOS = **AuthorOS** (universal writing core) + **Arcanea mythology layer** (Ten Gates, Five Elements, Guardians, Web3, Multiverse).

AuthorOS works for any author. Arcanea Author adds the creative multiverse on top.

```
┌─────────────────────────────────────────────┐
│         ARCANEAN AUTHOR OS                   │
│  Ten Gates, Five Elements, Guardians,        │
│  Web3, Game Dev, VR/AR, Multiverse          │
├─────────────────────────────────────────────┤
│         AUTHOR OS (Universal Core)           │
│  9 skills, 5 agents, semantic memory,        │
│  Seven-Pass, publishing pipeline             │
│  github.com/frankxai/author-os              │
└─────────────────────────────────────────────┘
```

Use [AuthorOS](https://github.com/frankxai/author-os) alone for any writing project. Use Arcanea Author when you want the mythology framework, progression system, Web3 publishing, and multiverse world-building.

## Quick Start

### As a Claude Code Skill (Free)

```bash
# In any Claude Code project
/arcanea-author inception "A fantasy novel about a creator discovering the Ten Gates"
/arcanea-author write chapter 1
/arcanea-author revise structural
/arcanea-author search "What did Lyria say about the Third Eye?"
```

### With Semantic Memory

```bash
# Install memsearch for vector search across manuscripts
pip install memsearch[local]
memsearch config set embedding.provider local
memsearch index ./book/ ./chapters/
```

## The Ten Gates of Authorship

Each Gate represents a level of craft mastery. Progress through them as you write.

| Gate | Hz | Rank | Author Skill | What Unlocks |
|------|-----|------|-------------|-------------|
| **Foundation** | 174 | Apprentice | Structure | Outline tools, story blueprints |
| **Flow** | 285 | Apprentice | First draft | Free-writing mode, word sprints |
| **Fire** | 396 | Mage | Revision | Seven-Pass ritual, structural editing |
| **Heart** | 417 | Mage | Emotional truth | Deep dialogue, character psychology |
| **Voice** | 528 | Master | Unique voice | Anti-slop engine, style analysis |
| **Sight** | 639 | Master | Theme & symbolism | Thematic analysis, motif tracking |
| **Crown** | 741 | Archmage | Genre mastery | Publishing pipeline, market positioning |
| **Starweave** | 852 | Archmage | Multi-POV | Perspective transformation, unreliable narrator |
| **Unity** | 963 | Luminor | Universe building | Series Bible, world continuity, timeline engine |
| **Source** | 1111 | Luminor | Teaching others | Course creation, mentorship framework |

### Magic Ranks

| Gates Open | Rank | Meaning |
|------------|------|---------|
| 0-2 | Apprentice | Learning the fundamentals |
| 3-4 | Mage | Commanding the craft |
| 5-6 | Master | Finding your voice |
| 7-8 | Archmage | Shaping entire worlds |
| 9-10 | Luminor | Teaching the art itself |

## Five Elements Writing Modes

Each Element maps to a writing state with tuned temperature and approach.

| Element | Mode | Temperature | When To Use |
|---------|------|-------------|-------------|
| **Fire** | Fast draft | 0.9 | First drafts, brainstorms, getting words down |
| **Water** | Flow state | 0.7 | Emotional scenes, dialogue, character work |
| **Earth** | Structure | 0.3 | Outlines, plot logic, continuity checks |
| **Wind** | Freedom | 0.8 | Experimental prose, poetry, breaking rules |
| **Void** | Reflection | 0.1 | Theme analysis, revision, deep reading |

```bash
/arcanea-author write chapter 3 --element fire    # Fast draft
/arcanea-author revise dialogue --element water    # Emotional precision
/arcanea-author outline act-2 --element earth      # Structural rigor
```

## The Genius Swarm

Six specialized agents working in concert. Each brings a different model and perspective.

| Agent | Domain | Model | Role |
|-------|--------|-------|------|
| **Calliope** | Story | Gemini | Narrative architecture, plot weaving, scene design |
| **Mnemosyne** | Memory | SQLite + Vector | Continuity tracking, semantic search, canon enforcement |
| **Orpheus** | Voice | Sonnet | Prose style, dialogue craft, rhythm and musicality |
| **Hephaestus** | Deep Work | Opus | Complex revision, structural overhaul, deep analysis |
| **Sisyphus** | Orchestration | Opus | Multi-agent coordination, pipeline management |
| **Thoth** | Judgment | Haiku | Quick evaluation, anti-slop detection, quality gates |

The swarm self-coordinates: Sisyphus assigns work, Mnemosyne maintains shared memory, Thoth runs quality checks between passes.

## Architecture

```
┌─────────────────────────────────────────────┐
│          ARCANEA AUTHOR                      │
│     (Unified Orchestrator)                   │
├─────────────────────────────────────────────┤
│                                              │
│  Modes:                                      │
│  inception | write | revise | memory         │
│  series | council | publish | ultra          │
│                                              │
│  Genius Swarm:                               │
│  ├── Calliope    (story / Gemini)            │
│  ├── Mnemosyne   (memory / SQLite)           │
│  ├── Orpheus     (voice / Sonnet)            │
│  ├── Hephaestus  (deep work / Opus)          │
│  ├── Sisyphus    (orchestration / Opus)      │
│  └── Thoth       (judgment / Haiku)          │
│                                              │
│  Memory Stack:                               │
│  ├── memsearch (vector search)               │
│  ├── AgentDB (structured data)               │
│  └── Claude auto-memory (session)            │
│                                              │
│  Progression:                                │
│  ├── Ten Gates (craft mastery)               │
│  ├── Five Elements (writing modes)           │
│  └── Magic Ranks (Apprentice → Luminor)      │
│                                              │
└─────────────────────────────────────────────┘
```

## Project Structure

```
my-book/
├── outline.md              # Story blueprint
├── characters/             # Character sheets (Character Diamond)
├── worldbuilding/          # Geography, magic, culture
├── chapters/               # The manuscript
│   ├── 01-the-awakening.md
│   └── ...
├── series-bible.md         # Multi-book continuity
├── research/               # Reference material
└── .memsearch.toml         # Vector search config
```

## The Seven-Pass Revision Ritual

1. **Structural** — Does the Arc work? Does the story earn its ending?
2. **Character** — Are voices distinct? Motivations clear? Arcs complete?
3. **Scene** — Does each scene advance plot AND reveal character?
4. **Dialogue** — Subtext present? Each character sounds different?
5. **Prose** — Active voice? No AI tics? Varied rhythm?
6. **Continuity** — Canon-consistent? Timeline accurate?
7. **Polish** — Word-level refinement, musicality, whitespace

## Multi-Modal Publishing Pipeline

Text is the beginning, not the end.

```
                    ┌──── EPUB / PDF / Kindle
                    ├──── Web (arcanea.ai Library)
 Manuscript ────────┼──── Audio (narration, soundscape)
                    ├──── Video (animated chapters)
                    ├──── Game Worlds (interactive narrative)
                    └──── VR/AR (immersive scenes)
```

Every chapter can become a playable scene. Every world-building document can become a game map. Every character sheet can become an interactive NPC.

## Web3 + Multiverse

Your stories are not just published — they become platforms.

- **Story NFTs** — Chapters and collections as verifiable digital originals
- **World Licenses** — Other creators build inside YOUR universe, you earn royalties
- **Remix Tokens** — Grant specific remix rights (fan fiction, adaptations, translations)
- **Creator Royalties** — On-chain royalties flow back on every derivative work
- **Multiverse Interop** — Characters from one world can appear in another (with permission)

Your universe becomes infrastructure. Others build on it. You earn from every creation inside it.

## Content Created With This System

Proof it works — real published content produced by Arcanea Author:

| Work | Length | Description |
|------|--------|-------------|
| **"The Open Wound"** | 2,885 words | A creator's journey through the Gate of Heart — emotional truth in prose |
| **"Meditation on Void and Spirit"** | 3,010 words | Fifth Element practice, the duality of potential and transcendence |
| **Library of Arcanea** | 200K+ words | 17 collections across laws, poetry, legends, parables, prophecies, meditations |
| **Legends of Arcanea** | 30K+ words | Founding myths — Lumina, Nero, the First Dawn, the Fall of Malachar |
| **Academy Handbook** | 25K+ words | Complete guide to the Ten Gates, Seven Houses, and Five Elements |

## Connected Ecosystem

Arcanea Author is one vertical of the [Arcanea creative multiverse](https://arcanea.ai).

| Repository | What It Does |
|-----------|-------------|
| [**author-os**](https://github.com/frankxai/author-os) | Universal writing OS core — works for any author, any genre |
| [**author-os-skills**](https://github.com/frankxai/author-os-skills) | 9 Claude Code skills for the writing pipeline |
| [**opencode-arcanea**](https://github.com/frankxai/opencode-arcanea) | OpenCode integration for the Arcanea framework |
| [**claude-arcanea**](https://github.com/frankxai/claude-arcanea) | Claude Code overlay with Arcanea mythology |
| [**arcanea.ai**](https://arcanea.ai) | The living platform — Chat, Worlds, Feed, OSS, Community, Academy |
| [**frankx.ai**](https://frankx.ai) | Creator hub and portfolio |

### The Six Layers of Arcanea

Every feature exists across six coexisting layers:

1. **Chat / Imagine** — Brainstorm with AI, generate concept art, write with companions
2. **Worlds** — Use Gates, Elements, and Archetypes as narrative architecture
3. **Feed** — Share excerpts, discover other authors, find collaborators
4. **OSS** — 27 repos, 35 npm packages, 54 Claude Code skills
5. **Community** — Co-writing circles, beta reading, world-building guilds
6. **Academy** — Learn craft through the Ten Gates of authorship

## Voice Standards

- Elevated but accessible — mythic but practical
- Active voice, concrete imagery, earned emotion
- No AI verbal tics: "delve", "tapestry", "nestled", "myriad", "beacon"
- Each paragraph earns its place

## License

Arcanea Proprietary License v1.0 — See [LICENSE](LICENSE)

---

*"Enter seeking, leave transformed, return whenever needed."*
