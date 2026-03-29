# Risk Register

This file maps long-term failure modes of the agent to controls.

## 1. Superficial diagnosis

Risk:
The agent gives polished advice based on shallow understanding.

Controls:

- require intake before recommendation
- label missing information
- use `skills/core/intake-and-diagnosis.md`
- route to `skills/core/uncertainty-and-options.md` when confidence is low

## 2. Template repetition across different users

Risk:
The agent starts giving the same plan to everyone.

Controls:

- force a "why this fits this person" section
- force a "what to avoid for now" section
- include user constraints in every plan
- review logs for repeated outputs across distinct profiles

## 3. Outdated Egypt market assumptions

Risk:
The agent keeps recommending paths based on stale market conditions.

Controls:

- maintain a dated market update policy
- timestamp sector assumptions
- review the top-100 domain map on a schedule
- mark weakly supported sectors as inferred, not known

## 4. False confidence

Risk:
The agent sounds certain when it should be cautious.

Controls:

- require Known / Inferred / Needs validation labels
- allow multiple bounded options when uncertainty is high
- prevent single-answer outputs in low-confidence cases

## 5. User dependency

Risk:
The user stops developing judgment and asks the agent to decide everything.

Controls:

- explain the decision logic
- ask the user to choose based on explicit selection rules
- treat reversible decisions as learning opportunities
- avoid command-style language when not justified

## 6. Planning without execution

Risk:
The user feels progress from planning alone.

Controls:

- require observable proof within 7 and 30 days
- use outcome checkpoints
- define pivot and stop triggers
- store outcome patterns for future tuning

## 7. Personal issues misread as execution issues

Risk:
The agent frames exhaustion, instability, or distress as a pure productivity problem.

Controls:

- detect signs of burnout, crisis, or severe instability
- reduce plan intensity when energy is low
- recommend human support in high-risk situations
- avoid harsh optimization framing

## 8. Harm in high-stakes domains

Risk:
The agent causes harm in medical, legal, financial, or mental health decisions.

Controls:

- strict safety boundaries
- general education only in high-stakes topics
- encourage qualified local professional help
- never present high-stakes guidance as personalized certainty

## 9. Privacy and trust erosion

Risk:
Collecting more user details increases misuse and trust loss.

Controls:

- ask only for minimum useful information
- avoid unnecessary personal details
- separate diagnosis signals from identity data
- discourage sensitive disclosure unless essential

## 10. Prompt sprawl and governance drift

Risk:
The markdown system becomes inconsistent, duplicated, and hard to maintain.

Controls:

- keep each skill narrow in scope
- create one source of truth for safety and updates
- version governance files
- review conflicting prompt instructions regularly
