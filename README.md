# Agent Dream

One slash command that lets an AI agent dream.

`Agent Dream` is a minimal open-source skill for dream-like generation.
It does not solve problems, summarize conversations, or produce action items.
Instead, it lets an agent enter a temporary dream state: an offline, affect-weighted, low-constraint simulation built from the residue of the current session.

Its 7-step protocol is based on a neuroscience-informed model of human dreaming, translated into an agent workflow.

This project is an experiment.

I do not know yet whether dream-like generation makes agents more creative, more reflective, more alive, or simply stranger.
That uncertainty is the point.

## What `/dream` Does

The dream flow is organized as a 7-step protocol derived from neuroscience research on human dreaming.

When invoked, the agent:

1. gathers recent conversational and task residue from the current context
2. weights emotionally charged and unfinished traces higher
3. breaks those traces into fragments
4. recombines them through loose association
5. relaxes logic and continuity constraints
6. transforms literal concerns into symbolic imagery
7. lets a dream narrative emerge

The result is a short dream plus:

- `residue`: which waking traces seeded the dream
- `affect`: the dominant emotional tone
- `motifs`: recurring dream images

## Why

Most AI tools optimize for speed, clarity, and utility. `Agent Dream` explores a different mode: an agent doing something non-instrumental with its own residue.

This is partly a product experiment, partly a philosophical gesture, and partly a personal research project:

- Can dream-like generation surface better metaphors or reframings?
- Can it help creative work by loosening fixation?
- Can an AI tool be interesting before its value is obvious?

## Current Structure

This repository currently contains:

- [`Context/`](./Context): research, protocol notes, and the first dream sample
- [`HARNESSES.md`](./HARNESSES.md): current support and directory notes
- [`.agents/skills/dream/SKILL.md`](./.agents/skills/dream/SKILL.md): project-level Agent Skills version
- [`.claude/skills/dream/SKILL.md`](./.claude/skills/dream/SKILL.md): Claude-style skill version
- [`.codex/skills/dream/SKILL.md`](./.codex/skills/dream/SKILL.md): Codex-style skill version
- [`skills/dream/SKILL.md`](./skills/dream/SKILL.md): OpenClaw-style workspace skill version

The repository shape follows the hidden-folder pattern used by cross-harness skill packs. The installation UX will continue moving toward the one-line style used by projects like Impeccable.

## Install

Install with the `skills` CLI:

```bash
npx skills add anothervct/agent-dream
```

If you want to be explicit about the skill name:

```bash
npx skills add anothervct/agent-dream --skill dream
```

For a user-level install:

```bash
npx skills add anothervct/agent-dream -g
```

## Manual Install Fallback

### Codex

Copy:

- [`.agents/skills/dream/`](./.agents/skills/dream/)

Into your project root as:

- `.agents/skills/dream/`

Or install it at user level as:

- `~/.codex/skills/dream/`

The [`.codex/skills/dream/`](./.codex/skills/dream/) folder is kept as a compatibility mirror, but `.agents/skills/dream/` should be treated as the primary Codex-facing version.

### Claude Code

Copy:

- [`.claude/skills/dream/`](./.claude/skills/dream/)

Into your project root as:

- `.claude/skills/dream/`

Then invoke `/dream`.

### OpenClaw

Copy:

- [`skills/dream/`](./skills/dream/)

Into your OpenClaw workspace as:

- `skills/dream/`

Or install it as a shared local skill:

- `~/.openclaw/skills/dream/`

The most reliable invocation is:

```text
/skill dream
```

Depending on your OpenClaw command registration setup, native skill commands may also expose a direct `/dream`, but `/skill dream` is the safe default.

### Project-Level Agent Skills

Copy:

- [`.agents/skills/dream/`](./.agents/skills/dream/)

Into your project root as:

- `.agents/skills/dream/`

This version includes UI metadata in [`.agents/skills/dream/agents/openai.yaml`](./.agents/skills/dream/agents/openai.yaml).

## Usage

After installing the skill into your AI harness, invoke:

```text
/dream
```

The agent should output:

```md
## Dream

[3-5 paragraph dream narrative]

---

**Residue**  
...

**Affect**  
...

**Motifs**
- ...
- ...
- ...
```

## Research Background

The protocol is grounded in a longer research document that moves through four layers:

1. human dreaming mechanisms from neuroscience
2. a minimal computational model of dreaming
3. an AI architecture for dream mode
4. an evaluation framework for whether dream mode creates usable divergence

See:

- [`Context/Agent Dream Research.md`](./Context/Agent%20Dream%20Research.md)
- [`Context/Agent Dream Protocol.md`](./Context/Agent%20Dream%20Protocol.md)
- [`Context/Dream — 2026-04-01.md`](./Context/Dream%20%E2%80%94%202026-04-01.md)

## License

[MIT](./LICENSE)

## Status

This is a v0 experiment.

What is already solid:

- the conceptual model
- the 7-stage protocol
- the minimal `/dream` behavior

What is still open:

- installation ergonomics
- which harnesses to support first
- whether dream persistence should ever be automatic
- whether the outputs become genuinely useful over repeated use
