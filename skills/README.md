# TFK Skills

Team-specific Claude Code skills (slash commands) for Telemark Fylke.

## What is a skill?

A skill is a Markdown file that Claude Code loads when you invoke it with `/skill-name`. Skills encode team workflows — things like "how we do code review", "how we debug", or "how we create a new service".

## Installing a skill

Copy the skill file to your local Claude skills directory:

```bash
cp skills/<skill-name>.md ~/.claude/skills/
```

After copying, the skill is available as `/<skill-name>` in any Claude Code session.

## Writing a skill

Create a new `.md` file in this folder. Use this frontmatter at the top:

```markdown
---
name: my-skill-name
description: One-line description of what this skill does and when to use it
---

# Skill title

Instructions for Claude go here...
```

**Tips:**
- Name the file the same as the `name` frontmatter field
- The `description` is shown in skill listings — make it clear when to trigger the skill
- Write the skill body as instructions *to Claude*, not documentation *about Claude*
- Keep skills focused — one workflow per skill

## Available skills

<!-- Add entries here as skills are added -->
| Skill | Description |
|-------|-------------|
| *(none yet — add your first skill!)* | |
