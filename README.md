# Koine for Life

A personal operating system you run by talking. Files stay on your computer. Claude Desktop is the default interface.

**New here? Start with [GETTING-STARTED.md](GETTING-STARTED.md).**

## Things you can ask for

Once you have run the opening interview (say *"run me first"* to Claude), these are the conversations available to you. You do not need to memorise them. They read naturally, and Claude will recognise the intent.

### Getting oriented

- *"run me first"*: the opening interview. Do this once.
- *"what can this pack do?"*: Claude reminds you what is available.
- *"remind me who I am"*: reads your identity file back to you.

### Finances

- *"let's look at the finances"*: monthly review.
- *"I'm thinking about buying X"*: decision log for larger purchases.
- *"annual check-in"*: year-level view.

### Family

- *"plan the week"*: weekly family plan.
- *"let's think about [child's name]"*: focused conversation about one of your children.
- *"term review"*: end-of-term reflection on how things went.

### Ventures

- *"new opportunity came up"*: capture and think through something new.
- *"Monday review"*: weekly operations review.
- *"let's check the thesis"*: revisit why you are doing what you are doing.

### Health

- *"habit check-in"*: how the habits you set are going.
- *"medical decision"*: think through a medical choice with a log.
- *"training review"*: review a training plan.

### Learning

- *"reading log"*: capture what you are reading and what is sticking.
- *"course progress"*: review a course or learning track.

### Hobbies and interests

- *"log a [thing]"*: record a session, outing, or event for any hobby.
- *"how's [hobby] going"*: reflect on progress or enjoyment.
- New hobby? Say *"I want to track [thing]"* and Claude will set it up.

### Career

- *"let's take stock of my career"*: the deeper career conversation, arc and current chapter.
- *"prep for this interview"*: walk through an interview before it happens.
- *"sharpen my bio"*: work on how you describe yourself.
- *"recruiter reached out"*: think through an approach before engaging.

### Adding something new

- *"I want help with [area of life not covered here]"*: Claude builds a new skill with you through an interview.

## Structure (for the curious)

```
koine-for-life/
  GETTING-STARTED.md    (read this first)
  SETUP.md              (detailed install for Desktop, web, Code)
  PRIVACY.md            (what to store, what not to)
  pack/
    identity/           (written during run-me-first)
    memory/             (your growing notes)
    domains/            (seven life domains, each with its own state and skills)
    skills/             (pack-level skills: run-me-first, new-life-skill)
    reviewers/          (quality checks Claude runs against its own output)
    conventions/        (house style for Claude)
```

## Etymology

*Koine* (κοινή) is the shared Greek of everyday life in the Hellenistic world, the common tongue rather than the literary one. This pack is named for that spirit: a shared way of working, in plain language.
