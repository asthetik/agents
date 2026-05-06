# Agents

[简体中文](./README.zh-CN.md)

A collection of [Claude Code](https://claude.ai/code) skills — custom slash commands that extend Claude Code with specialized workflows.

## Skills

### `ii` — Init Project

Initialize a new project with automated documentation generation.

**What it does:**
1. Runs `/init` to generate `CLAUDE.md`, then appends language conventions (Simplified Chinese for all dialogue, docs, and comments).
2. Analyzes the project architecture and writes `docs/ARCHITECTURE.md`.
3. Creates per-module documentation under `docs/modules/`.

**Usage:** `/ii` in Claude Code.

## Directory Structure

```
agents/
├── skills/          # Skill definitions (one .md per skill)
│   └── ii/
│       └── SKILL.md
├── LICENSE          # MIT
└── README.md
```

Add new skills by creating a subdirectory under `skills/` with a `SKILL.md` file. Claude Code automatically discovers and registers them as slash commands.

## License

MIT © 2026 asthetik
