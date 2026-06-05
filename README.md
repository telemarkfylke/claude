# TFK Claude Configuration Library

Shared Claude Code configuration and skills for Telemark Fylke.

## What's in this repo

| Path | Purpose |
|------|---------|
| `CLAUDE.md` | Shared team instructions loaded by Claude Code in every session |
| `skills/` | Team-specific Claude skills (slash commands) |
| `config/` | Example configuration files to copy and adapt locally |

## Getting started

### 1. Copy shared config

Copy the example files to your local Claude config directory and adapt them:

```bash
cp config/settings.example.json ~/.claude/settings.local.json
cp config/keybindings.example.json ~/.claude/keybindings.json
```

### 2. Install skills

Copy any skill files you want into your local skills directory:

```bash
cp skills/<skill-name>.md ~/.claude/skills/
```

Or symlink the whole folder if you want changes to sync automatically:

```bash
ln -s $(pwd)/skills ~/.claude/skills/tfk
```

### 3. Use CLAUDE.md

For project repos, copy or symlink `CLAUDE.md` into the repo root so Claude picks up team conventions automatically:

```bash
cp CLAUDE.md /path/to/your/project/CLAUDE.md
```

## Contributing

- Add new skills to `skills/` with a descriptive name and clear frontmatter
- Keep `config/` files as examples — never commit real API keys or personal paths
- Update this README when adding new content
