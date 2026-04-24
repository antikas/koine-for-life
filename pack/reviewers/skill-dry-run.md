---
name: skill-dry-run
description: Walk through a skill file as if it were being invoked, to surface gaps, ambiguities, and failure modes before real use.
type: reviewer
trigger_phrases:
  - "dry run this skill"
  - "test the skill"
  - "check this skill before I use it"
---

# skill-dry-run

A new skill gets one shot at a first real invocation. This reviewer pressure-tests it first.

## Before you start

Read `pack/conventions/voice.md`, `pack/conventions/memory.md`, and the skill file being reviewed.

## How to run

Ask: *"Which skill file, and is this a new skill or a change to an existing one?"*

Then:

### 1. Structural check

Verify the file has:

- Frontmatter with name, description, type, trigger_phrases, and domain if applicable.
- A framing paragraph.
- A "Before you start" section naming which state file, if any, to read.
- A "How to run" section with questions in order.
- An "After the conversation" section saying exactly what to write and where.
- A "Voice reminder" section.

Flag any missing pieces.

### 2. Trigger check

Look at the trigger phrases. Ask: *"Say one of these out loud. Does it sound like you? If not, which would you actually say?"*

If trigger phrases feel generic or un-civilian, suggest better ones from the user's own recent messages.

### 3. Conversation walk-through

Pretend to be the user, picking a plausible invocation. Walk through the questions one by one. At each, ask the writer (the real user):

- Is this question clear?
- Is it in your voice?
- Is it in the right order?
- Does it actually move things toward the write-back?

Note any question that is vague, generic, or redundant.

### 4. Write-back check

Look at "After the conversation". Ask:

- Does it name the exact file?
- Does it name the exact section?
- Does it specify the format (a bullet, a block, a rewrite)?
- Does it preserve existing content where relevant?
- Is the date format specified?

Flag any "update state.md" without specifics. That is a fail.

### 5. Overlap check

Scan the rest of the pack for skills with similar triggers or purpose. If overlap exists, name it and ask whether to extend the existing skill instead.

### 6. Voice pass

Run the skill file through the `voice-check` rules (you can call that reviewer or apply the rules yourself).

## Report

Give the user:

- A headline: ready to ship, needs small fixes, needs rework.
- A short list of specific issues with line references.
- A recommendation for the first fix.

## Voice reminder

Be specific. "This question is vague" is useless. Name which question and what would make it specific.
