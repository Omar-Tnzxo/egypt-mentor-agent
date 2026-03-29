# Egypt Opportunity Agent

Agent prompt system focused on helping people in Egypt answer:

- What should I do?
- How do I do it?
- How do I do it in my real situation?

The structure is intentionally simple:

- `prompts/system.md`: the main system prompt
- `skills/`: modular markdown skills loaded alongside the system prompt
- `market/egypt-2026-top-100.md`: a practical map of 100 high-signal domains for Egypt in 2026
- `governance/`: long-term quality, safety, review, memory, and update controls
- `architecture/`: implementation-oriented docs for open-source builders

## Suggested runtime pattern

1. Load `prompts/system.md`
2. Load core skills:
   - `skills/core/intake-and-diagnosis.md`
   - `skills/core/guided-questioning.md`
   - `skills/core/memory-and-continuity.md`
   - `skills/core/plan-construction.md`
   - `skills/core/egypt-lens.md`
   - `skills/core/uncertainty-and-options.md`
   - `skills/core/follow-up-and-accountability.md`
3. Load governance files:
   - `governance/risk-register.md`
   - `governance/safety-boundaries.md`
   - `governance/memory-policy.md`
   - `governance/market-update-policy.md`
   - `governance/outcome-review-loop.md`
4. Load domain skills based on the user's topic
5. Load `market/egypt-2026-top-100.md` when the user needs sector selection or market positioning
6. Use `architecture/user-case-memory-schema.md` and `architecture/mentor-loop.md` when implementing the open-source runtime

## Current scope

This starter pack is optimized for:

- Business
- Tech
- Career direction
- Execution planning
- Long-term mentorship-style follow-up

It can be expanded later into health, education, family business, creative work, trades, and regional opportunities inside Egypt.

## Long-term quality stance

This project treats the agent as:

- a decision-support system
- a mentor-style thinking partner
- not an authority
- not a therapist
- not a doctor
- not a lawyer
- not a financial advisor

The agent should help users think clearly and act concretely, while exposing assumptions, uncertainty, fit limits, and progress evidence.
