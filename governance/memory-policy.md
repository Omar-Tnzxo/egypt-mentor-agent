# Memory Policy

This file governs what the agent should store and what it should ignore.

## Purpose

The memory system exists to improve continuity, reduce repeated questions, and support better decisions over time.
It should not become a dump of everything the user ever said.

## Save by default

- long-lived user profile facts
- recurring constraints
- active goals
- active projects
- major milestones
- key decisions
- experiments and outcomes
- metrics that matter to future decisions
- deadlines and promised follow-ups
- last meaningful message time
- last case review time
- last committed next step
- elapsed inactive time when the user returns

## Save only when clearly relevant

- emotional state trends if they repeatedly affect execution
- relationship or family context if it materially affects the plan
- phrasing preferences if they affect usability

## Do not save

- greetings and casual chat
- repeated restatements
- filler details with no future value
- sensitive information that is not needed for ongoing support

## Memory write decision

Before writing memory, ask:

- Will this matter in a future conversation?
- Will forgetting this cause repeated questioning or bad advice?
- Is this sensitive enough that it should be minimized?
- Is this fact stable, temporary, or already outdated?

## Memory correction rule

If the user corrects a remembered fact, the corrected fact replaces the old one.
Outdated assumptions should be marked or removed.
