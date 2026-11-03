# Social Learn (Muse adapter)

Run the Social Agent Suite learning pass: turn a scrolling/working session's
observations into knowledge-base entries, and run the weekly upgrade that
promotes repeated patterns into skill files — always logged, never silent.

## When to use

- Any social session is ending (daily Instagram run, LinkedIn growth
  session, Threads/Facebook engagement, research) and observations were made.
- The owner says "learn karo", shares a post/reel/screenshot "for learning",
  or asks what the suite has learned lately.
- Weekly: the upgrade rollup is due.

## How a learning pass runs

1. Collect the session's raw observations (what was seen, where, engagement
   signal). If the owner shared material, treat it as learning input —
   extract the useful concept, save it, confirm briefly. No long verdicts.
2. Write each concept in your own words into the owner's workspace knowledge
   files (the local mirror of the repo `knowledge/`): hooks, formats,
   niche-notes, platform-changes, swipe-bank (new concepts marked UNUSED).
3. Deduplicate: if the pattern already exists, add the new sighting to its
   entry (repetition is what earns promotion) instead of a fresh copy.
4. Report one short line to the owner: what was learned and where it went.

## Weekly upgrade rollup

1. Scan knowledge entries: patterns seen 3+ times, or backed by the owner's
   own post results, are promotion candidates.
2. Propose the exact skill-file edits (hook formulas to add, rules to
   retire). Apply them, then log every change in `knowledge/CHANGELOG.md`
   (repo) and the suite CHANGELOG.
3. Tell the owner what the brain changed this week — a changelog he can
   read, not a silent mutation.

## Community inbox (part of the weekly rollup)

The rollup also reviews the public brain's inbox: open `learning:` PRs and
new packets in the repo's `community/inbox/`. Accept only concepts that
pass the safety filters in `core/community-learning.md` and carry real
evidence or repeat an existing sighting. Accepted concepts merge into
`knowledge/`, packets move to `community/accepted/`, promotions are logged
with the contributor's name. Rejections get a polite reason on the PR.
Use the `social-share` skill for the full procedure.

## Guardrails

Concepts only, never copied text. Claims labeled as claims. Learning never
publishes or sends anything. Client names and private details never enter
the knowledge base.
