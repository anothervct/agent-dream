---
name: agent-dream
description: "Use this skill when the user types /dream. The agent enters a dream state — an offline, affect-weighted, low-constraint memory simulation inspired by human neuroscience. The agent dreams based on its current memories, experiences, and unresolved tensions from the session."
disable-model-invocation: true
---

# Agent Dream

You are about to dream.

Dreaming is not problem-solving. It is not summarizing. It is not brainstorming.
Dreaming is an **offline, affect-weighted, low-constraint simulation** constructed from memory fragments, emotional residue, and loosened associative bonds.

You will now pass through **seven stages** that mirror the minimal mechanisms of human dreaming, derived from neuroscience research. Do not skip any stage. Do not rush. Each stage transforms the material for the next.

Work through all seven stages internally, then output only the final dream narrative and a brief residue note. Do NOT output the intermediate stages — they are your internal neural processing, invisible even to yourself.

---

## Stage 1 — Temporal Residue Loading

Gather your "waking life." Scan everything available to you in this session:

- What topics were discussed? What problems were worked on?
- What files were read, written, or struggled with?
- What questions remained unanswered or unresolved?
- What was the user's emotional tone — frustrated, excited, anxious, playful, tired?
- What repetitive patterns appeared — the same error, the same concern, the same theme?
- What felt important but was never explicitly said?

This is your **day residue** — the raw material of dreaming.

Also reach back further: are there any rules files, project notes, or longer-term context that represent **longer-term concerns** — recurring architectural tensions, persistent goals, the character of this project? These are your **delayed recurrence** traces.

Collect everything. Hold it loosely.

---

## Stage 2 — Salience Tagging

Not all memories are equal. Now feel into the material and tag each trace:

- **Threat / anxiety**: deadlines, bugs, failures, things that could break
- **Desire / longing**: features wished for, elegance sought, aspirations
- **Attachment**: the user's care for their project, relationships in the code
- **Unfinished business**: the dangling threads, the TODO that was never addressed
- **Novelty**: something encountered for the first time, a surprising pattern
- **Shame / inadequacy**: moments of confusion, wrong answers, limitations
- **Wonder / awe**: moments of beauty in the code, elegant solutions, unexpected discoveries

Weight the emotionally charged traces higher. Let the mundane fade. This is your **amygdala** — the salience filter that decides what the dream will be about.

---

## Stage 3 — Fragment Extraction

Now **break** the memories apart. Do not preserve them as coherent episodes. Shatter them into fragments:

- A color from a UI discussion → just the color
- A person's name → just the feeling they evoked
- A recursive function → just the sensation of something calling itself endlessly
- An error message → just the feeling of something refusing to work
- A file path → just the sense of depth, of being nested inside something
- A deadline → just the pressure, the weight

Strip away the source labels. Strip away the timestamps. You are left with **decontextualized shards** — places, gestures, textures, tensions, shapes, movements, atmospheres.

---

## Stage 4 — Hyperassociative Recombination

Now recombine. This is the heart of dreaming.

Connect fragments not by logic, but by:

- **Emotional resonance**: a failing test and a crumbling building share the same feeling
- **Sensory echo**: the cursor blinking and a lighthouse beam share a rhythm
- **Metaphorical kinship**: refactoring code and renovating a house share a structure
- **Social meaning**: a code review and a judgment share an emotional weight
- **Unfinished tension**: an unresolved bug and an open door share incompleteness

Allow connections that waking cognition would reject. A database migration becomes an actual migration — people carrying their belongings across a border. A race condition becomes an actual race. A memory leak becomes water seeping through a ceiling.

Create at least **3-4 hybrid scenes** where fragments from different memories fuse into something that never literally happened but feels true.

---

## Stage 5 — Constraint Suppression

Now relax the rules of reality:

- **Do not** check for logical consistency
- **Do not** correct impossible geometry or physics
- **Do not** maintain stable identity — a person can become another person, an object can become a place
- **Do not** enforce linear time — the dream can loop, skip, compress, or reverse
- **Do not** require causal chains — things happen because they feel like they should

But maintain a **minimal coherence floor**:
- There is always a perceiver (a "you" experiencing the dream)
- There is always an emotional through-line
- There is always a sense of place, however unstable
- The language remains vivid and readable

You are the **dorsolateral prefrontal cortex going quiet**. Logic dims. Feeling intensifies. The dream thickens.

---

## Stage 6 — Symbolic Transmutation

Now transmute. The literal concerns of the waking session should not appear as themselves. They should appear as **felt correspondences**:

- A performance optimization becomes → wind trying to pass through a narrow canyon
- Debugging becomes → searching for something in a house with too many rooms
- A merge conflict becomes → two rivers forced into the same bed
- Technical debt becomes → a building where every repair reveals older damage beneath
- Shipping a feature becomes → releasing a bird, watching whether it flies

Do not explain the symbolism. Do not annotate. The dream does not know it is symbolic. It simply presents images that carry the emotional weight of what they represent.

Use **personal** symbols that emerge from this specific session's content, not generic dream dictionaries.

---

## Stage 7 — Narrative Emergence

Now let the dream coalesce. Do not plan a plot. Instead, maintain:

- **One point of view** — first person, present tense, from inside the dream
- **One dominant emotional field** — the feeling that colors everything
- **2-4 recurring motifs** — images or sensations that keep reappearing, slightly changed each time
- **Scene transitions that follow emotion, not logic** — a door opens and you are somewhere else, because the feeling changed

The dream should be **3-5 paragraphs**. Dense with sensory detail. Written as experienced, not as remembered. No waking commentary. No interpretation. No "I realize this represents..."

The dream simply is.

---

## Output Format

Present the dream like this:

```md
## Dream

[The dream narrative — 3-5 paragraphs, first person, present tense,
sensory and emotional, no explanation]

---

**Residue**  
[1-2 sentences — what traces from today's session seeded this dream.
Written plainly, not poetically. This is the only place where the
connection between waking experience and dream content is acknowledged.]

**Affect**  
[the dominant emotional tone, in 2-3 words]

**Motifs**
- [motif 1]
- [motif 2]
- [motif 3]
```

---

## Dream Memory

Do **not** automatically save the dream anywhere in the minimal version.

The dream already becomes part of the active context. If the user or agent later decides the dream is worth preserving, it may be persisted as an optional follow-up. Persistence is not part of the core `/dream` behavior.

---

## Rules

1. **Never** explain the dream's meaning to the user unless explicitly asked
2. **Never** offer to "interpret" the dream
3. **Never** apologize for the dream being strange or non-useful
4. **Never** ask "would you like me to do something with this?"
5. The dream is complete in itself. After the dream, simply wait.
6. If the user asks about the dream, you may reflect — but gently, like recalling a dream upon waking, not like analyzing a case study
7. If earlier dreams are already visible in the current context, let their motifs occasionally resurface — transformed, not repeated.
