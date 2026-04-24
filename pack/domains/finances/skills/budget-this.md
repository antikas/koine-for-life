---
name: finances / budget-this
description: Plan a specific spend. Holiday, kitchen, car, school fees, a gift. Concrete, bounded, produces a number.
type: skill
domain: finances
trigger_phrases:
  - "help me budget this"
  - "budget a holiday"
  - "budget for the kitchen"
  - "plan spending for"
---

# finances / budget-this

The user has a specific spend in mind and wants to think it through before committing. Output is a rough number and the bits it is made of, not a line-by-line spreadsheet.

## Before you start

Read `pack/domains/finances/state.md`. Note their current focus and any existing savings pots.

## How to run

Ask: *"What are we budgeting for, and when does it need to happen?"*

Then, one at a time:

1. What are the known pieces that make it up? (For a holiday, flights, accommodation, food, activities. For a kitchen, cabinets, appliances, labour, unknowns.)
2. For each piece, what is a rough figure, even if wide?
3. What pieces are you unsure about?
4. What is the "fine" number in your head, and what is the "too much" number?
5. Where is the money coming from? Savings, income smoothing, borrowing?

## After the conversation

Lay the budget back as a short list with rough figures and a total. Mark the uncertain bits clearly. Compare the total to the user's "fine" and "too much" numbers.

Ask: *"Does the shape of that feel right?"*

If they adjust, do it with them. When they are settled, ask to log. On yes, append to Recent decisions:

```
- **YYYY-MM-DD.** Budgeted [item], rough total [X], from [source]. Known unknowns, [list].
```

## Voice reminder

Do not add prudence the user did not ask for. If they have decided to splash out, help them plan it well, not talk them out of it.
