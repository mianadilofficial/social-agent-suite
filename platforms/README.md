# Platform Modules

One module per platform. Each module is a self-contained skill: it knows the
platform's formats, the owner's locked rules, the real publishing route
(the "hands"), lead-hunting rules, and the learning pass every session owes
the shared knowledge base (`knowledge/`).

| Module | Status | Publishing route |
|---|---|---|
| Instagram — `core/skills/` (ig-*) + `adapters/muse/social-ig-content` | ✅ Live | instagram-cli + browser |
| [Threads](threads/SKILL.md) | ✅ Live | threads-cli |
| [LinkedIn](linkedin/SKILL.md) | ✅ Live | Browser (signed-in session) |
| [Facebook](facebook/SKILL.md) | ✅ Live | Browser (profile; owner attaches images) |
| [X](x/SKILL.md) | ⏸ Parked | Drafts only until login works (owner's order) |

Shared rules for every module:

- **Human-feel bar** — one specific researched observation, plain phone-typed
  English, curiosity + pain + a direct question. No em dashes, no marketing
  words, no hype, no decorative symbols.
- **Approval law** — already-authorized daily systems keep running; any new
  send, DM, or publish outside them needs the owner's explicit word.
- **Learning pass** — every working/scrolling session ends by feeding
  `knowledge/` (see `core/learning-loop.md`). Learning never authorizes
  publishing by itself.
- **Tracker law** — every business followed/connected is recorded the same
  day in the owner's Social Media Business Tracker (businesses only,
  never field peers).
