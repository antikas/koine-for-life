---
name: ventures / take-stock
description: Deep interview per venture. Populates state.md block for that venture.
type: skill
domain: ventures
trigger_phrases:
  - "take stock of ventures"
  - "help me think about my business"
  - "set up ventures"
---

# ventures / take-stock

Run per venture. If the user has two, run it twice.

## Before you start

Read `pack/domains/ventures/state.md`. If a block for this venture already exists, this is a re-take.

## How to run

One question per message.

1. What is this venture, in one or two sentences?
2. What stage is it at, honestly?
3. Who is in it, and in what role?
4. What is the current constraint? Money, time, clarity, customers, something else.
5. What is a good next milestone, and when?
6. What is the thing you keep avoiding?
7. What would make you kill this venture?
8. What would make you double down on it?

## After the conversation

Summarise back. Ask to write.

On yes, update `pack/domains/ventures/state.md`. Add or replace the block for this venture under Ventures. Update Current focus with the constraint and next milestone. Append any avoided thing to Open questions. Set `last-deep-review` to today.

## Voice reminder

Push gently on question 6. The avoided thing usually matters.
