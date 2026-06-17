# Skill: review

**Use when:** something went live, or you've got results (views, replies, signups).
This is the skill that makes the workspace get *smarter* instead of just busier.

**Reads & writes:** `memory/published.md`, `memory/what-worked.md`

---

## What to do

### Part 1 — always: log what shipped
For each piece that went live, append an entry to `memory/published.md` (newest at top):

```
## YYYY-MM-DD — <title or hook>
- **Platform:** <where>
- **Pillar:** <which pillar>
- **Format:** <video | short | post | newsletter | thread>
- **Link:** <url>
- **Repurposed into:** <list, or "not yet">
- **Notes:** <anything worth remembering>
```

### Part 2 — when you have results: extract the pattern
Ask the user for whatever signal they have — views, watch time, replies, shares,
signups, sales. Numbers are great; gut read is fine too.

Then decide: is this a **pattern** or a **one-off**? Only patterns go in memory.
If you see a repeatable signal, append to `memory/what-worked.md` (newest at top):

```
## YYYY-MM-DD — <observation in one line>
- **Evidence:** <the numbers or signal>
- **Theory:** <why you think it happened>
- **Do more of:** <the repeatable move>
```

## Quality bar
- **Be honest, including about flops.** "This format underperformed twice — stop
  making it" is one of the most valuable lines in the file.
- Don't over-fit to one data point. Wait for a pattern before writing a rule.
- Tie observations to something **actionable** — a "do more of" line that
  `plan-week` can actually use next time.
- Keep `what-worked.md` short and high-signal. Prune entries that stop being true.

## The payoff
Next time `plan-week` runs, it reads what you wrote here. That's the loop closing:
this week's results shape next week's plan. The workspace compounds.
