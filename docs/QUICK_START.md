# Arcanea Author — Quick Start

## Option 1: Claude Code Skill (Recommended)

Copy `skills/arcanea-author.md` to your project's `.claude/commands/` directory:

```bash
cp skills/arcanea-author.md /path/to/your/project/.claude/commands/
```

Then in Claude Code:
```
/arcanea-author inception "A novel about..."
/arcanea-author write chapter 1
/arcanea-author revise
```

## Option 2: With Semantic Memory

Install memsearch for vector search across your manuscripts:

```bash
# Using uvx (recommended — no system packages)
uvx --with "memsearch[google]" memsearch index ./chapters/

# Or with pip
pip install memsearch[google]
memsearch index ./chapters/
```

Configure: copy `memory/memsearch.toml` to `.memsearch.toml` in your project root.

Set your API key:
```bash
export GOOGLE_API_KEY=your-key  # for Google embeddings
# or
export OPENAI_API_KEY=your-key  # for OpenAI embeddings
```

## Option 3: Agent Definitions

Copy agent definitions from `agents/` to `.claude/agents/` for specialized AI team members:
- **lore-master.md** — Canon keeper and narrative coordinator
- **character-crafter.md** — Character depth and dialogue
- **world-expander.md** — Locations, systems, cultures

## Your First Project

```bash
mkdir my-novel && cd my-novel
cp -r /path/to/arcanea-author/templates/novel/* .
```

Then open Claude Code and run `/arcanea-author inception`.
