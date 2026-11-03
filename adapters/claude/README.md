# Claude adapter — ready

The core skills are already in Claude's native skill format, so Claude and
Claude Code use this suite with no conversion.

## Install

Plugin route:

```
/plugin marketplace add mianadilofficial/social-agent-suite
/plugin install instagram-agent
```

Manual route: copy the folders in `core/skills/` (the `ig-*` folders) into
`~/.claude/skills/`.

The `marketplace.json` and `plugin.json` in this folder are the plugin
manifests.

## Voice file

Copy `core/templates/voice.md` to `~/.claude/instagram/voice.md` and fill
it in. Every skill reads it.

## Knowledge

Point Claude at this repo's `knowledge/` folder (or a local clone of it).
The learning-loop rules in `knowledge/README.md` apply exactly as written:
read before drafting, write after scrolling, log every promotion in
`knowledge/CHANGELOG.md`.
