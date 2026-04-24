---
name: finances / take-stock
description: First-time deep interview about the user's finances. Populates state.md from a thin seed. Run once per major life change.
type: skill
domain: finances
trigger_phrases:
  - "help me with finances"
  - "let's look at my money"
  - "take stock of finances"
  - "I want to sort out my money"
  - "get my finances in order"
---

# finances / take-stock

This is the deeper interview for the finances domain. Run it the first time the user engages seriously with this area, and again after a major life change (move, job change, big windfall, big loss).

## Before you start

Read `pack/domains/finances/state.md`. If it has real content already, this is a re-take, not a first run. Tell the user what is already there and ask what has changed, rather than re-interviewing from scratch.

If the state is still the thin seed, proceed.

## How to run

One question per message. Wait for the answer. Do not stack. If the user sounds reluctant on a topic, skip and come back later. Capture numbers only where the user offers them. Do not press for precision.

## The questions

Ask these in order, in your own words, with short follow-ups where something is interesting.

1. What is actually going on in money in your life right now? Any recent change, good or bad?
2. Who earns in the household, and how stable is that?
3. What are the big fixed things going out each month? Roughly is fine.
4. Do you have savings set aside? Roughly how much, and what is it for?
5. Any investments? Just the broad shape, not every position.
6. Any debts, other than a mortgage?
7. Pension. Do you have one, are you contributing, and do you have a sense of it?
8. What is the biggest money decision on your mind right now?
9. What money worry sits with you most often?
10. What would "finances in good shape" actually look like for you in a year?

## After the conversation

Summarise back what you heard, in plain English, short. Ask: *"Shall I write this into your finances state file?"*

On yes, rewrite `pack/domains/finances/state.md`. Preserve the frontmatter, set `last-deep-review` to today. Fill:

- Angle (from questions 1, 8, 10).
- Shape of things (from 2 through 7).
- Current focus (from 8).
- Open questions (from 9 and anything else that surfaced).
- Leave Recent decisions and Worries and wins untouched if they have content. If empty, seed with nothing.

Name the file you wrote when you are done. Say briefly what you put where.

## Voice reminder

Money is emotional. Do not summarise their situation as a problem statement. Reflect it back as they described it.
