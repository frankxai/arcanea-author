# Arcanea Author

> AI-native book production system — from concept to published book.

Arcanea Author turns Claude Code into a complete author's operating system with semantic memory, multi-agent orchestration, and a full publishing pipeline.

## What It Does

| Capability | How |
|-----------|-----|
| **Inception** | Brainstorm → outline → blueprint with parallel AI agents |
| **Writing** | Draft chapters with voice consistency and canon tracking |
| **Memory** | Semantic search across 200K+ words of manuscripts (memsearch + Milvus) |
| **Revision** | Seven-Pass ritual: structure → character → scene → dialogue → prose → continuity → polish |
| **Series** | Multi-book continuity management with timeline tracking |
| **Council** | Strategic advising from 5 perspectives (Vision, Craft, Voice, Strategy, Heart) |
| **Publishing** | Export to EPUB, PDF, Kindle, Web (arcanea.ai Library) |

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

## Architecture

```
┌─────────────────────────────────────────┐
│          ARCANEA AUTHOR                  │
│     (Unified Orchestrator)               │
├─────────────────────────────────────────┤
│                                          │
│  Modes:                                  │
│  inception | write | revise | memory     │
│  series | council | publish | ultra      │
│                                          │
│  Agent Team:                             │
│  ├── Master Story Architect              │
│  ├── Character Psychologist              │
│  ├── Line Editor & Voice Alchemist       │
│  ├── Developmental Editor                │
│  ├── Continuity Guardian                 │
│  ├── Research Librarian                  │
│  └── Publishing Strategist               │
│                                          │
│  Memory Stack:                           │
│  ├── memsearch (vector search)           │
│  ├── AgentDB (structured data)           │
│  └── Claude auto-memory (session)        │
│                                          │
└─────────────────────────────────────────┘
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

## Part of the Arcanea Ecosystem

Arcanea Author is one vertical of the [Arcanea creative multiverse](https://arcanea.ai):

- **Chat/Imagine** — Brainstorm with AI, generate concept art
- **Worlds** — Use Gates, Elements, and Archetypes as narrative architecture
- **Feed** — Share excerpts, discover other authors
- **OSS** — 27 repos, 35 npm packages, 54 Claude Code skills
- **Community** — Co-writing circles, beta reading
- **Academy** — Learn craft through the Ten Gates of authorship

## Voice Standards

- Elevated but accessible — mythic but practical
- Active voice, concrete imagery, earned emotion
- No AI verbal tics: "delve", "tapestry", "nestled", "myriad", "beacon"
- Each paragraph earns its place

## License

Arcanea Proprietary License v1.0 — See [LICENSE](LICENSE)

---

*"Enter seeking, leave transformed, return whenever needed."*
