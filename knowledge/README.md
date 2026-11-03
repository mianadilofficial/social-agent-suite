# Knowledge — the learning memory

This folder is the suite's long-term memory. Every agent that works with
this suite reads it before creating content and writes to it after any
scrolling session. See `docs/BLUEPRINT.md` for the full learning-loop
design.

## Files

| File | Holds |
|---|---|
| `hooks.md` | Hook patterns, each with where it was seen and what it earned |
| `formats.md` | Content formats ranked by what they produce (reach, saves, comments) |
| `niche-notes.md` | Field knowledge captured while scrolling (web design, SEO, AI, small business) |
| `platform-changes.md` | Platform rule and algorithm changes, dated, with the source |
| `swipe-bank.md` | Concepts worth adapting, each marked UNUSED or USED (with date) |
| `CHANGELOG.md` | Every promotion of a pattern into the skills — the brain upgrades |

## Entry format

Every entry follows the same shape:

```
## YYYY-MM-DD — short title
- Source: platform, author/account, link if public
- Signal: what made this worth saving (engagement vs that account's norm, a result, a repeated pattern)
- Concept: the idea in your own words. NEVER copied text.
- Use: how the next content cycle should apply it
- Status: UNUSED / USED (date, where)
```

## Rules

- Own words only. A copied post is a copyright problem and a lazy entry;
  the concept is the value.
- A claim is stored as a claim until it is verified. Mark unverified
  entries clearly.
- One viral post is a signal, not a rule. Promotion into `core/skills/`
  needs the pattern to repeat, and every promotion is logged in
  `CHANGELOG.md`.
- Nothing in this folder authorizes publishing or sending. It informs
  drafting; the owner's approval rules govern acting.
