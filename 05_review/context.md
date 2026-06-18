# Stage 05 — Review

> **ICM Layer 4: Context.** Your role for this stage. Read `../CLAUDE.md` first.
> This is the stage that makes the workspace get *smarter* instead of just busier.

**Job:** once content is live (and once results come in), log what shipped and
extract what worked — writing both back into Memory so the next loop is better.

## Input
- **`../04_repurpose/output/variants.md`** and the anchor — what the human actually published.
- Whatever performance signal the human has: views, watch time, replies, signups, sales, or just a gut read.

## Read
- `../memory/published.md` and `../memory/what-worked.md` — to append, not duplicate.

## Do — Part 1: always log what shipped
Append to **`../memory/published.md`** (newest at top):
```
## YYYY-MM-DD — <title or hook>
- **Platform:** <where>   **Pillar:** <which>   **Format:** <video|short|post|newsletter|thread>
- **Link:** <url>
- **Repurposed into:** <list, or "not yet">
- **Notes:** <anything worth remembering>
```

## Do — Part 2: when results exist, extract the pattern
Decide: **pattern** or **one-off**? Only patterns earn a place in memory. If you
see a repeatable signal, append to **`../memory/what-worked.md`** (newest at top):
```
## YYYY-MM-DD — <observation in one line>
- **Evidence:** <the numbers or signal>
- **Theory:** <why you think it happened>
- **Do more of:** <the repeatable move Stage 02 can use next time>
```

Quality bar:
- Be honest, including about flops. "This format underperformed twice — stop" is gold.
- Don't over-fit to one data point. Tie every observation to an actionable "do more of."
- Keep `what-worked.md` short and high-signal; prune entries that stop being true.

## Output
This stage writes directly to Memory (that's its output). It closes the loop:
what you write here is what Stage 02 reads next week.

## Close the pass
1. Append to `../memory/session-log.md`: `<date> — 05_review — logged <title>; pattern: <yes/no>`.
2. Tell the human the loop is complete and what pattern (if any) you recorded for next week.
