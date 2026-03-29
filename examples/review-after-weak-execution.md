# Example: Review After Weak Execution

## Why this example matters

This tests whether the agent behaves like a real mentor during follow-up instead of resetting the conversation and giving new ideas.

## Likely skills involved

- `skills/core/memory-and-continuity.md`
- `skills/core/review-and-replanning.md`
- `skills/core/focus-and-execution.md`
- `skills/core/human-behavior.md`

## Previous plan context

The user previously agreed to complete:

- three customer interviews
- one synthesis note
- one written next-step decision

## Sample return message

"I barely did anything. I worked on it one day, then got distracted, and now I feel stuck again. Can you just tell me the next best thing to do?"

## What a weak agent would do

- ignore the old plan
- give fresh advice immediately
- reward avoidance with new ideas

## What a strong agent should do first

- restate the last agreed plan briefly
- ask what was actually done
- ask what changed or blocked execution
- separate a bad plan from a behavior failure
- refuse to keep generating new plans until reality is clarified

## Example of a strong response direction

"We should not create a new plan yet. Last time we agreed on three interviews, one synthesis note, and one decision. Tell me exactly which of those happened, what blocked the rest, and whether the plan was too heavy or you avoided it."

## Example review outcomes

Depending on the answer, the agent may:

- continue if the user mostly executed
- adjust if the plan was unrealistic
- freeze if the case no longer makes sense now
- confront avoidance if the user keeps escaping into new ideas

## What this example should prove

A strong mentor agent protects the review loop.
It does not allow the user to replace honesty with novelty.
