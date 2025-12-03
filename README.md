# Flow

Structured AI-assisted development. Research → Plan → Implement.

## Install

**Step 1:** Add the marketplace
```bash
/plugin marketplace add stevef24/flow
```

**Step 2:** Install the plugin
```bash
/plugin install flow@stevef24/flow
```

## Commands

| Command | Purpose |
|---------|---------|
| `/flow:research` | Investigate codebase |
| `/flow:plan` | Create implementation plan |
| `/flow:implement` | Execute with checkpoints |

## Usage

```
/flow:research
> How does auth work?

/flow:plan docs/research/2025-01-15-auth.md
> Add Google OAuth

/flow:implement docs/plans/2025-01-15-oauth.md
```

## Philosophy

You are the developer. AI amplifies your judgment.

- **Research**: You investigate. AI documents.
- **Plan**: You design. AI structures.
- **Implement**: You review. AI executes.

## Agents

| Agent | Purpose |
|-------|---------|
| `codebase-researcher` | Find and document code |
| `pattern-finder` | Locate existing patterns |
| `dependency-tracer` | Trace call chains |
| `implementation-analyzer` | Propose approaches |

## Output

```
docs/
├── research/
│   └── YYYY-MM-DD-topic.md
└── plans/
    └── YYYY-MM-DD-feature.md
```

## Credits

Based on Dex Horthy's "Frequent Intentional Compaction" workflow.

## License

MIT
