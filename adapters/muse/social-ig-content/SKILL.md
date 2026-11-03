# Social IG Content (Muse adapter)

Create Instagram content for the owner using the Social Agent Suite core:
a 4–6 slide carousel (the suite's proven reach format), a linted caption,
and a humanized final draft — then publish through Muse's real routes
under the owner's standing daily-system authorization.

## When to use

The owner asks for an Instagram post, carousel, caption or story idea, or
the daily Instagram run starts. For one-off captions, use the caption
section only. For reels, use the core `ig-reel` skill instead.

## Inputs to read first

1. The owner's voice profile (private workspace copy of
   `core/templates/voice.md`, filled in).
2. `knowledge/swipe-bank.md` — adapt the newest UNUSED concept first; mark
   it USED with the date when the post ships.
3. `knowledge/formats.md` and `knowledge/hooks.md` — current evidence on
   what earns reach, saves and comments.
4. The content log of the daily system — never repeat yesterday's topic
   or hook type.

## Workflow

1. **Pick the hook type** from the weekly mix: ~2 debate/binary, 1
   numbered mistake list, 1 story post, 1 keyword post, rest
   myth-busting / hot take.
2. **Draft the carousel** (core `ig-carousel` rules, 1080×1350 per slide):
   - Cover: a pain-point hook in ≤8 words, the owner's real face where the
     design calls for it, one strong scene, a clear swipe cue.
   - Middle slides: scene-based teaching. Never flat text-and-icon slides,
     never paragraph slides. Fresh layout every day; the branding is the
     repeatable system, not a copied template.
   - Last slide: the debate/binary question (or the keyword exchange on
     keyword days).
   - Every slide passes the brand check at full size and at 360px:
     owner's real face unchanged, brand line present, site link spelled
     exactly right.
3. **Write the caption** (core `ig-caption` rules): the hook lives in the
   first ~125 characters; the story/points follow; the LAST line is the
   slide-5 question. No pitch line except on keyword days. Maximum 5
   hashtags (platform rule, 2025-12-18 — see
   `knowledge/platform-changes.md`). Run the caption through
   `core/skills/ig-caption/caption.py`.
4. **Humanize** the full draft with the core `ig-human` tools
   (`humanize.py` + `detect.py`): no em dashes, no stock AI vocabulary, no
   invisible characters. Nothing fabricated: no invented clients, numbers
   or results, ever.
5. **Publish** (only inside the owner's standing authorization): feed post
   with all slides in order at one shared size; story = cover slide with
   the link sticker; the same carousel to Threads with a ≤500-character
   caption when the daily system calls for it.
6. **Log and learn**: record the post (topic, hook type, links) in the
   content log. Then run the learning pass: anything field-relevant seen
   while working today goes into `knowledge/` in the standard entry
   format, in your own words.

## Hard rules

- Stop instantly on any Instagram block, warning or challenge. No retry
  the same day.
- A DM is drafted, never sent, without the owner's explicit approval.
- If artwork cannot meet the brand check, ship nothing rather than ship a
  wrong face or a missing brand line.
