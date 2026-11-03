# Gemini / Antigravity adapter — in progress

Gemini CLI and Antigravity read persistent context from `GEMINI.md` and run
repeatable jobs as workflow files. This adapter will ship:

- A `GEMINI.md` that loads the suite core (`core/skills/`,
  `core/templates/`, `knowledge/`) and states the hard rules once.
- Workflow files mirroring the daily content cycle and the learning pass,
  so a Gemini agent scrolling any platform files its learnings into
  `knowledge/` in the same entry format every other agent uses.
- The five Python tools, unchanged — they are plain local scripts.

Status: being written and tested in Antigravity. Until this page says
otherwise, treat the Claude adapter as the reference implementation.
