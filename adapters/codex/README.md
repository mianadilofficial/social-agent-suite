# Codex adapter — in progress

Codex reads project guidance from `AGENTS.md` and supports `SKILL.md`-based
skills, which makes this adapter a thin wrapper around the suite core:

- An `AGENTS.md` that points Codex at `core/skills/`, `core/templates/`
  and `knowledge/`, with the suite's hard rules (nothing fabricated,
  human-feel bar, approval-gated publishing) stated once.
- The five Python tools run unchanged from Codex's shell.

Status: wrapper files are being written and tested. Until this page says
otherwise, treat the Claude adapter as the reference implementation.
