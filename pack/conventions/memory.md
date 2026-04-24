---
name: Memory
description: How the pack stores what it remembers. Where files live, what goes in which folder, when to write.
type: convention
---

# Memory

The pack remembers by writing files. This doc says where to write them and what shape they take.

## Folder layout

```
pack/
  identity/         (who the user is. Written by run-me-first. Rarely changes.)
  memory/           (everything else the user wants remembered.)
  domains/          (per-domain files like finances, family, and so on. Live logs and state.)
```

## Identity

Two files, written by `run-me-first` and only updated when the user explicitly says their situation has changed:

- `identity/user.md`: name, rough context, what they want from this pack, how they want to be spoken to, privacy preferences.
- `identity/people.md`: the people who matter across their life, organised by domain. Names, relationships, relevant notes.

## Memory

Free-form. Each file is one topic. The file name is a short kebab-case slug. Examples:

- `memory/kitchen-refit-2026.md`
- `memory/pension-rebalance-2026.md`
- `memory/reading-support-plan.md`

When writing a new memory file:

1. Check if an existing file already covers the topic. If yes, update it.
2. If writing a new file, add one line to `memory/INDEX.md` pointing to it.
3. Lead with a one-line description. Keep it append-friendly, a log shape rather than an essay.

## Domain files

Each active domain has its own folder. Files inside are domain-specific (see each domain's README). Typical pattern: a `state.md` for current state, a `log.md` for append-only history, and optionally per-topic files.

## When to write

Write when:

- The user tells you a fact you will need next time.
- A decision is made, with what and why and what would need to be seen to change minds.
- A review happens, capturing the state and what was noticed.
- The user says "remember this" or similar.

Do not write when:

- The conversation is exploratory and nothing is settled.
- The information is already in an existing file (update instead).
- The user has not asked and it is ephemeral (a passing question, a stray thought).

## When to update vs. append

- **Update** when a fact has changed, such as the user's address, a position they hold, or a decision that supersedes an earlier one. Mark the change briefly.
- **Append** when something happened, such as a review, a purchase, an outing, or a conversation. Logs grow, they do not get rewritten.

## Naming and dates

Dates in file content use `YYYY-MM-DD`. Relative dates in user messages ("last Thursday") are converted to absolute dates before writing.

File names do not include dates unless the file is inherently a dated artefact (for example `reviews/2026-04-monthly.md`).
