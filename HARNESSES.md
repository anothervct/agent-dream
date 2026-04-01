# Harness Support

Support notes for `Agent Dream`.

Last reviewed: 2026-04-01

## Current Target

`Agent Dream` is currently shaped as a cross-harness skill pack, with the best support aimed at:

- Codex via `.agents/skills/`
- Claude Code via `.claude/skills/`
- OpenClaw via `skills/`

## Layout in This Repository

This repository currently includes:

- `.agents/skills/dream/`
- `.claude/skills/dream/`
- `.codex/skills/dream/`
- `skills/dream/`

The `.agents/skills/` version is the primary source for Codex-style agent skills. The `.claude/skills/` version exists so Claude Code can expose `/dream` directly as a skill command. The `.codex/skills/` version is kept as a convenience mirror for environments and tooling that look there, but `.agents/skills/` should be treated as the canonical Codex-facing path.
The `skills/` version exists for OpenClaw, whose workspace-native skill root is `<workspace>/skills`.

## Invocation Notes

### Codex

- Repository skills live in `.agents/skills/`
- Codex can explicitly invoke skills by typing `$` and selecting the skill
- In the Codex app, enabled skills can also appear in the slash command list

Recommended path:

- `.agents/skills/dream/`

### Claude Code

- Project skills live in `.claude/skills/`
- Skills can be invoked directly with `/dream`
- `disable-model-invocation` and `user-invocable` are supported in frontmatter

Recommended path:

- `.claude/skills/dream/`

### OpenClaw

- Workspace skills live in `<workspace>/skills`
- Shared local skills live in `~/.openclaw/skills`
- The most reliable explicit invocation is `/skill dream`
- Direct `/dream` may depend on channel and command registration settings

Recommended path:

- `skills/dream/`

## Notes

- `Agent Dream` is intentionally instruction-only in v0. It does not require scripts, tools, or memory persistence.
- The minimal contract is the skill text itself plus the expected Markdown output format.
- If a future release adds a one-line installer, this file should be updated with the exact supported targets and any fallback behavior.
