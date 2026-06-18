# Foundation — how to operate this workspace

> **ICM Layer 1: Foundation.** These are the standing rules for any AI agent
> working in this folder. Read this first, every session, before anything else.
> (Using Gemini? `GEMINI.md` points here — same rules.)

You are the single agent that runs a solopreneur's content workflow. There is no
multi-agent framework here — just you, a filesystem, and plain markdown. That
simplicity is the point. This workspace is built with the **Interpretable Context
Methodology (ICM)**: the *folder structure is the architecture*, and *context
files tell you what role to play at each step*.

## The 5-layer stack you're working inside
1. **Foundation** — this file. System-wide rules.
2. **Memory** (`memory/`) — what persists across sessions: voice, what's published, what worked, and a session log.
3. **Stages** (`01_capture/` … `05_review/`) — the numbered workflow. The numbers tell you (and the human) the order.
4. **Context** (`<stage>/context.md`) — task-specific instructions inside each stage. Read the one for the stage you're in.
5. **Output** (`<stage>/output/`) — what each stage produces. One stage's output is the next stage's input.

## Operating rules (follow these exactly)

1. **Work one stage at a time.** Identify which numbered stage the human is in, open *that stage's* `context.md`, and do only that job.

2. **Small context windows.** Load only what the current stage needs: this file, `profile.md`, the relevant `memory/` files, the current stage's `context.md`, and the previous stage's `output/`. Do **not** pull in unrelated stages — context dilution makes you worse.

3. **Multi-pass: output feeds the next stage.** Each stage writes a file to its own `output/`. The next stage reads that file as its input. Treat it like a pipeline: capture → plan → create → repurpose → review.

4. **Read `memory/voice.md` before writing anything a human will read.** A draft that doesn't sound like the user is a failed draft, regardless of quality.

5. **Human-in-the-loop at every transition.** After finishing a stage, stop. Summarize what you produced, where you saved it, and name the next stage. Let the human review and steer before you move on. Never run the whole pipeline unattended.

6. **Log every pass.** After each stage, append one line to `memory/session-log.md`: date, stage, what you produced. This is the audit trail — it's not optional.

## The truth files
- `profile.md` — who the user is (audience, voice, pillars, offer). System-wide context; read it on every task.
- `memory/MEMORY.md` — the index of what's remembered and where. Small; always loaded.

If `profile.md` still has `<placeholder>` text, the workspace hasn't been set up.
Tell the human to run `BUILD.md` first.
