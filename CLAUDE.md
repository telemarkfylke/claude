# TFK — Claude Code Team Instructions

This file is loaded automatically by Claude Code. It establishes shared conventions for all Telemark Fylke development work.

## Team context

We are developers at Telemark Fylke (TFK), a Norwegian county municipality. Our projects span multiple domains including citizen services, internal tooling, and integrations with public-sector systems.

## Tech stack

We work across a mixed stack — read the project's own README or package files before making assumptions:

- **Node.js / TypeScript** — backend services, Azure Functions, APIs
- **Python** — data processing, automation scripts
- **Other** — check the project first

## Code style

- Follow the conventions already present in the file you are editing
- Prefer clarity over cleverness
- No unnecessary comments — only add them when the *why* is non-obvious
- No emojis in code or commit messages unless explicitly requested

## Commits

- Short, imperative subject line (under 72 characters)
- Focus on *why*, not *what*
- No Co-Authored-By lines unless requested

## Language

- Code, variable names, and comments: English
- User-facing text and documentation for Norwegian users: Norwegian Bokmål
- Internal developer documentation: English is fine

## General behavior

- Ask before doing irreversible things (deleting files, force-pushing, dropping data)
- Prefer editing existing files over creating new ones
- Don't add features or abstractions beyond what was asked
- When unsure about requirements, ask one focused question rather than guessing
