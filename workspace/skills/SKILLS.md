# Skills — index

> These are the playbooks. They ship done and work the same for everyone — they
> just read **your** `profile.md` and `memory/voice.md`. To run one, tell your AI:
> *"Run the `write-piece` skill on this idea: …"*

| Skill | When to use it | Reads | Writes |
|---|---|---|---|
| **capture-idea** | You have a raw thought, build log, or voice memo and want it logged as a usable idea. | profile | (idea list) |
| **plan-week** | Start of the week — decide what to actually make. | profile, what-worked, published | (week plan) |
| **write-piece** | Turn one idea into a finished draft in your voice. | profile, voice | (draft) |
| **repurpose** | Turn one finished piece into many, format-matched per platform. | profile, voice, published | (variants) |
| **review** | Something went live, or you got results — log it and learn. | published, what-worked | published, what-worked |

## The order they run in (the loop)
```
capture-idea  →  plan-week  →  write-piece  →  repurpose  →  review
                                                              │
                                          review feeds plan-week next time
```

See `workflow/content-engine.md` for how to run the whole loop in one sitting.

## Rule for every skill
Always read `memory/voice.md` before producing anything a human will read. A draft
that doesn't sound like the user is a failed draft, no matter how good the content.
