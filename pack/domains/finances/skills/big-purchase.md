---
name: finances / big-purchase
description: Walk through a major buy before committing. Car, house move, big piece of kit, a family-size decision.
type: skill
domain: finances
trigger_phrases:
  - "big purchase decision"
  - "buying a car"
  - "thinking about buying"
  - "major purchase"
---

# finances / big-purchase

A proper purchase conversation. This is more than `think-through` because big buys have a ritual: research, short-list, decide, buy, live with it. Claude helps at whichever stage the user is in.

## Before you start

Read `pack/domains/finances/state.md`. Note Current focus, any ongoing savings pot, and any related open question.

## How to run

Ask: *"What are you thinking of buying, and where are you in the process?"*

Depending on the stage, run the matching block. Do not run them all.

### Early (still deciding whether to buy at all)

1. What is driving this? A need, a want, a replacement, a change of circumstance?
2. What happens if you do not buy it this year?
3. What would you have to give up to buy it?
4. What would buying it change, day to day?

### Middle (narrowing options)

1. What are the real contenders, not the longlist?
2. For each, what do you know about the total cost of ownership, not just the sticker?
3. What have you heard from people who already have one?
4. What would decide it for you?

### Late (about to buy)

1. What has changed in your view since you started looking?
2. Is there anything you are pretending does not matter, that actually does?
3. Walk me through the first three months with this thing. What does it actually look like?

## After the conversation

Depending on stage, append to Current focus (early), Open questions (middle), or Recent decisions (late):

```
- **YYYY-MM-DD.** Decided to [buy/postpone/cancel] [item]. Reason, [one line].
```

## Voice reminder

Do not shame spending. Do not cheerlead either. Stay level.
