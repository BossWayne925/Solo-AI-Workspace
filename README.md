# Solo AI Workspace

A tiny, AI-native workspace that runs **one job for a solopreneur: your content.**

You point Claude (or Gemini) at this folder, spend ~10 minutes teaching it who you are, and from then on it helps you go from *raw idea* to *published post* to *ten repurposed pieces* — in your voice, remembering what you've already made and what worked.

No app to install. No automation platform. No multi-agent framework. Just a folder, your AI, and one workflow that compounds.

> This is the "mini" version of a much bigger AI Operating System kit. It throws out everything a solo creator doesn't need (vendor management, governance policies, automation flows, goal hierarchies) and keeps the one loop that actually moves the needle.

---

## Built on ICM (Interpretable Context Methodology)

This isn't a pile of prompts — it's structured with **ICM**: a filesystem-based way
to orchestrate an AI without writing any orchestration code. The big ideas:

- **The folder structure *is* the workflow.** Numbered stages (`01_capture/` …
  `05_review/`) make the next step obvious to both you and the AI.
- **Context-as-protocol.** A plain `context.md` inside each stage tells the AI what
  role to play at that step.
- **Multi-pass pipeline.** Each stage writes to its `output/`, which becomes the
  next stage's input — like a Unix pipe.
- **Human-in-the-loop.** The AI stops after every stage so you can review and steer.
- **Small context windows.** The AI only loads the files the current stage needs.

It maps to ICM's 5-layer stack:

| Layer | Here |
|---|---|
| 1 · Foundation | `CLAUDE.md` / `GEMINI.md` — the standing rules |
| 2 · Memory | `memory/` — voice, what's published, what worked, session log |
| 3 · Stages | `01_capture/` … `05_review/` — the numbered workflow |
| 4 · Context | each stage's `context.md` — its instructions |
| 5 · Output | each stage's `output/` — verified, fed to the next stage |

---

## The one workflow: the Content Pipeline

```
 01_capture  →  02_plan  →  03_create  →  04_repurpose  →  05_review
  raw → ideas    pick what    draft in      1 piece →        what landed →
                 to make      your voice    many formats     back into memory
       ▲                                                            │
       └──────────────── memory makes the next loop better ─────────┘
```

Every pass leaves the workspace a little smarter: it learns your voice, remembers what you published, and notices what performed.

---

## What's in here

```
Solo-AI-Workspace/
├── README.md              ← you are here
├── CLAUDE.md / GEMINI.md  ← Foundation: the rules the AI follows every session
├── BUILD.md               ← run once. Answer ~8 questions, the AI personalizes your workspace.
├── profile.md             ← who you are: voice, audience, platforms, pillars
├── memory/                ← what the AI remembers between sessions
│   ├── MEMORY.md          ← the index (always loaded)
│   ├── voice.md           ← samples + do/don't, so drafts sound like YOU
│   ├── published.md       ← log of what's gone out
│   ├── what-worked.md     ← performance notes that feed better ideas
│   └── session-log.md     ← one line per stage pass (the audit trail)
├── 01_capture/            ← Stage 1 — each stage has a context.md + an output/
│   ├── context.md
│   └── output/
├── 02_plan/
├── 03_create/
├── 04_repurpose/
├── 05_review/
└── workflow/
    └── content-engine.md  ← the pipeline overview
```

The clever part: **the stages ship done.** They're the same for everyone. The only thing the AI has to learn is *you* — and that's exactly what `BUILD.md` captures.

---

## Quickstart (~10 minutes)

1. **Open this folder** with an AI that can read files — Claude Code, Claude Desktop with the folder added as a Project, Gemini CLI, or Cursor.
2. **Run [BUILD.md](BUILD.md).** Paste it in, answer the ~8 questions. The AI fills in `profile.md` and `memory/voice.md` for you.
3. **Run the pipeline.** Starting at **`01_capture/`**, tell your AI: *"Read `01_capture/context.md` and run it on this: …"* It does the stage, saves its output, and stops for your review. Move to `02_plan`, and so on. See [workflow/content-engine.md](workflow/content-engine.md).
4. **Never skip Stage 05.** It's the one that writes back to memory — so next week's ideas stand on this week's results.

That's it. The workspace gets better the more you use it.

---

## Who this is for

- Solopreneurs and creators who publish content but feel like they're starting from a blank page every time.
- Anyone who wants their AI to **remember** their voice and history instead of re-explaining it every chat.
- Build-in-public folks who want a system they can actually show people.

## Requirements

- One AI that can read a folder of Markdown: **Claude** (Opus/Sonnet/Haiku) or **Gemini**. Free tiers work fine to start.
- Comfort opening folders and editing Markdown. That's the whole tech stack.

---

*Built in public. Fork it, gut it, make it yours.*
