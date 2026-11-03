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

### Added
- Muse adapter: first adapted skill (`social-ig-content`) and adapter guide.
- Threads, LinkedIn, Facebook and X platform modules (in progress).
- Codex and Gemini/Antigravity adapters (in progress).

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
