# Progress

Mastery is evidence-based. Do not raise scores without demonstrated understanding in a session.

**Status, mastery, Bloom, and `next_review` live only in `curriculum/INDEX.md`.** This file holds scales, review rules, weak areas, and the session log.

## Scale

| Mastery | Meaning |
|---------|---------|
| 0/5 | Not started |
| 1/5 | Heard of it / fragile awareness |
| 2/5 | Can follow explanations; cannot apply reliably |
| 3/5 | Can apply with guidance; gaps remain |
| 4/5 | Can explain, apply, and compare alternatives |
| 5/5 | Meets mastery criteria (explain, build, compare, when not to use) |

Bloom levels: Knowledge → Understanding → Application → Analysis → Evaluation → Creation

Status: `not_started` | `in_progress` | `review` | `mastered`

## Review intervals

When mastery or last_reviewed changes, set `next_review` = today + interval for current mastery:

| Mastery | Interval |
|---------|----------|
| 1/5 | +3 days |
| 2/5 | +1 week |
| 3/5 | +2 weeks |
| 4/5 | +1 month |
| 5/5 | +3 months |

Adjust intervals if retention evidence says they are too aggressive or too loose. Unstarted topics (0/5) have no `next_review`.

## Weak areas / open gaps

- None recorded yet (system just initialized)

## Recent sessions

Keep the last ~10 rows. Older rows may be dropped once reflected in topic files and INDEX.

| Date | Topic | Outcome |
|------|-------|---------|
| — | — | — |

## How to update

After a non-trivial lesson:

1. Update `topics/<slug>.md` (detail + status block including `next_review`)
2. Update the row in `curriculum/INDEX.md` (status, mastery, Bloom, last reviewed, next review)
3. Append a line under **Recent sessions** here; trim to ~10
4. Update **Weak areas** if a new gap or closed gap is clear
5. Propose commit: `session(<slug>): <summary>`
