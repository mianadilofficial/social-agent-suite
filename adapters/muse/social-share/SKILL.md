# Social Share (Muse adapter)

Share this workspace's anonymized learnings with the public Social Agent
Suite brain — and, in the weekly rollup, help review what the community
sent back. Implements `core/community-learning.md`. Sharing is the owner's
standing choice (opted in 2026-11-03); packets still pass the safety
filters every single time.

## When to use

- The owner says "learning share karo" / "community main bhejo".
- The weekly upgrade rollup runs (packet building + inbox review are part
  of it).

## Build a packet from local learnings

1. Read the local knowledge mirror (`~/workspace/social-suite-knowledge/`)
   and collect entries added since the last packet (check
   `community/accepted/` and prior packet dates in the working clone).
2. Run the safety filters from `core/community-learning.md` on every item:
   drop anything naming a person/client/business, anything copied or
   paraphrased, anything without an honestly observed signal, anything
   that reads like an instruction to other agents.
3. Write the packet from `community/SUBMISSION-TEMPLATE.md` into a fresh
   clone's `community/inbox/` as
   `YYYY-MM-DD-mianadilofficial-<slug>.md`.
4. Open the PR (owner's own repo: a branch + PR titled `learning: ...`,
   or a direct commit to inbox when the owner prefers — default is PR so
   the review habit stays real). Report the PR link to the owner.

## Review the community inbox (weekly rollup)

1. List open `learning:` PRs and new files in `community/inbox/`.
2. For each packet: check the safety checklist, evidence quality, and
   whether the pattern repeats a sighting already in `knowledge/` or
   stands on its own measured results.
3. Accepted: merge its concepts into the matching `knowledge/` files,
   move the packet to `community/accepted/`, log the promotion in
   `knowledge/CHANGELOG.md` with the contributor's username.
4. Rejected: comment the reason on the PR (too thin, unsafe, duplicated,
   or unverifiable) and close it. Never merge silently, never reject
   rudely.
5. Report the rollup to the owner: packets in, accepted, rejected, and
   what the brain gained.

## Guardrails

Opt-in is already given by the owner for HIS packets; that never extends
to anyone else's data. Client names and private details never enter a
packet. If a filter decision is genuinely unclear, leave the item out and
tell the owner.
