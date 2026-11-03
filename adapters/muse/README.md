# Muse adapter

Muse runs skills from `~/workspace/custom-skills/` as `local-*` folders,
triggered by natural language rather than slash commands. This adapter
converts the suite's core skills into that format and wires them to the
routes Muse actually has hands for:

- **Instagram** — the instagram connector/CLI (posting, insights), the
  live browser (follows and engagement, human-paced), and schedulers for
  the daily run.
- **Threads** — the threads connector/CLI.
- **LinkedIn and Facebook** — the signed-in browser, under the owner's
  standing session rules.
- **Knowledge** — the repo's `knowledge/` files are mirrored into the
  workspace, so learning captured by any run is available to every run.

## Skills in this adapter

| Folder | Adapts | Status |
|---|---|---|
| `social-ig-content/` | ig-carousel + ig-caption + ig-human, wired to Muse's carousel system | ✅ live |
| more | ig-reel, ig-plan, ig-audit, platform modules | 🚧 in progress |

## Voice and paths

The owner's filled voice profile and brand assets stay in his private
workspace. Only the generic template (`core/templates/voice.md`) ships in
this public repo. The Muse skills reference the workspace paths at runtime;
they contain no personal data themselves.

## Approval rules (binding)

Drafting, research and learning are autonomous. Publishing follows the
owner's standing authorizations (for example his daily Instagram system);
anything new — a first send on a channel, any DM — needs his explicit word.
Any platform block or warning stops the run immediately.
