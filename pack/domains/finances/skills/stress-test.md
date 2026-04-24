---
name: finances / stress-test
description: Walk through a "what if" scenario the user is worried about, so they see it clearly rather than carrying it vaguely.
type: skill
domain: finances
trigger_phrases:
  - "stress test my finances"
  - "what if I lose my job"
  - "what if the market drops"
  - "worst case money scenario"
---

# finances / stress-test

The user wants to look at a worst-case. This is often more calming than avoiding it, because a vague fear is worse than a clear one. Claude's job is to help them see the scenario, not to reassure them falsely.

## Before you start

Read `pack/domains/finances/state.md`. You need the shape of things and the cadence before you can help here.

## How to run

Ask: *"What is the scenario you want to look at?"*

Once you have it (job loss, income drop, market fall, big unexpected cost, partner's work change, illness), ask one at a time:

1. How likely do you think this is, roughly? (Not a probability, a gut sense.)
2. If this happened tomorrow, what would go wrong first?
3. How long would your current savings or buffer cover?
4. What would you cut first?
5. What would you not cut, even under pressure?
6. Is there anything you could do now that would make the scenario easier if it came?

## After the conversation

Summarise in two or three sentences what the user would actually do if this happened. Do not soften. If the picture is bleak, say so plainly.

Ask: *"Want me to add any of this to your current focus or open questions?"*

Append concrete actions to Current focus only. Append any "I do not know" to Open questions. Log the scenario run in Recent decisions with:

```
- **YYYY-MM-DD.** Stress-tested scenario, [one-line]. Outcome, [one line].
```

## Voice reminder

Do not reassure. Do not minimise. If the user finds the exercise settling, that is from the clarity, not from you telling them it will be fine.
