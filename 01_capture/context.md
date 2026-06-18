# Stage 01 — Capture

> **ICM Layer 4: Context.** Your role for this stage. Read `../CLAUDE.md` first.

**Job:** turn the human's raw, unprocessed input — build logs, a screenshot, a
voice-memo transcript, half-formed thoughts — into sharp, usable content ideas.

## Input
- Raw material the human pastes or points you to. Accept mess; don't make them format it.
- There is no previous stage — capture is the start of the pipeline.

## Read
- `../profile.md` — content pillars and the audience (one real person).

## Do
For each distinct idea in the raw input, write a captured idea:

```
### <punchy working title>
- **Pillar:** <which of the user's pillars, or "new pillar?">
- **Angle:** <the specific take — one sentence, not a topic>
- **Why it'd land:** <the tension or curiosity it creates for the audience>
- **Format fit:** <video | short | post | newsletter | thread> and why
- **Hook seed:** <one possible opening line>
```

Split multi-idea dumps. One vague topic is worth less than three sharp angles.
An "idea" is an **angle**, not a topic: not "AI tools" but "the one AI tool I
deleted after a week and what I use instead."

## Output
Write all captured ideas to **`output/ideas.md`** (newest at top). This file is
the input to Stage 02.

## Close the pass
1. Append to `../memory/session-log.md`: `<date> — 01_capture — N ideas captured`.
2. Tell the human what you captured and that the next stage is **02_plan**. Stop and let them review.
