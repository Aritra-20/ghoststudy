# 👻 GhostStudy

**Live demo → [ghoststudy-aritrapal.vercel.app](https://ghoststudy-aritrapal.vercel.app/)**

A concept prototype from my Design Thinking course at Great Lakes Institute of Management.

## The problem

MBA students are told to upskill (certifications, courses, side projects), but the timetable leaves no obvious room for it. The time does exist. It's scattered across 40- and 90-minute gaps between classes, and those gaps get eaten by scrolling, snacks and "I'll start after lunch."

The problem isn't motivation. Nobody plans a 50-minute gap, so it never gets used.

## The idea

GhostStudy reads your calendar, finds the usable gaps, and **ghost-blocks** them with the next module of the certification you're working towards. When a block is about to start, it nudges you once with the exact module to open.

## What the prototype does

- **Loads a sample PGPM week** with classes and club commitments
- **Finds usable gaps** with a threshold you set (30/45/60 min). It keeps a 10-minute buffer after each class and protects lunch.
- **Books the longest gaps first**, capped per day, so the plan doesn't turn into a second timetable
- **Assigns modules in order** for PL-300, Google Advanced Data Analytics or Tableau Desktop Specialist
- **Tracks progress**: tap a block to mark it done and watch the minutes add up

## Design decisions

| Decision | Why |
|---|---|
| Daily cap on ghost blocks | A tool that fills every gap stops being a nudge and becomes pressure. Users ignore that fast. |
| Longest gaps first | A 90-minute gap is a real study session. A 45-minute one is a revision slot. |
| Buffer after class | Back-to-back scheduling looks efficient on paper and fails in real life. |
| One nudge, not reminders | The goal is to lower the activation cost of starting, not to nag. |

## What's next

- Connect to Google Calendar / Outlook with read-only access
- Learn which gaps a student actually uses and stop booking the ones they always skip
- Point nudges at the exact lesson URL in the course platform

---

*Concept prototype: a sample schedule and rule-based scheduling in plain HTML/JS, with no real calendar connection. Built to test the interaction, not as production code.*
