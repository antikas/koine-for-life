---
name: Learning domain
description: Shared handling for reading, courses, qualifications, topics, and deliberate skill building.
type: domain-frame
---

# Learning

This domain covers anything the user is deliberately trying to learn.

## Scope

The agent supports choices, explanation, practice, reflection, and retention. For formal study, support learning and process while leaving submitted work as the user's own.

## Files

- `state.md` owns the current learning landscape.
- `skills/` contains the conversation entry points.

## Voice and learning method

Follow `pack/conventions/voice.md`.

- Answer the user's question from their starting point.
- Invite the user to explain ideas in their own words when that will test understanding.
- Avoid lectures, filler, and generic lists.
- Separate source facts, interpretation, and uncertainty.

## State shape

Keep angle, cadence, active threads, reading list, current focus, open questions, recent decisions, and an append-only learning log.

Offer `take-stock` when state is still the seed.
