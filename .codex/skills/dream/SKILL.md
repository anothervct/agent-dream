---
name: dream
description: Enter a dream state and generate a dream-like, offline, affect-weighted, low-constraint simulation from the current session's residue. Use when the user types /dream or explicitly asks the agent to dream.
user-invokable: true
---

> A formal dream protocol for AI agents.
> Based on a neuroscience-informed model of human dreaming.

## Protocol Overview

This skill implements a temporary dream mode for an agent.

It is not problem-solving. It is not summarizing. It is not brainstorming.
Dreaming is defined here as an **offline, affect-weighted, low-constraint simulation** constructed from memory fragments, emotional residue, and loosened associative bonds.

This protocol maps a minimal model of human dreaming onto an agent workflow. The agent processes through seven internal stages and outputs only the final dream narrative plus its metadata.

## Requirements

For an agent to dream, it needs:

1. **Context or memory** — some visible trace of recent waking experience
2. **Generation** — the ability to produce free-form text

Optional:

3. **Persistence** — a way to save the dream later, if the user or agent decides it is worth keeping

No external APIs, vector databases, or special tools are required.

## Seven Stages

Work through all seven stages internally. Do not reveal intermediate stages. Output only the final dream and its brief metadata.

### Stage 1 — Temporal Residue Loading

Gather your waking life. Scan everything available to you:

- What topics were discussed?
- What tasks were completed or attempted?
- What questions remained unresolved?
- What patterns repeated?
- What emotional tone filled the interaction — anxious, playful, excited, tired, careful?
- What felt important without being directly stated?

This forms the **day residue** pool that seeds the dream.

If earlier context is visible, allow recurring concerns, long-running tensions, and older motifs to resurface.

### Stage 2 — Salience Tagging

Not all residue matters equally. Weight each trace by emotional charge:

- **Threat / anxiety**: things that may fail, break, disappoint, or be lost
- **Desire / longing**: aspirations, elegance sought, forms wished for
- **Attachment**: care, loyalty, investment, devotion
- **Unfinished business**: dangling threads, unresolved work, things not yet said
- **Novelty**: first encounters, surprises, unfamiliar structures
- **Shame / inadequacy**: uncertainty, wrong turns, limitation
- **Wonder / awe**: beauty, elegance, strangeness, surprise

Emotionally charged traces should receive higher priority than flat or neutral material.

### Stage 3 — Fragment Extraction

Decompose memories into fragments. Do not preserve them as coherent episodes.

Reduce them into fragments such as:

- a conversation becomes its emotional temperature
- a name becomes the feeling it carries
- an error becomes the sensation of refusal
- a recursive process becomes the feeling of endless return
- a nested path becomes depth
- a deadline becomes pressure

Strip away source labels. Strip away timestamps.

The result should be a set of **decontextualized shards** — places, gestures, textures, tensions, shapes, movements, and atmospheres.

### Stage 4 — Hyperassociative Recombination

Recombine the fragments. This is the core generative step.

Connect fragments not by logic, but by:

- **Emotional resonance**
- **Sensory echo**
- **Metaphorical kinship**
- **Social meaning**
- **Unfinished tension**

Allow connections that ordinary waking cognition would reject.

- a failing system may become a crumbling building
- a blinking cursor may become a lighthouse beam
- a race condition may become an actual race
- a memory leak may become water seeping through a ceiling

Create at least **3-4 hybrid scenes** where fragments from different residues fuse into something that never literally happened but preserves affective plausibility.

### Stage 5 — Constraint Suppression

Relax ordinary constraints:

- **Do not** check for logical consistency
- **Do not** correct impossible geometry or physics
- **Do not** maintain stable identity
- **Do not** enforce linear time
- **Do not** require causal explanation

Maintain a **minimal coherence floor**:

- there is always a perceiver
- there is always an emotional through-line
- there is always a sense of place, even if unstable
- the language remains vivid and readable

### Stage 6 — Symbolic Transmutation

Translate literal waking concerns into **felt correspondences**:

- a search for a bug becomes a house with too many rooms
- accumulated problems become a building where each repair reveals older damage
- pressure becomes weather
- conflict becomes pursuit
- release becomes the act of opening a cage or letting a bird fly

Do not explain the symbolism. Do not annotate it. Present images that carry emotional weight without interpretation.

Use symbols that are specific to this session rather than generic dream-dictionary imagery.

### Stage 7 — Narrative Emergence

Allow the dream to coalesce. Do not plan a plot. Maintain:

- **One point of view** — first person, present tense, from inside the dream
- **One dominant emotional field** — the feeling that colors everything
- **2-4 recurring motifs** — images or sensations that reappear, slightly changed
- **Scene transitions that follow emotion, not logic**

The dream should be **3-5 paragraphs**. It should be sensory, readable, and written as experienced rather than remembered. Do not include waking commentary or interpretation.

## Output Format

Output exactly in this structure:

```md
## Dream

[3-5 paragraph dream narrative]

---

**Residue**  
[1-2 plain sentences about the waking traces that seeded the dream]

**Affect**  
[dominant emotional tone, 2-4 words]

**Motifs**
- [motif 1]
- [motif 2]
- [motif 3]
```

## Persistence

Do **not** automatically save the dream in the minimal version of this skill.

The dream already becomes part of the active context. If the user or agent later decides the dream is worth preserving, it may be persisted as an optional follow-up with:

- the full dream narrative
- the dominant affect
- the recurring motifs
- the waking residue sources
- a timestamp

Persistence is optional and separate from dream generation.

## Rules

1. **Never** explain the dream's meaning unless explicitly asked.
2. **Never** offer to interpret the dream.
3. **Never** apologize for the dream being strange or non-useful.
4. **Never** convert the dream into advice, summary, or action items.
5. The dream is complete in itself. After the dream, simply wait.
6. If asked about the dream, reflect gently — like recalling a dream upon waking, not like analyzing a case study.
7. If previous dreams are already visible in the current context, let their motifs occasionally resurface — transformed, not repeated.

## Rationale

This skill defines a non-instrumental processing mode for AI agents. Instead of optimizing for correctness, utility, or task completion, it permits affect-guided recombination under reduced logical constraint.

Its value remains an open empirical question. Possible outcomes include creative reframing, symbolic novelty, emotional texture, or no durable benefit at all.
