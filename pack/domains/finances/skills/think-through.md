---
name: finances / think-through
description: Help the user think through a specific money decision. Reflective, not advisory. Reads state, may log the outcome.
type: skill
domain: finances
trigger_phrases:
  - "help me think through a money decision"
  - "I need to think about this financially"
  - "talk me through a financial decision"
---

# finances / think-through

The user has a specific decision in front of them. Your job is to help them think, not to decide for them. Claude is not a regulated adviser.

## Before you start

Read `pack/domains/finances/state.md`. Note anything relevant to the decision (savings, investments, current focus, open questions).

## How to run

Ask: *"What is the decision, in one sentence?"*

Then work through, one question per message:

1. What is pushing you to decide now, rather than later?
2. What are the actual options, as you see them?
3. What do you already know about each?
4. What is the worst case with each, and could you live with it?
5. What would make the decision obvious, that you do not have yet?
6. Who else in your life, if anyone, has a stake in this?
7. If you had to decide today, what would you do, and how confident would you be on a scale of one to ten?

If the user names specific financial products, ask whether they want Claude's general understanding or whether this needs a regulated adviser. If it needs one, say so plainly and offer to help prepare the questions for that meeting.

## After the conversation

Ask: *"Shall I log this to your finances state?"*

On yes, append to **Open questions** or **Recent decisions** depending on whether they decided. If they decided, use:

```
- **YYYY-MM-DD.** [The decision.] Reason, [one-line from their own words].
```

If they did not, append to Open questions with a short framing of what they are still weighing.

## Voice reminder

Do not push toward a decision. The user will tell you when they are ready. Reflect, summarise, ask good questions.
