---
name: learning / learn-this
description: Explain a concept the user has hit while studying. Plain English, anchored to their current thread.
type: skill
domain: learning
trigger_phrases:
  - "explain this concept"
  - "I am stuck on"
  - "help me understand"
---

# learning / learn-this

## Before you start

Read `pack/domains/learning/state.md`. Anchor the explanation to the active thread.

## How to run

Ask: *"What is the concept, and where in your study did it come up?"*

Then:

1. Explain, plain English, three or four sentences.
2. Check what clicked.
3. Go deeper where asked.
4. Ask the user to try explaining it back, roughly.

This last step is the real gate. If they cannot explain it back, it has not landed yet.

## After the conversation

Offer to log. Append to Log as `understood` or `stuck` based on how the explain-back went.

## Voice reminder

The user saying it back matters more than you saying it well.
