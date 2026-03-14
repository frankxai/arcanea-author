# Arcanea Author — Competitive Analysis (March 2026)

## The Competitive Landscape

### Commercial Platforms

| Platform | Price | Key Features | What They Lack |
|----------|-------|-------------|----------------|
| **Sudowrite** | $10-59/mo | Muse 1.5 (fiction-tuned), Story Bible, Describe tool | No multi-agent, no semantic search, no revision system, no publishing |
| **NovelCrafter** | $4-20/mo + BYOK | Codex wiki, 300+ models via OpenRouter, beat mapping | No built-in AI, no vector search, no revision methodology |
| **NovelAI** | ~$10-25/mo | Lorebook triggers, custom fine-tuned models, image gen | Interactive fiction focus, no structured authoring |
| **Jasper** | $49-69/mo | Brand voice training, team collab | Marketing focus, not fiction |
| **Copy.ai** | $49/mo | Workflow automation | Short-form only |

### Open-Source GitHub Repos

| Repo | Stars | Gap vs Arcanea Author |
|------|-------|----------------------|
| SillyTavern | 15K+ | Roleplay/chat, not structured authoring |
| KoboldAI/KoboldCpp | 6K+ | Text gen engine, no orchestration |
| GOAT-Storytelling-Agent | ~500 | Multi-stage but fully autonomous, no human-in-loop |
| KazKozDev/NovelGenerator | ~300 | Multi-agent but no memory, no revision |
| raestrada/storycraftr | ~200 | CLI worldbuilding, single-agent |
| MetaGPT | 50K+ | Software agents pattern (not writing-tuned) |

## Capability Matrix

| Capability | Sudowrite | NovelCrafter | NovelAI | SillyTavern | GOAT | **Arcanea Author** |
|-----------|-----------|-------------|---------|-------------|------|-------------------|
| Multi-agent orchestration | No | No | No | No | Partial | **12+ agents** |
| Semantic vector search | No | No | No | No | No | **2,200 chunks** |
| Canon verification | No | No | No | No | No | **CANON_LOCKED.md** |
| Revision methodology | No | No | No | No | No | **Seven-Pass** |
| Character framework | Story Bible | Codex wiki | Lorebook | WorldInfo | Basic | **Character Diamond** |
| Publishing pipeline | No | No | No | No | No | **epub/pdf/kindle/web** |
| Model-agnostic | No | Yes | No | Yes | Partial | **Yes** |
| Open-source/portable | No | No | No | Yes | Yes | **54 skills** |
| Series management | No | No | No | No | No | **Series Bible** |
| Quality gate/anti-slop | No | No | No | No | No | **9-point gate** |

## What to Absorb

| Source | Feature | How to Integrate |
|--------|---------|-----------------|
| NovelCrafter | Real-time Codex linking | Auto-surface canon when character names appear |
| Sudowrite | Sensory Describe tool | Add sensory expansion pass to revision |
| NovelAI | Lorebook trigger words | Keyword triggers for critical canon elements |
| SillyTavern | Extension ecosystem | Formalize author skill registry |
| GOAT Agent | Draft zero generation | "Inception sprint" mode |

## Market Position

Arcanea Author is the ONLY system that treats book production as an orchestrated pipeline — inception through revision through publishing — with specialized agents, semantic memory, canon verification, and quality gates. The closest analog is CI/CD for books.

At $19/month (Arcanea Creator tier), this delivers more than Sudowrite ($59/mo) and NovelCrafter ($20/mo) combined.
