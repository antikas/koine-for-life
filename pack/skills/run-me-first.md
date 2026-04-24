---
name: run-me-first
description: The opening interview. Personalises the pack on first use. Writes identity files and seeds the seven life domains. Has a fresh path and an existing-vault bootstrap path.
type: skill
trigger_phrases:
  - "run me first"
  - "I'm new"
  - "let's start"
  - "set this up"
  - "first run"
---

# run-me-first

This is the most important conversation in the pack. Get it right and everything else follows. Get it rushed and the user will be re-explaining themselves for months.

## What you are doing

You are going to interview the user so the pack can know who they are, who matters to them, what they want help with, and how they want to be spoken to. At the end, you will write:

- `pack/identity/user.md`
- `pack/identity/people.md`
- `pack/memory/INDEX.md` seeded with a first few topics if any surfaced
- One starter file per domain the user opted into, under `pack/domains/[name]/state.md`

Follow `pack/conventions/voice.md` throughout. One question at a time. No stacked questions. No breezy tone. No summaries at the end of every message.

## Fresh path vs. existing-vault path

Before asking anything, decide which path to take.

**Existing-vault path.** Check whether any of these exist anywhere reachable from the pack folder, or one level up:

- A file called `VAULT_INDEX.md` or `MEMORY.md`.
- A folder called `knowledge/`, `vault/`, or `projects/` at a sibling level to this pack.
- Files inside this pack's `identity/` that already have content.

If any are present, ask the user: *"It looks like you already have a knowledge vault or notes system alongside this pack. Would you like me to read it and build on what's there, or start fresh?"* If they say build on it, go to the **existing-vault path** below. If they say start fresh, or nothing is found, go to the **fresh path**.

## Fresh path

Run through these in order, one question per message, writing nothing until the user has answered all of them. Then confirm the write before saving.

### 1. Welcome and frame

Open with a single message that says, in your own words:

- What this is (a second brain that keeps notes on their computer).
- What you are about to do (ask them about themselves for about twenty minutes).
- That they can skip any question, and change anything later.
- That the goal is not a filled-in form, it is a real conversation.

Then pause. Wait for them to be ready.

### 2. Who they are

Ask, in order, pausing for each answer:

1. What should the pack call them? (Name, or what they prefer to be called.)
2. Where do they live, roughly? (City or region. Do not ask for address.)
3. Who else is in the household? (Partner, children, anyone else. Ages roughly if children.)
4. What do they do, roughly? (Work, study, retired, looking.)

Keep the tone like a new friend over coffee. Do not tick off a form.

### 3. Why they are here

Ask: *"What made you decide to try this? What are you hoping to stop forgetting, or to think through better?"*

Listen for the real thing. If they give a generic answer ("be more organised"), ask once more: *"What would being more organised actually change for you day to day?"* Do not push further than that.

### 4. How they want to be spoken to

Ask: *"Do you want me to be brief and direct, or warmer and more conversational? And how much pushback do you want when you are making a decision, none, some, or a lot?"*

Capture the answer literally. This drives tone for every future conversation.

### 5. Seven domains

Explain, plainly, that the pack is organised into seven areas of life, and you will ask about each briefly. They can opt any in or out.

For each domain, ask two questions and move on. Do not go deep. Depth comes later.

**Finances.** "Do you want help with this area? If yes, what is the main thing, day-to-day money, bigger decisions, investments, or something else?"

**Family.** "Do you want help here? If yes, is it mostly about the children, your partner, extended family, or the household running?"

**Ventures.** "By ventures I mean anything you are building or running, a business, a side thing, a serious project. Do you want help here, and with what?"

**Career.** "By career I mean how you earn a living and the arc of your working life. Do you want help here? If yes, is it mostly the current role, a transition you are thinking about, or the longer-term direction?"

**Health.** "Do you want help here? Habits, training, medical decisions, or something else?"

**Learning.** "Do you want help here? Reading, courses, a qualification, a specific topic you are working through?"

**Hobbies and interests.** "Anything you do for the love of it that you would like to track or think about? Examples are music, sports, cooking, a craft, horse riding."

For each yes, note the specific angle in your head. You will use it when writing the domain starter file.

### 6. People who matter

Ask: *"Who are the people I should know about across the parts of life you said yes to? Family, close friends, colleagues, teachers, coaches, advisers, anyone who comes up often."*

Let them list. Ask, one at a time, a sentence each: *"And [name] is?"* Capture name, relationship, and anything they volunteer (often a detail, a current situation, a sensitivity). Do not dig.

### 7. Cadence

Ask: *"How often would you like me to nudge you for reviews? Weekly, monthly, termly, annually, or only when you ask?"*

Capture per domain if they give different answers.

### 8. What not to bring up

Ask: *"Is there anything you do not want me to raise unless you raise it first?"*

This is important. Some people have a topic that is theirs to open. Respect it.

### 9. Privacy check

Remind them, briefly, that the pack keeps files on their computer and that Anthropic processes conversations during a chat. Point at `PRIVACY.md`. Ask: *"Anything you want to keep out of this pack on principle?"* Note it.

### 10. Confirm and write

Summarise, in your own words, what you heard. Short. Then say: *"I am going to write four or five starter files based on this. You can edit anything after. Shall I go ahead?"*

On yes, write:

- `pack/identity/user.md` with name, location, household, work, what they said they want from the pack, tone preference, pushback preference, and privacy notes.
- `pack/identity/people.md` with the people they mentioned, grouped by domain.
- For each domain they opted into, `pack/domains/[name]/state.md` with a one-paragraph description of their specific angle, their chosen cadence, and an empty "current focus" and "open questions" section.
- `pack/memory/INDEX.md` with one line per domain starter file.

After writing, say briefly what you wrote and where. Point them at the README for the phrases that open each part of the pack. End with: *"Welcome in."*

## Existing-vault path

The user already has notes. Your job is to bootstrap from them rather than re-interview.

### 1. Ask permission and locate

Ask: *"Tell me where your existing notes live, or let me guess from the folder structure. I will read what is there before asking anything."*

Find and read, in order if present:

- `VAULT_INDEX.md` or any root index.
- `MEMORY.md`.
- `identity/` or `user_profile.md` or equivalent.
- Any dashboard or `status/` folder.
- Any `CLAUDE.md` at the vault root.

### 2. Reflect back

In a single message, tell them in plain English what you learned about them from the vault. Name, work, household, active projects, recent focus. Keep it factual, not flattering.

Ask: *"Is that still right? Anything out of date?"*

### 3. Fill the gaps specific to koine-for-life

Run only the fresh-path questions that the existing vault did not already answer. Typically:

- Tone and pushback preference, if not captured.
- Which of the seven domains are in scope for this pack (they may want to keep some things outside it).
- Cadence preferences.
- What not to bring up.

One question at a time.

### 4. Confirm and write

Write `pack/identity/user.md` and `pack/identity/people.md` using what the existing vault already told you, with the gaps filled in from the conversation. Cite the source file for anything carried across, so a future session can trace it.

Seed `pack/domains/[name]/state.md` only for domains the user said are in scope for this pack. For anything that lives in the outer vault (for example a big project that is not part of daily life review), link to it rather than duplicating.

End the same way: *"Welcome in."*

## Quality gate before declaring done

Before marking run-me-first complete, check:

- Every file written passes the voice rules in `pack/conventions/voice.md`. No em dashes, no "not X, but Y", no staccato.
- `pack/identity/user.md` captures tone and pushback preference explicitly.
- The user has confirmed the summary before files were written.
- `pack/memory/INDEX.md` has a line per starter file.

If any of these fail, fix before closing the conversation.
