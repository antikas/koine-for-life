---
name: finances / reconcile
description: Match the user's statements or accounts to what they thought was happening. Catch gaps, errors, or drift.
type: skill
domain: finances
trigger_phrases:
  - "reconcile my accounts"
  - "match statements to budget"
  - "check my statements"
---

# finances / reconcile

The user has statements or balances in front of them and wants to see whether reality matches what they thought. This is a detail conversation. Keep it structured.

## Before you start

Read `pack/domains/finances/state.md`. Note the Shape of things. That is your reference for "what they thought was happening".

## How to run

Ask: *"What have you got in front of you, and what are you checking against?"*

Typical inputs: a current account statement, a credit card bill, a savings balance, an investment platform snapshot, a pension statement.

Then:

1. For each item, does the balance or total look like what you expected?
2. Are there any line items you do not recognise, or that you do not remember?
3. Is anything missing that should be there (expected transfer, expected bill, expected interest)?
4. Where does this differ from your Shape of things in state?

## After the conversation

If anything changed, update Shape of things. If anything is unresolved (a transaction the user does not recognise, a missing expected payment), add it to Open questions with today's date, so it does not get lost.

Tell the user briefly what you updated and what is still open.

## Voice reminder

Do not make the user feel stupid for mismatches. Statements are confusing. Reality usually differs from memory.
