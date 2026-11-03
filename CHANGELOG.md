# Changelog

All notable changes to Social Agent Suite are documented here.
Brain upgrades (learning-loop promotions into the skills) are logged
separately in `knowledge/CHANGELOG.md`.

## [Unreleased]

### Changed
- Licensing is now dual (owner's decision, 2026-11-03): the derived base
  portions remain MIT; all of Mian Adil's original additions are
  All Rights Reserved. Root `LICENSE` rewritten to state both parts;
  the standalone MIT text for the base portions lives in
  `core/skills/LICENSE`; NOTICE.md updated to match.

## [0.2.0] — 2026-11-03

### Added
- Platform modules (`platforms/`): Threads, LinkedIn, Facebook — full
  management skills with the owner's locked rules, real publishing routes,
  lead-hunting and tracker law. X module written and parked (owner's order).
- `core/learning-loop.md` — the canonical learning protocol.
- Muse adapter completed: social-reel, social-plan, social-audit,
  social-learn, social-threads, social-linkedin, social-facebook
  (8 skills total).
- Codex adapter ready: drop-in `AGENTS.md` + `skills/social-suite/SKILL.md`.
- Gemini / Antigravity adapter ready: `GEMINI.md` + daily-content and
  learning-pass workflows.
- The learning loop is wired into the owner's live Instagram daily run:
  every run reads the swipe bank first and ends with a learning pass into
  the local knowledge mirror.

## [0.1.0] — 2026-11-03

### Added
- Initial public release of the suite structure: `core/`, `knowledge/`,
  `adapters/`, `docs/`.
- Core brain: 13 Instagram content skills and 5 local Python tools
  (hook scorer, beat timer, caption linter, humanizer, swipe ranker),
  derived from Jakeschincariol/instagram-agent-skill (MIT, see NOTICE.md).
- The self-learning loop: knowledge files (hooks, formats, niche notes,
  platform changes, swipe bank) plus the brain-upgrade changelog discipline.
- Claude adapter (plugin marketplace files).
- Project documentation: professional README, CONTRIBUTING, SECURITY,
  Code of Conduct, issue and pull request templates.
