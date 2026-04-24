---
name: finances / check-in
description: Periodic review of the user's finances at the cadence they chose. Short, conversational, updates state.
type: skill
domain: finances
trigger_phrases:
  - "finances check-in"
  - "money check-in"
  - "let's review my finances"
  - "time for a money review"
---

# finances / check-in

A short, regular review. This is not a deep reset. It is a way to catch drift, notice what changed, and keep `state.md` honest.

## Before you start

Read `pack/domains/finances/state.md`. Note the date of the last deep review and the current focus items.

## How to run

One question per message. Keep it light. Aim for fifteen minutes, not an hour.

Ask, in order:

1. Since we last looked, what has actually changed in money? Income, outgoings, anything unusual.
2. Looking at what we said was your current focus last time, where are each of those things now?
3. Anything new worrying you, or anything that has eased?
4. Any decisions you have taken since last time that should go on the record?
5. Is your current focus still the right focus for the next period, or should it shift?

## After the conversation

Summarise back. Short. Ask to write.

On yes, update `pack/domains/finances/state.md`:

- Shape of things, only where the user told you something that changes it.
- Current focus, rewrite if it shifted.
- Open questions, add new ones and tick off any that closed.
- Recent decisions, append anything new from question 4 with today's date and a one-line reason.

Do not touch Angle or Cadence unless the user explicitly changed them.

Tell the user briefly what you updated and where. Do not write a long summary.

## Voice reminder

This is a check-in, not an audit. Do not score or grade the user's progress.
