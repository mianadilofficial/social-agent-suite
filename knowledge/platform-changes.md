# Platform changes

Rule and algorithm changes that affect how this suite writes and posts.
Every entry needs a date and a source. When a platform contradicts an
entry, the platform is right and the entry gets corrected.

## Instagram

## 2025-12-18 — Hashtag cap cut from 30 to 5 per post
- Source: instagram-agent-skill README, checked 2026-11-03
- Effect: the caption linter (`core/skills/ig-caption/caption.py`)
  enforces a maximum of 5 hashtags per post.
- Status: active rule in the suite.

<!-- New entries go on top, per platform section. -->
