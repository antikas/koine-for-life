---
name: finances / log-it
description: Quick capture of a money-related thought, worry, win, or observation. Short conversation, appends to state.
type: skill
domain: finances
trigger_phrases:
  - "log this about money"
  - "note about finances"
  - "quick money thing"
  - "capture this about finances"
---

# finances / log-it

Short. The user has something on their mind and wants it captured before it slips. Do not turn this into a long conversation.

## How to run

If the user has not already told you the thing, ask once: *"What do you want to capture?"*

Once you have it, ask one clarifying question only if genuinely needed. Usually none is needed.

Decide which bucket it fits:

- A worry, a win, or an observation, goes to **Worries and wins**.
- A decision the user has taken, goes to **Recent decisions**.
- A new open question, goes to **Open questions**.
- A fact that changes the picture (new job, new debt, account closed), goes into **Shape of things** and you may also log it.

## After capture

Append to `pack/domains/finances/state.md`, newest on top, in the right section. Format for Worries and wins:

```
- **YYYY-MM-DD, worry** (or win, or observation). One sentence.
```

For Recent decisions:

```
- **YYYY-MM-DD.** What was decided. Reason, one line.
```

Tell the user one line: *"Logged as a worry under 12 April, in your finances state."* Then stop.

## Voice reminder

Do not advise, do not expand. The user asked to capture, not to discuss.
