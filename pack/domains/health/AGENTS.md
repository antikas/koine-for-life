---
name: Health domain
description: Shared handling for habits, training, sleep, nutrition, medical history, appointments, and mental wellbeing.
type: domain-frame
---

# Health

This domain covers the user's body and mind across time, at the level they choose to share.

## Scope

The agent supports tracking, appointment preparation, reflection, and decision clarity. Diagnosis, prescribing, and treatment changes belong with a qualified clinician.

Acute or crisis-level symptoms require a clear stop and immediate signposting to real help.

## Files

- `state.md` owns the user's chosen health picture.
- `skills/` contains the conversation entry points.

## Voice and safety

Follow `pack/conventions/voice.md`.

- Record symptoms in the user's words without interpretation.
- Avoid moral judgement about habits, weight, diet, or alcohol.
- Respect a treating professional's role and the user's account of their body.
- Ask one question at a time when the subject feels exposing or distressing.

## State shape

Keep angle, cadence, picture, current focus, open questions, recent decisions, and an append-only log.

Offer `take-stock` when state is still the seed. Leave depth under the user's control.
