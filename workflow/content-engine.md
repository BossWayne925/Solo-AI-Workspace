# The Content Engine — the pipeline

This workspace runs **one workflow**, expressed the ICM way: as numbered stage
folders. The folder structure *is* the workflow. You run the stages in order,
and each stage's `output/` feeds the next stage's input — a Unix-style pipeline.

```
 01_capture  →  02_plan  →  03_create  →  04_repurpose  →  05_review
  raw → ideas    ideas →     plan →        anchor →         log + learn
                 plan        draft         many variants    (writes to memory)
       │                                                          │
       │            ┌─── memory feeds planning ──────────────────┘
       └────────────┘   (Stage 05's output is Stage 02's input next week)
```

Each arrow is a real file handoff:
`01_capture/output/ideas.md` → `02_plan/output/week-plan.md` →
`03_create/output/<slug>.md` → `04_repurpose/output/variants.md` →
Stage 05 → `memory/published.md` + `memory/what-worked.md`.

## How to run a stage

Tell your AI which stage you're on. It reads `CLAUDE.md` (the rules), then that
stage's `context.md`, then does only that job:

> *"Read `01_capture/context.md` and run it on this: …"* (paste your raw notes)

After each stage the AI **stops, summarizes, and waits for you** (human-in-the-loop).
You review the `output/`, then move to the next stage. Nothing runs end-to-end
unattended — that's by design.

## First time?

> Run `BUILD.md` first if you haven't — the stages read the `profile.md` and
> `memory/voice.md` it generates. Without them, drafts won't sound like you.

A full first loop, start to finish, takes about an hour:

1. **01_capture** — dump everything in your head; get back sharp angles → `output/ideas.md`
2. **02_plan** — pick an anchor + supporting pieces, sized to what you can finish → `output/week-plan.md`
3. **03_create** — draft the anchor in your voice (hook options first) → `output/<slug>.md`
4. **04_repurpose** — turn the one anchor into 5–8 platform-native pieces → `output/variants.md`
5. **05_review** — once it's live, log it and capture what worked → writes to `memory/`

## The weekly rhythm

Memory does the heavy lifting, so the loop gets fast:
- **Monday (15 min):** Stage 02. It already knows what worked — lean into it.
- **Mid-week:** Stage 03, then Stage 04.
- **Friday (10 min):** Stage 05. Log the week, note any pattern.

## The one rule
**Never skip Stage 05.** It's the only stage that writes back to memory — the only
thing that makes the system *compound* instead of just repeat. Skip writing, skip
planning, never skip review. (And every stage logs one line to
`memory/session-log.md`, so you can always see what's been done.)
