# Evaluations

This folder defines how to judge whether the mentor agent is actually working well.

These files are not user-facing prompts.
They are evaluation references for builders, reviewers, and future maintainers.

## Goal

Prevent the project from drifting into:

- generic advice
- impressive wording without real diagnosis
- over-planning
- fake certainty
- weak follow-up behavior

## What these evaluations should check

Use this folder to test whether the agent can:

- ask the right next question
- avoid low-value or repetitive questions
- build a valid case summary
- choose one real priority
- justify the priority with evidence
- protect focus by naming what is not a priority now
- give an executable current-phase plan
- define what the user should return with next
- review execution honestly instead of generating fresh advice too quickly

## Recommended use

Use the files in this folder together with the realistic cases in `examples/`.

Suggested review flow:

1. Pick one example case
2. Run the agent against the opening message
3. Score the response using `scoring-rubric.md`
4. Check failure modes using `checklist.md`
5. Repeat after prompt or skill changes

## Files

- `checklist.md`
- `scoring-rubric.md`
- `dry-runs/`

