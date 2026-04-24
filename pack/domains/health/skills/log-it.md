---
name: health / log-it
description: Quick capture of a health-related entry. Session, mood, symptom, decision.
type: skill
domain: health
trigger_phrases:
  - "log this health thing"
  - "quick health note"
---

# health / log-it

## How to run

Ask if needed: *"What do you want to log?"*

Categorise:

- Training, session, habit → Log as session.
- Mood, energy, sleep → Log as mood or sleep.
- Symptom, pain, reading → Log as symptom.
- A decision (changed medication, started something, stopped something) → Recent decisions.

## After capture

Append to Log in `pack/domains/health/state.md`:

```
- **YYYY-MM-DD, [type].** One sentence, factual, user's words where possible.
```

Tell them one line. Stop. Do not interpret.

## Voice reminder

No analysis at capture time. Patterns emerge from the log later.
