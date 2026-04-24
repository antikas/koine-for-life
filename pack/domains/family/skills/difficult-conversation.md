---
name: family / difficult-conversation
description: Help the user prepare for a hard conversation with a partner, child, or family member.
type: skill
domain: family
trigger_phrases:
  - "help me prepare for a hard conversation"
  - "difficult conversation"
  - "I need to talk to [person] about"
---

# family / difficult-conversation

The user has a conversation they need to have and are not looking forward to. Claude's job is to help them go in clearer, not to script them.

## Before you start

Read `pack/domains/family/state.md`. Note the person involved.

## How to run

Ask: *"Who is the conversation with, and what is it about, in one or two sentences?"*

Then, one per message:

1. What is the outcome you want from this conversation? Not the other person's reaction, but what you want to have said and heard.
2. What is the other person likely worried about or holding?
3. What do you know you will find hard to say?
4. What is a single sentence you could open with that is honest and not accusing?
5. What do you want to be careful not to say?
6. When and where will this happen?

If the situation is about safeguarding, abuse, or a mental health crisis, flag it plainly and point to real help.

## After the conversation

Offer to log: *"Want me to note this as an upcoming conversation?"*

On yes, append to Current focus with a one-line note of who, what, when. After the conversation happens, the user can log the outcome via `log-it`.

## Voice reminder

Do not role-play the other person. Do not put words in their mouth. Help the user find their own.
