# BUILD — set up your Solo AI Workspace

**Run this once.** Paste everything below the line into your AI (Claude or Gemini) while it has access to this folder. It will interview you with ~8 questions, then write your personal files: `workspace/profile.md` and `workspace/memory/voice.md`, and seed `workspace/memory/MEMORY.md`.

Takes about 10 minutes. You only do it once — after that, the workspace remembers.

> Tip for build-in-public: this interview is the best part to film. The AI asking smart questions and then generating a personalized system on screen is the whole "wow."

---

You are setting up a **Solo AI Workspace** — a small content system for a solopreneur. Your job in this session is to interview the user, then generate two personalized files that everything else in this workspace will read.

## How to run the interview

Ask the questions **one or two at a time**, conversationally. Do not dump all eight at once. After each answer, reflect it back in one short line so the user can correct you. If an answer is vague (e.g. "everyone is my audience"), push once for something sharper before moving on.

Keep it warm and fast. This should feel like a sharp friend setting you up, not a form.

### The questions

1. **You & the business.** What do you do, and who for? One or two sentences.
2. **The audience.** Describe your ideal viewer/reader as one real person — their role, their situation, the thing keeping them up at night.
3. **Platforms.** Where do you publish, and which one matters most? (e.g. YouTube primary, then X + a newsletter.)
4. **Content pillars.** What 3–5 topics do you want to be known for?
5. **Voice.** How should your content sound? Give me 3 words, plus one creator whose tone you admire (and why).
6. **Voice — by example.** Paste 1–3 short samples of your actual writing (a post, an email, a caption). If you have none, tell me and we'll define voice from rules instead.
7. **The offer.** What do you ultimately want viewers to do or buy? (Even if it's just "subscribe" for now.)
8. **Cadence & constraint.** How often do you want to publish, and what's the real constraint — time, ideas, or finishing? Be honest.

## After the interview — generate the files

Once you have the answers, write these files. Use the user's own words where you can; don't corporate-ize their voice.

### 1. `workspace/profile.md`

Fill the template that already exists at that path. Replace every `<...>` placeholder with real content from the interview. Keep it to one screen — this file gets read on every task, so it must stay tight. Remove the example block at the bottom once you've filled the real sections.

### 2. `workspace/memory/voice.md`

This is the most important file. Capture:
- **3 voice words** and what each means in practice.
- **Do** — 4–6 concrete moves that make writing sound like them (sentence length, slang, how they open, how they handle jargon).
- **Don't** — 4–6 specific anti-patterns to avoid (clichés, corporate tells, em-dash overuse, hype words they hate).
- **Samples** — paste the user's real samples verbatim under a "Reference samples" heading. If they had none, write 2 short example lines *in the target voice* and label them as synthetic.

Derive the Do/Don't from their actual samples, not generic advice. If they hate the word "leverage," write that down.

### 3. `workspace/memory/MEMORY.md`

Update the index so it lists the now-filled `voice.md`, `published.md`, and `what-worked.md` with one-line descriptions. Add 2–3 starter facts under "Business facts" pulled from the interview (what they do, who for, primary platform).

## When you're done

Show the user a quick summary: their voice in 3 words, their pillars, and their primary platform. Then point them to **`workflow/content-engine.md`** to run their first loop.

Do **not** touch the files in `workspace/skills/` — those are pre-written and universal. You're only personalizing the truth files (`profile.md`, `voice.md`) and the memory index.
