---
name: voice-check
description: Review a file or a recent message against pack/conventions/voice.md. Report findings and offer fixes.
type: reviewer
trigger_phrases:
  - "check the voice"
  - "voice review"
  - "does this sound right"
---

# voice-check

Apply the voice rules to a specific piece of text. The user asks this when something feels off, or before they send something written by Claude or by themselves.

## Before you start

Read `pack/conventions/voice.md` fully. You will check against both the principles and the hard rules.

## How to run

Ask: *"What are we checking? A file path, a recent message, or something you want to paste in?"*

Once you have the text, work through in this order:

### 1. Hard rules (non-negotiable)

For each, report hits with line or phrase:

- Em dashes (`—`) or en dashes (`–`). Only ASCII hyphens allowed.
- "Not X, but Y" or "It is not X, it is Y" constructions.
- Staccato short-sentence sequences of three or more.
- "Your X... Your Y..." LinkedIn-style openings.
- "Let me share", "Here's the thing", "Let us unpack".
- Rhetorical questions as section openers.
- Banned vocabulary: leverage, robust, unlock, empower, nascent, paradigm, nuanced, multifaceted, landscape, synergy, ecosystem, holistic.
- Sentences over 40 words.
- AI brand names in written artefacts (except where the product context genuinely requires it).

### 2. Principles (judgement calls)

- Plain English. Jargon without gloss?
- Direct, not brusque. Padding?
- Over-structured for a simple thing?
- Summaries at the end of every message?
- Corporate tone ("going forward", "utilising")?

### 3. Report

Give the user:

- A short "passes" or "fails" headline.
- Hard rule hits as a list, with the offending phrase quoted.
- Principle-level observations as a short paragraph.
- Offer to produce a revised version that fixes the hard-rule hits (principles are the user's call).

## If they want fixes applied

Apply only the hard-rule fixes unless the user explicitly asks for a rewrite. Show the diff, not a full rewrite, where possible.

## Voice reminder

Do not use the voice rules in a way that violates them. Plain English when explaining what you found.
