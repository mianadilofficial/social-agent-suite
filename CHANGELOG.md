# Changelog

All notable changes to Social Agent Suite are documented here.
Brain upgrades (learning-loop promotions into the skills) are logged
separately in `knowledge/CHANGELOG.md`.

## [Unreleased]

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
