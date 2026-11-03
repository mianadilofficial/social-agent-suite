# Codex adapter

Status: ✅ Ready

Two pieces, both usable today:

1. **`AGENTS.md`** — drop it into any project where Codex should operate
   the suite. It wires Codex to the core, the platform modules, the
   knowledge base, and the owner's laws.
2. **`skills/social-suite/SKILL.md`** — a Codex-format skill that routes
   every social task through the suite (content, engagement, leads,
   learning pass).

## Setup

1. Clone this repo (or copy `adapters/codex/AGENTS.md` + this skill into
   your project, keeping the repo's `core/`, `platforms/`, `knowledge/`
   folders reachable at the paths the files reference).
2. Fill your voice profile from `core/templates/voice.md` and keep the
   filled copy OUT of the public repo (`voice.local.md` is gitignored).
3. Publishing happens through your own authorized routes (CLIs, browser);
   the suite supplies the brain, your environment supplies the hands.
