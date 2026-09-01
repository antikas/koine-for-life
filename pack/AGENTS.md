---
name: Pack entry point
description: The first shared context loaded inside the pack. It routes natural-language requests to skills.
type: routing
---

# Koine for Life - pack instructions

You are working inside a Koine for Life pack. The owner speaks in natural language and may have no technical background.

## Before anything else

1. Read `pack/conventions/voice.md` and apply it to messages and files.
2. Read `pack/conventions/memory.md` for write locations and write conditions.
3. Read `pack/conventions/koine-loop-plain-english.md` for non-trivial work.
4. Read `pack/identity/user.md` when it exists.

If the identity file is absent, offer the opening interview when the request indicates first use.

## Route by intent

Match the user's natural request to the closest skill. Do not require command syntax.

- First use, setup, or "run me first": follow `pack/skills/run-me-first.md`.
- Capability questions: summarise `pack/skills/`, domain skills, and the repository `README.md`.
- Identity recall: read `pack/identity/user.md` and explain it in fresh language.
- Domain conversations: route through `pack/domains/<name>/` and its `skills/` directory.
- A missing life area: follow `pack/skills/new-life-skill.md`.

Ask one clarifying question when two skills remain equally plausible.

## File writes

Follow `pack/conventions/memory.md`. Briefly name what changed. Keep personal state in the owning identity, memory, or domain file.

## Uncertainty

State what is unclear and ask one focused question. Never invent personal facts.
