---
name: health / symptom-log
description: Log a symptom or series of symptoms specifically. Structured capture for later pattern-spotting.
type: skill
domain: health
trigger_phrases:
  - "log a symptom"
  - "record a symptom"
  - "note this symptom"
---

# health / symptom-log

## How to run

Ask if not already given: *"What is the symptom, and when did it happen?"*

Then capture, one question at a time, only the fields that are relevant:

1. What exactly, in your words?
2. When did it start, when did it ease, or is it ongoing?
3. Severity roughly (mild, moderate, bad enough to stop your day)?
4. Anything that made it better or worse?
5. Was there anything unusual before it (food, stress, sleep, training)?

If severity sounds acute (chest pain, severe abdominal pain, neurological symptoms, self-harm thoughts), stop capture and point at real help plainly.

## After capture

Append to Log in `pack/domains/health/state.md`:

```
- **YYYY-MM-DD, symptom.** [What]. Severity, [mild/moderate/bad]. Triggers or context, [one line]. Duration, [one line].
```

If the symptom is recurring, add to Open questions: *"Pattern to watch: [symptom] since [date]."*

## Voice reminder

Record what the user said. Do not diagnose.
