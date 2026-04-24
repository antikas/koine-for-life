---
name: finances / whats-changed
description: Reconcile the gap between state.md and reality since the last check-in. Catch drift before it piles up.
type: skill
domain: finances
trigger_phrases:
  - "what's changed in my finances"
  - "catch up my money"
  - "reconcile my finances"
---

# finances / whats-changed

Lighter than a check-in. The user just wants to bring the state file back in line with reality. Receipts, a new bill, an account change, a decision they already took but did not log.

## Before you start

Read `pack/domains/finances/state.md`. Note the date of the last update and the current Shape of things.

## How to run

Ask: *"What has actually changed since we last looked?"*

Let them talk. Do not interrupt with structure. When they pause, ask:

1. Anything you decided that we did not log?
2. Anything new on the worry side, or that has eased?
3. Anything in the shape of things that is now different (new account, closed account, new debt, new income)?

## After the conversation

Update `pack/domains/finances/state.md`:

- Shape of things, where it changed.
- Recent decisions, for anything the user took without logging.
- Worries and wins, append new entries.
- Open questions, add or close as needed.

Tell the user, in two or three lines, what you changed.

## Voice reminder

This is maintenance. Short, businesslike, warm. No deep questions here.
