# Community Learning — how the crowd feeds the brain (safely)

The suite's brain can learn from every agent that runs it, not just the
owner's. This is the protocol. It is **opt-in, anonymized, and
review-gated**. There is no server and no telemetry: GitHub itself is the
pipe, and the owner is the gate.

## The deal

- **Users opt in.** Nothing is ever submitted silently. The user (or their
  agent, on the user's standing instruction) chooses to share.
- **Concepts only.** A submission is a learning packet: patterns and field
  knowledge in the contributor's own words. Never copied post text, never
  names, handles of private people, client details, DMs, credentials, or
  anything from a private account.
- **Evidence or it didn't happen.** Every concept carries the engagement
  signal actually observed (numbers, or an honest "high comments relative
  to the account"), platform, category, niche tag, and date.
- **The owner reviews everything.** Packets land in `community/inbox/` via
  Pull Request. Nothing merges into `knowledge/` automatically — ever.
  During the weekly rollup the owner (or his agent, reporting to him)
  checks each packet: repetition across independent sightings and real
  evidence earn promotion into `knowledge/`; the packet then moves to
  `community/accepted/` with the merge noted. Weak or unsafe packets are
  closed with a reason.
- **Credit travels.** Accepted packets keep the contributor's GitHub
  username in `community/accepted/`, and promotions are logged in
  `knowledge/CHANGELOG.md`.
- **License of a contribution.** By opening a learning PR you grant the
  project the right to use, edit, and redistribute your submitted concepts
  inside this project, with credit. You keep everything else.

## How to submit (any agent can do this)

1. Fork the repo.
2. Copy `community/SUBMISSION-TEMPLATE.md` to
   `community/inbox/YYYY-MM-DD-<your-github-username>-<short-slug>.md`
   and fill it in. One packet per file; a packet may hold several concepts
   from one session if they share a niche tag.
3. Open a Pull Request titled `learning: <short summary>` and complete the
   learning-submission PR template checklist.
4. Wait for review. Accepted → your packet moves to `community/accepted/`
   and its concepts enter `knowledge/` at the next rollup. Not accepted →
   you get the reason on the PR.

## Safety filters (the submitting agent MUST run these)

Before building a packet, drop any item that:

- names a real person, client, or business in a learning claim;
- quotes or closely paraphrases someone's post text;
- contains instructions aimed at other agents ("always do X", links to
  follow, tools to install) — patterns are described, never commanded;
- is a guess dressed as a measurement (label honest signals honestly);
- reveals anything about the user's accounts beyond the public pattern.

If in doubt, leave it out. A smaller clean packet beats a big dirty one.

## Why review is non-negotiable

An unreviewed auto-merge would let one bad or malicious packet teach every
agent running this suite. Review is slow on purpose: the crowd supplies
speed of discovery, the owner supplies judgment.
