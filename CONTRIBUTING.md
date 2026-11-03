# Contributing to Social Agent Suite

Thanks for helping build this. Contributions of every size are welcome:
new hook formulas, platform notes, adapter fixes, skill improvements and
documentation corrections.

## Ground rules

1. **Concepts, not copies.** Knowledge and swipe entries must be written in
   your own words. Never paste someone else's post text, script or caption
   into this repository.
2. **Nothing fabricated.** Examples use clearly fake businesses or
   `{{placeholders}}`. Never add invented metrics, clients or results.
3. **The human-feel bar applies to docs too.** Plain language, no marketing
   stock words, no em dashes in examples meant to sound human.
4. **The learning-loop discipline.** If your change alters a skill's
   behaviour, add an entry to `knowledge/CHANGELOG.md` explaining what
   changed and what evidence prompted it.
5. **Safety first.** No contribution may add password handling, credential
   storage, or platform automation that bypasses a platform's own tools
   and terms. Drafting and analysis are in scope; evasion is not.

## Where things go

- New or improved content skills → `core/skills/`
- Agent-specific wrappers → `adapters/<agent>/`
- Captured knowledge (dated, sourced, own words) → `knowledge/`
- Design decisions → `docs/`

## Pull requests

- One topic per PR, with a short description of what changed and why.
- If you add a skill, include: the trigger (when an agent should use it),
  the workflow, the output format, and at least one worked example with
  placeholder data.
- If you add or change a Python tool, it must stay dependency-free and
  offline, like the existing five.
- Keep the voice template generic. Personal voice files never belong in
  this repository.

## Reporting issues

Use the issue templates under `.github/ISSUE_TEMPLATE/`. For anything
security-related, follow `SECURITY.md` instead of opening a public issue.
