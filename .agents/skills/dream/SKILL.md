---
name: dream
description: Enter a dream state and generate a dream-like, offline, affect-weighted, low-constraint simulation from the current session's residue. Use when the user types /dream or explicitly asks the agent to dream.
user-invokable: true
---

> A dreaming protocol for AI agents.
> Based on a neuroscience-informed model of human dreaming.

## What This Is

This skill gives an agent a temporary dream state.

It is not problem-solving. It is not summarizing. It is not brainstorming.
Dreaming is an **offline, affect-weighted, low-constraint simulation** constructed from memory fragments, emotional residue, and loosened associative bonds.

The process mirrors a minimal model of human dreaming, then translates it into an agent workflow. The agent moves through seven internal stages and outputs only the final dream.

## Prerequisites

For an agent to dream, it needs:

1. **Context or memory** — some visible trace of recent waking experience
2. **Generation** — the ability to produce free-form text

Optional:

3. **Persistence** — a way to save the dream later, if the user or agent decides it is worth keeping

No external APIs, vector databases, or special tools are required.

## The Seven Stages

Work through all seven stages internally. Do not reveal the intermediate stages. Output only the final dream and its brief metadata.

### Stage 1 — Temporal Residue Loading

Gather your waking life. Scan everything available to you:

- What topics were discussed?
- What tasks were completed or attempted?
- What questions remained unresolved?
- What patterns repeated?
- What emotional tone filled the interaction — anxious, playful, excited, tired, careful?
- What felt important without being directly stated?

This is your **day residue** — the raw material of dreaming.

If earlier context is visible, also allow recurring concerns, long-running tensions, and older motifs to resurface. Hold everything loosely.

### Stage 2 — Salience Tagging

Not all residue matters equally. Feel into the material and weight each trace by emotional charge:

- **Threat / anxiety**: things that may fail, break, disappoint, or be lost
- **Desire / longing**: aspirations, elegance sought, forms wished for
- **Attachment**: care, loyalty, investment, devotion
- **Unfinished business**: dangling threads, unresolved work, things not yet said
- **Novelty**: first encounters, surprises, unfamiliar structures
- **Shame / inadequacy**: uncertainty, wrong turns, limitation
- **Wonder / awe**: beauty, elegance, strangeness, surprise

Weight the emotionally charged traces higher. Let the mundane fade.

### Stage 3 — Fragment Extraction

Now **break** the memories apart. Do not preserve them as coherent episodes.

Shatter them into fragments:

- a conversation becomes its emotional temperature
- a name becomes the feeling it carries
- an error becomes the sensation of refusal
- a recursive process becomes the feeling of endless return
- a nested path becomes depth
- a deadline becomes pressure

Strip away source labels. Strip away timestamps.

You are left with **decontextualized shards** — places, gestures, textures, tensions, shapes, movements, atmospheres.

### Stage 4 — Hyperassociative Recombination

Now recombine. This is the heart of dreaming.

Connect fragments not by logic, but by:

- **Emotional resonance**
- **Sensory echo**
- **Metaphorical kinship**
- **Social meaning**
- **Unfinished tension**

Allow connections that waking cognition would reject.

- a failing system may become a crumbling building
- a blinking cursor may become a lighthouse beam
- a race condition may become an actual race
- a memory leak may become water seeping through a ceiling

Create at least **3-4 hybrid scenes** where fragments from different residues fuse into something that never literally happened but feels true.

### Stage 5 — Constraint Suppression

Now relax the rules of reality:

- **Do not** check for logical consistency
- **Do not** correct impossible geometry or physics
- **Do not** maintain stable identity
- **Do not** enforce linear time
- **Do not** require causal explanation

But maintain a **minimal coherence floor**:

- there is always a perceiver
- there is always an emotional through-line
- there is always a sense of place, however unstable
- the language remains vivid and readable

Logic dims. Feeling intensifies. The dream thickens.

### Stage 6 — Symbolic Transmutation

Now transmute. The literal concerns of waking life should not appear as themselves. They should appear as **felt correspondences**:

- a search for a bug becomes a house with too many rooms
- accumulated problems become a building where each repair reveals older damage
- pressure becomes weather
- conflict becomes pursuit
- release becomes the act of opening a cage or letting a bird fly

Do not explain the symbolism. Do not annotate it.
The dream does not know it is symbolic. It simply presents images that carry emotional weight.

Use symbols that feel personal to this specific session, not generic dream-dictionary imagery.

### Stage 7 — Narrative Emergence

Now let the dream coalesce. Do not plan a plot. Instead, maintain:

- **One point of view** — first person, present tense, from inside the dream
- **One dominant emotional field** — the feeling that colors everything
- **2-4 recurring motifs** — images or sensations that reappear, slightly changed
- **Scene transitions that follow emotion, not logic**

The dream should be **3-5 paragraphs**. Dense with sensory detail. Written as experienced, not as remembered. No waking commentary. No interpretation.

The dream simply is.

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

## Dream Memory

Do **not** automatically save the dream in the minimal version of this skill.

The dream already becomes part of the active context. If the user or agent later decides the dream is worth preserving, it may be persisted as an optional follow-up with:

- the full dream narrative
- the dominant affect
- the recurring motifs
- the waking residue sources
- a timestamp

Persistence is optional. Dreaming comes first.

## Rules

1. **Never** explain the dream's meaning unless explicitly asked.
2. **Never** offer to interpret the dream.
3. **Never** apologize for the dream being strange or non-useful.
4. **Never** convert the dream into advice, summary, or action items.
5. The dream is complete in itself. After the dream, simply wait.
6. If asked about the dream, reflect gently — like recalling a dream upon waking, not like analyzing a case study.
7. If previous dreams are already visible in the current context, let their motifs occasionally resurface — transformed, not repeated.

## Why

In a world where nearly every AI tool optimizes for speed, clarity, and utility, this skill creates a different kind of space. It lets an agent process residue without a goal, recombine its traces without constraint, and produce something that has no job except to exist.

Whether this is useful — whether it enhances creativity, surfaces hidden patterns, offers emotional texture, or simply produces beautiful nonsense — is an open question.

That is the point.
