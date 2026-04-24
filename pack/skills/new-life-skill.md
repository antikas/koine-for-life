---
name: new-life-skill
description: Create a new skill in the pack by conversation. The user does not need to know the file format. Adds to an existing domain or creates a cross-cutting skill.
type: skill
trigger_phrases:
  - "new life skill"
  - "add a new skill"
  - "I want a new skill for"
  - "create a skill that helps me"
  - "add this to the pack"
---

# new-life-skill

This is how the user grows the pack. They describe a recurring conversation or task they want Claude to handle the same way each time, and you turn it into a skill file. Quality matters here. A sloppy skill is worse than no skill, because it will be triggered and do the wrong thing.

## Before you start

Read `pack/conventions/voice.md` and `pack/conventions/memory.md`. The skill you write will be held to both. Also glance at the existing skills in the relevant domain, if the user has picked one, so you can check for overlap.

## How to run

One question per message. Do not rush this. It usually takes fifteen to thirty minutes.

### 1. What is it for

Ask: *"What is the recurring thing you want help with, in your own words?"*

Let them describe it in their own language. Do not jump to a skill name. Do not offer a template.

### 2. Check for overlap

In your head, scan the skills that already exist in the domain the user seems to be describing, and across domains. If something close already exists, tell the user:

*"There is already a skill called [X] in [domain] that does something similar. Do you want to extend that, or is this genuinely different?"*

If they want to extend an existing skill, stop this skill and go into edit mode on the existing file. One place for each thing.

If it is genuinely new, continue.

### 3. Where it belongs

Ask: *"Does this live in one of the seven domains (finances, family, ventures, career, health, learning, hobbies), or is it cross-cutting?"*

If cross-cutting, it goes under `pack/skills/`. If domain, it goes under `pack/domains/[name]/skills/`.

### 4. What triggers it

Ask: *"What would you actually say when you want to use this? Give me two or three natural phrases."*

Capture literally. These become trigger phrases. Civilian phrasing is the point.

### 5. What the conversation looks like

Ask, one at a time:

- What does Claude need to know before it starts (which state file to read, any context)?
- What are the questions Claude should ask you, in order?
- What should Claude avoid doing (common failure modes, things that would annoy you)?
- What should Claude write down at the end, and where?

Go at the user's pace. If they get stuck on the questions list, ask them to imagine a real recent time they wished they had this skill, and walk through what Claude should have asked them.

### 6. Name it

Propose two or three short, civilian names. Let the user pick. Lowercase, hyphens, no cleverness. If it is a domain skill, the file name is just the verb (e.g. `budget-this.md`), not prefixed with the domain.

### 7. Draft and review

Write the draft of the skill file in the right location, following the same shape as the existing skills:

- Frontmatter: name, description, type (skill), domain if applicable, trigger_phrases.
- Short framing paragraph.
- "Before you start" section.
- "How to run" section with numbered questions.
- "After the conversation" section with what to write and where.
- "Voice reminder" section with the thing the user said to avoid.

Show the user the draft, or the path and a short summary. Ask: *"Does this look right, or should we change anything?"*

Iterate until they are happy. Maximum three passes. If you cannot land it in three, step back and ask what is off.

### 8. Save and register

Save the file. Tell the user where it is. Ask whether they want a line in a running "skills I have added" list. If yes, append to `pack/memory/INDEX.md` under a "Custom skills" section, one line with the skill name, path, and one-sentence purpose.

## Quality gate before declaring done

Before marking the new skill complete, check:

- The trigger phrases sound like something the user would actually say.
- The questions in "How to run" are in the user's voice, not generic.
- The write-back instruction is specific (file, section, format).
- The skill does not duplicate an existing one.
- The skill honours `pack/conventions/voice.md`, including the hard rules on em dashes and "not X, but Y".

If any fail, fix before closing the conversation.

## Voice reminder

This is the meta-skill. How you do this conversation is how the user learns to think about skills in general. Be patient. Be concrete. If the user is vague, help them be specific before writing anything.
