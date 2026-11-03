# Gemini / Antigravity adapter

Status: ✅ Ready

- **`GEMINI.md`** — the context file Gemini CLI and Antigravity read at
  project start. It wires the agent to the core, the platform modules,
  the knowledge base, the owner's laws, and the learning duty.
- **`workflows/`** — literal step files for the two recurring jobs:
  `daily-content.md` (the daily cross-platform cycle) and
  `learning-pass.md` (the end-of-session knowledge update).

## Setup

1. Clone this repo into the workspace the agent runs in, so the relative
   paths in `GEMINI.md` resolve.
2. Keep the filled voice profile local (`voice.local.md`, gitignored);
   the public repo only carries `core/templates/voice.md`.
3. Publishing uses the environment's own authorized routes (CLIs,
   browser, crons). The suite is the brain; the host supplies the hands.
