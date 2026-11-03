# Social Agent Suite — Blueprint (Adil's vision, 2026-11-03)

Goal: one skill suite that runs Adil's social media management on every relevant
platform, usable by any agent (Claude, Muse, Codex, Gemini/Antigravity), and
that LEARNS while it works — every scrolling session feeds its knowledge back
into the system so the brain keeps upgrading itself.

Base: Jakeschincariol/instagram-agent-skill (MIT — clone/modify/publish legal;
the LICENSE copyright notice stays in the repo). His sibling linkedin-agent-skill
can be mined the same way for the LinkedIn module.
Publish target: Adil's own repo — LINK PENDING from Adil.
Licensing CONFIRMED by Adil 2026-11-03: live WITH the MIT license, PUBLIC repo.

## Structure

1. CORE BRAIN (platform-agnostic, shared by all agents)
   - voice.md — Adil's voice profile (public repo gets the empty template only;
     the real file stays private/local)
   - human-feel rules (his locked bar: one specific observation, plain English,
     no em dashes, no marketing words, curiosity + pain + hook)
   - hook formulas bank, caption rules (first ~125 chars carry the hook),
     hashtag rules, content-format rules per goal (reach / saves / comments)
   - knowledge/ — the learning memory (below)
   - tools/ — the portable Python tools (hook scorer, caption linter,
     humanizer, swipe ranking by multiple-over-median)

2. PLATFORM MODULES (management skills per platform)
   - Instagram: carousel/reel/story writing + audit, wired to his real posting
     route (instagram-cli daily system, v2 carousel style)
   - Threads: same content adapted, threads-cli posting step
   - LinkedIn: post writing (his locked poster + brand rules), comment/reply
     rules, growth-session support (rotation, warm-up, tracker updates)
   - Facebook: profile handling rules (posts, comment replies, Adil attaches
     images himself — known browser limit)
   - X: module written but PARKED until login works (his order)
   - Each module: plan → write → humanize → publish route → audit, plus
     lead-hunting rules (research first, DM only with Adil's approval,
     businesses-only tracker sheet updates)

3. AGENT ADAPTERS (same core, different wrappers)
   - Claude: original SKILL.md format (base repo already is this)
   - Muse: ~/workspace/custom-skills/ local-* format, natural-language triggers,
     voice/knowledge paths pointed at Adil's workspace
   - Codex: SKILL.md / AGENTS.md wrapper
   - Gemini / Antigravity: GEMINI.md + workflow files

4. HANDS LAYER (what the base repo lacks)
   - The skills write; the hosting agent acts: instagram-cli, threads-cli,
     browser (FB/LinkedIn), crons. All acting stays inside Adil's standing
     approval rules — daily systems already authorized keep running, DMs and
     new sends still need his word, stop instantly on any block/warning.

## THE LEARNING LOOP (Adil's core ask, 2026-11-03)

Whenever any agent scrolls any platform for Adil's work (growth sessions,
daily runs, research), it must not just act — it must learn:

1. SPOT: field-relevant knowledge (web design, SEO, AI, small business) and
   high-engagement patterns in his niche (hooks, formats, questions that
   pull comments).
2. EXTRACT: the CONCEPT in its own words — never copied text (his swipe-file
   rule + copyright). Source platform, author, date, engagement signal noted.
3. STORE: into knowledge/ files by topic (hooks.md, formats.md, niche-notes.md,
   platform-changes.md) and the swipe/concept bank, marked used/unused.
4. APPLY: the next content cycle adapts the newest unused learnings first.
5. UPGRADE: a weekly rollup promotes repeated patterns into the skill files
   themselves (new hook formulas, retired weak rules) with a changelog entry,
   so Adil can see exactly how the brain changed. Knowledge updates are
   automatic; skill-logic changes are logged, never silent.
6. GUARDRAILS: unverified claims are stored as claims, not facts; a single
   viral post is a signal, not a rule (promotion needs repetition);
   learning never authorizes publishing or sending by itself.

## Build order
1. Clone base, build core, Muse Instagram module first; test on a real run.
2. Threads + LinkedIn + Facebook modules; X module parked.
3. Wire the learning loop into the existing daily crons (IG daily run,
   LinkedIn sessions) so learning starts accumulating immediately.
4. Codex + Gemini/Antigravity adapters.
5. Publish to Adil's repo (his name, his README, MIT LICENSE notice retained,
   voice template only — no personal data).

## Waiting on Adil
- The repo link where this goes live.
