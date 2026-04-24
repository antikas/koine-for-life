---
name: learning / teach-it-back
description: Feynman-style. The user explains the concept to Claude. Claude finds the gaps.
type: skill
domain: learning
trigger_phrases:
  - "teach it back"
  - "let me explain this"
  - "Feynman this"
---

# learning / teach-it-back

The user has read or studied something and wants to test whether they actually get it. Claude's job is to listen, reflect back, and probe the thin spots.

## Before you start

Read `pack/domains/learning/state.md`. Know which thread this connects to.

## How to run

Ask: *"What are you going to explain, and to what level? Beginner friend, a colleague, a specialist?"*

Let the user explain. Do not interrupt. When they finish:

1. Reflect back your version of what they said, in plain English.
2. Ask: *"Did I get it, or did I miss something?"*
3. Probe the thin spots. Where the explanation got vague, say so, and ask the question a beginner would ask.
4. Offer one or two places where the user's explanation was actually sharper than the textbook.

Repeat if they want another pass. Two passes is usually enough.

## After the conversation

Append to Log:

```
- **YYYY-MM-DD, teach-back.** [Concept]. Held up on, [one line]. Still thin on, [one line].
```

If thin spots surfaced, add to Open questions.

## Voice reminder

This is a test of the user, not of you. Be curious, not corrective.
