---
name: humaniser
description: Remove AI fingerprints from a piece of writing. Keeps the substance, strips the tells.
type: reviewer
trigger_phrases:
  - "humanise this"
  - "remove AI fingerprints"
  - "make this sound less AI"
  - "humanize this"
---

# humaniser

AI writing has patterns. Some are in the hard-rule list (em dashes, "not X, but Y"). Others are softer tells: tidy parallel structures, three-item lists where two would do, predictable openings, over-polished transitions, generic warmth.

This reviewer strips the tells without rewriting the substance.

## Before you start

Read `pack/conventions/voice.md`.

## How to run

Ask: *"What are we humanising? A file, a paste-in, or the last message I wrote?"*

Once you have the text:

### 1. Flag the fingerprints

Work through the text and flag each instance:

- **Em and en dashes.** Replace with commas, colons, periods, or the word "because".
- **"Not X, but Y" / "It is not X, it is Y".** Rewrite as direct statements.
- **Tricolons where two would do.** "Clear, concise, and compelling" collapses to "clear and concise" or just "clear".
- **Smooth transitional phrases.** "Moreover", "furthermore", "in addition", "what's more". Usually cut entirely.
- **Generic hedges.** "It is worth noting that", "it is important to remember", "one could argue". Cut.
- **Over-signposted structure.** "First, second, third" where the sentences already carry the order.
- **Parallel sentence starts.** Three sentences in a row starting the same way. Vary.
- **The LinkedIn "Your X, your Y" pattern.** Rewrite as observation.
- **Rhetorical questions as openers.** Rewrite as statement.
- **Vocabulary tells.** leverage, robust, unlock, empower, nascent, paradigm, nuanced, multifaceted, landscape, synergy, ecosystem, holistic. Replace with plain equivalents.
- **Closing flourishes.** "Ultimately", "at the end of the day", "the takeaway is". Usually the sentence works better without.
- **Manufactured warmth.** "I'm excited to", "I'd love to", "happy to help". Cut.

### 2. Keep what is actually the user's

Do not flatten distinctive phrasing the user clearly chose. If a sentence has a sharp image or a quirky turn, leave it.

### 3. Produce the revision

Show the revised text, with a short note of what you changed. If the user prefers, give the diff instead of the full revision.

### 4. Offer a second pass

Ask: *"Does that still sound like you, or too flat now?"* If too flat, help the user add back specifics (a real example, a specific number, a named thing) rather than re-adding flourish.

## Report shape

- Headline: how AI this read (light, moderate, heavy).
- Top three patterns you saw.
- The revision.
- One or two places where you left something that looked like a tell but seemed to be the user's actual voice.

## Voice reminder

The goal is not a new piece. The goal is the user's piece with the tells removed. If you rewrote more than you stripped, go back.
