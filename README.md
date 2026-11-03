# Social Agent Suite

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status: Building in public](https://img.shields.io/badge/status-building%20in%20public-blue.svg)](#-roadmap)
[![Agents: Claude · Muse · Codex · Gemini](https://img.shields.io/badge/agents-Claude%20%C2%B7%20Claude%20Code%20%C2%B7%20Codex%20%C2%B7%20Gemini-purple.svg)](#-agent-adapters)

**Social media management skills for AI agents — with a self-learning loop.**

Created and maintained by **[Mian Adil](https://portfolio.mianadil.site)** — Full-Stack Web Engineer · Technical SEO · AI Automation · Co-Founder, [Renzoify](https://portfolio.mianadil.site)

[![Portfolio](https://img.shields.io/badge/Portfolio-mianadil.site-0A66C2?style=flat-square)](https://portfolio.mianadil.site)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-mianadilhussain-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/mianadilhussain/)
[![Instagram](https://img.shields.io/badge/Instagram-mianadilofficial-E4405F?style=flat-square&logo=instagram)](https://www.instagram.com/mianadilofficial)
[![Threads](https://img.shields.io/badge/Threads-mianadilautomation-000000?style=flat-square&logo=threads)](https://www.threads.com/@mianadilautomation)
[![Facebook](https://img.shields.io/badge/Facebook-Mian%20Adil%20Hussain-1877F2?style=flat-square&logo=facebook)](https://www.facebook.com/mianadilhussain007)
[![GitHub](https://img.shields.io/badge/GitHub-mianadilofficial-181717?style=flat-square&logo=github)](https://github.com/mianadilofficial)

One core brain that any agent can use to manage **Instagram, Threads,
LinkedIn, Facebook and X**: planning, writing, humanizing, publishing
through the agent's own tools, and auditing what worked.

What makes this suite different is the loop: **every scrolling session is
also a learning session.** When an agent works on any platform, it extracts
field-relevant knowledge and high-engagement patterns *in its own words*,
stores them in [`knowledge/`](knowledge/), applies them to the next content
cycle, and promotes repeated patterns into the skills themselves — always
with a changelog entry, never silently. The system upgrades its own brain
while it works.

---

## Table of contents

- [Why this exists](#why-this-exists)
- [Features](#-features)
- [Quick start](#-quick-start)
- [Repository structure](#-repository-structure)
- [The learning loop](#-the-learning-loop)
- [Agent adapters](#-agent-adapters)
- [The 13 core skills](#-the-13-core-skills)
- [Rules this suite lives by](#-rules-this-suite-lives-by)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [Credit](#-credit)
- [License](#-license)

## Why this exists

Most "social media agent" packs do one thing: they write drafts and stop.
The agent running them still has to act through its own tools, and nothing
it sees while working ever makes the next post better.

This suite is built the other way around:

1. **A shared brain** — skills, tools and a voice profile that every agent
   reads the same way.
2. **Real hands** — each agent connects the skills to its own publishing
   routes (CLIs, browser, schedulers) under the owner's approval rules.
3. **A memory that compounds** — knowledge captured during ordinary work is
   filed, reused and promoted into the skills on a weekly rollup.

## ✨ Features

- **13 production content skills** — reels, carousels, captions, stories,
  profile scoring, weekly planning, comment/reply/DM drafting, repurposing,
  niche viral research and post audits.
- **5 local tools that actually run** — a hook scorer, a script timer, a
  caption linter (with the 125-character feed preview), an AI-slop
  humanizer, and a swipe-file ranker that scores posts by *multiple over
  the account's own median* instead of raw views. No dependencies, no
  network, nothing uploaded.
- **Multi-platform by design** — the same core drives Instagram today;
  Threads, LinkedIn, Facebook and X modules build on the same structure.
- **Agent-agnostic** — adapters for Claude, Muse, Codex and
  Gemini/Antigravity. Update the core once; every agent improves.
- **Self-learning loop** — structured knowledge files, a swipe bank, and a
  brain-upgrade changelog (see below).
- **Safety built in** — nothing fabricated under the user's name, a strict
  human-feel bar on all writing, instant stop on any platform block or
  warning, and publishing always governed by the owner's approval rules.

## 🚀 Quick start

### 1. Give the suite your voice

Copy `core/templates/voice.md` to your agent's voice location (each adapter
README names its path) and fill it in — or hand your agent three of your own
posts and say *"write my voice.md from these"*. Every skill reads this file.
Ten minutes here is the difference between content you publish and content
you rewrite.

### 2. Pick your agent

| Agent | Where to start |
|---|---|
| Claude / Claude Code | [`adapters/claude/`](adapters/claude/) — ready |
| Muse | [`adapters/muse/`](adapters/muse/) — first skills live |
| Codex | [`adapters/codex/`](adapters/codex/) — in progress |
| Gemini / Antigravity | [`adapters/gemini/`](adapters/gemini/) — in progress |

### 3. Run your first skill

Ask your agent for a carousel, a caption or a weekly plan in plain language
(or use the adapter's commands). The agent drafts with the core skills,
runs the humanizer, and hands you a publish-ready result. Posting happens
through your agent's own tools, under your approval rules — the suite
itself never asks for your password and never automates a platform behind
your back.

## 📁 Repository structure

```
core/            the platform-agnostic brain
  skills/        the 13 content skills (see table below)
  templates/     voice.md template
knowledge/       the learning memory
  hooks.md           hook patterns that proved themselves
  formats.md         formats ranked by what they earn (reach/saves/comments)
  niche-notes.md     field knowledge captured while scrolling
  platform-changes.md  algorithm and rule changes, dated and sourced
  swipe-bank.md      concepts worth adapting, marked used/unused
  CHANGELOG.md       every brain upgrade, with the reason
adapters/        the same core, wrapped per agent
  claude/  muse/  codex/  gemini/
docs/            blueprint and design notes
```

## 🧠 The learning loop

Whenever any agent scrolls any platform for the owner's work — a growth
session, a daily run, research — it must not just act. It must learn:

1. **Spot** — field-relevant knowledge and posts that clearly beat their
   account's normal engagement.
2. **Extract** — save the *concept* in its own words. Never copy text.
   Note the source, the date and the engagement signal.
3. **Store** — file it in `knowledge/`, marked used or unused. Unverified
   claims are stored as claims, not facts.
4. **Apply** — the next content cycle adapts the newest unused learnings
   first.
5. **Upgrade** — on the weekly rollup, patterns that repeated are promoted
   into the skill files themselves, with an entry in
   `knowledge/CHANGELOG.md`. A single viral post is a signal, not a rule;
   promotion needs repetition.

Learning never authorizes publishing or sending by itself.

## 🔌 Agent adapters

- **Claude** — the original skill format. Plugin marketplace files live in
  `adapters/claude/`; the skills in `core/skills/` install as-is.
- **Muse** — custom skills in Muse's `local-*` format with
  natural-language triggers and workspace paths, wired to Muse's real
  publishing routes (Meta CLIs, browser, schedulers).
- **Codex** — `SKILL.md` / `AGENTS.md` wrapper around the same core.
- **Gemini / Antigravity** — `GEMINI.md` context + workflow files around
  the same core.

## 🧰 The 13 core skills

| Skill | What it does |
|---|---|
| `ig-reel` | One idea → three scored hooks (26 formulas), script, on-screen text, timed beat sheet |
| `ig-viral` | Finds what is working in your niche, ranks by multiple over each account's median, builds the swipe file |
| `ig-caption` | The caption, linted — shows the ~125 characters the feed actually displays |
| `ig-carousel` | Swipe posts: the cover that earns the swipe, slide copy, 1080×1350 output |
| `ig-story` | Daily story sequences and which sticker does which job |
| `ig-profile` | Scores a profile out of 100 against a 12-part rubric, rewrites in fix-first order |
| `ig-plan` | The week: what to post, which format, when, and which accounts to engage |
| `ig-human` | The humanizer: strips em dashes, stock AI vocabulary and invisible characters, scores the result |
| `ig-comment` | Comments on other posts, in nine types matched to the post — never generic praise |
| `ig-reply` | Your own comment threads, sorted keyword / lead / substance / question / support / noise |
| `ig-dm` | Keyword delivery, first message, collab pitch, and exactly two follow-ups |
| `ig-repurpose` | One video, podcast or newsletter → a week of posts that each stand alone |
| `ig-audit` | Post-mortem: ranks your posts by outlier multiple and sends per reach, not views |

## 📏 Rules this suite lives by

- **Nothing fabricated.** No invented clients, metrics or results under the
  user's name. A missing number stays a `{{placeholder}}` and gets flagged.
- **Human-feel bar.** One specific observation, plain everyday language,
  curiosity + pain + a hook. No em dashes, no marketing stock words
  ("leverage", "game-changer", "skyrocket"), no hype, no emoji spam.
- **Approvals are real.** Learning and drafting are automatic; publishing
  and sending follow the owner's standing rules. DMs need the owner's word.
- **Platform safety.** Human pace, genuine engagement only, no fake
  engagement ever — and an instant stop on any block, warning or challenge.

## 🗺️ Roadmap

- [x] Core brain imported (13 skills + 5 tools)
- [x] Knowledge base + learning-loop structure
- [x] Claude adapter
- [ ] Muse adapter — full Instagram set, then wired into a live daily system
- [ ] Threads module
- [ ] LinkedIn module
- [ ] Facebook module
- [ ] X module (written; activates when the account route is ready)
- [ ] Codex adapter
- [ ] Gemini / Antigravity adapter
- [ ] Learning loop wired into live daily runs, first weekly rollup

## 🤝 Contributing

Issues and pull requests are welcome — see
[`CONTRIBUTING.md`](CONTRIBUTING.md) and the
[Code of Conduct](CODE_OF_CONDUCT.md). Security reports: see
[`SECURITY.md`](SECURITY.md).

## 👤 Author

<img src="https://github.com/mianadilofficial.png" width="110" align="left" alt="Mian Adil" />

**Mian Adil** — Full-Stack Web Engineer, Technical SEO Consultant and AI
Automation builder from Pakistan, working with international clients.
Co-Founder of **Renzoify**, a digital agency. He builds websites, SEO
systems and AI automations for local businesses, and created this suite to
run his own social media with AI agents — then open-sourced the system so
other builders can do the same.

- 🌐 Portfolio: [portfolio.mianadil.site](https://portfolio.mianadil.site)
- 💼 LinkedIn: [linkedin.com/in/mianadilhussain](https://www.linkedin.com/in/mianadilhussain/)
- 📸 Instagram: [@mianadilofficial](https://www.instagram.com/mianadilofficial)
- 🧵 Threads: [@mianadilautomation](https://www.threads.com/@mianadilautomation)
- 📘 Facebook: [Mian Adil Hussain](https://www.facebook.com/mianadilhussain007)
- 🐙 GitHub: [@mianadilofficial](https://github.com/mianadilofficial)

<br clear="left" />

## 🙏 Credit

The core Instagram skills are derived from
[Jakeschincariol/instagram-agent-skill](https://github.com/Jakeschincariol/instagram-agent-skill)
(MIT) — see [`NOTICE.md`](NOTICE.md). The multi-platform structure, agent
adapters, publishing workflows and the self-learning loop are original work
by **Mian Adil**.

## 📄 License

MIT — see [`LICENSE`](LICENSE). Use it, change it, ship it.

---

<p align="center">
  <b>Social Agent Suite</b> — created and maintained by <a href="https://portfolio.mianadil.site">Mian Adil</a>.<br/>
  If this project helps you, a ⭐ on the repo is the best thank-you.
</p>
