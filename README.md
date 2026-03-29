# Egypt Opportunity Agent

A flexible markdown-based mentor agent for Egyptian users.

Status: early open-source prompt pack for a mentor-style decision and execution agent.

This repository is an open-source prompt pack built around:

- one bootstrap file to mention at the start of a conversation
- one main system prompt
- modular skills
- governance guardrails
- market context files
- architecture references for builders
- contribution guidance for open-source collaborators

## What This Repo Solves

This project is meant to help an agent answer questions like:

- What should this person focus on now?
- What is the real bottleneck?
- What should they do next in their actual life constraints?
- How should the agent follow up after weak execution or changing evidence?

It is designed for users in Egypt first, and for builders who want a reusable mentoring system rather than a generic advice bot.

## Primary entrypoint

- `START-HERE.md`

This is the bootstrap file.
It points the agent to the rest of the repository and the intended load order.

## Quick start

If you are using the repo:

1. If your host supports file mentions, start from `START-HERE.md`
2. If file mentions are unavailable, load `START-HERE.md` manually into the host context
3. Follow `manifests/load-order.md`
4. Use `examples/` to understand intended behavior
5. Use `evaluations/` to judge response quality

If you are contributing to the repo:

1. Read `CONTRIBUTING.md`
2. Change the smallest relevant file set
3. Add or update an example or evaluation when the change is meaningful

## What Is Included

This repo includes:

- a bootstrap entrypoint
- a system prompt
- a response contract
- modular skills
- governance rules
- realistic examples
- evaluation rubrics and dry runs

## What Is Not Included

This repo does not currently include:

- a bundled runtime
- a UI
- a database or memory backend
- a hosted service
- a provider-specific integration layer

It is intentionally host-agnostic so builders can adapt it to ChatGPT-style file mentions, custom GPTs, editor agents, local tools, or other environments.

## Repository structure

- `START-HERE.md`: bootstrap entrypoint
- `manifests/load-order.md`: intended file loading order
- `manifests/host-contract.md`: generic host capability contract
- `prompts/system.md`: main behavioral foundation
- `prompts/response-contract.md`: response quality contract
- `skills/`: modular mentoring capabilities
- `governance/`: long-term quality, safety, and memory controls
- `market/`: Egypt-specific market context
- `architecture/`: structure references for builders and integrators
- `examples/`: realistic case walkthroughs for builders and reviewers
- `evaluations/`: quality checks and scoring references
- `CONTRIBUTING.md`: contributor guidance and change rules

## Skill philosophy

Skills are organized in two layers:

- problem-type skills under `skills/core/`
- domain skills under `skills/domains/`

This lets the agent combine a problem lens such as validation, monetization, prioritization, growth, or execution with a market/domain lens such as real estate, fintech, ecommerce, education, career and work, creator and media, local services, healthcare, or tech.

Across both layers, the agent should stay actor-aware.
A sector does not imply one default user type, buyer, or decision-maker.

## Design philosophy

This repo is host-agnostic.
It is meant to preserve the same mentoring logic across different environments and products.

## Fast Evaluation Path

If you want to judge the repo quickly:

1. Read `examples/founder-no-revenue.md`
2. Read `evaluations/dry-runs/founder-no-revenue-dry-run.md`
3. Check `evaluations/checklist.md`
4. Check `evaluations/scoring-rubric.md`

This gives a fast picture of how the system is supposed to think, respond, and review.

## Product identity

The agent is:

- a mentor-style decision and execution guide
- memory-aware when the host supports memory
- Egypt-focused by default
- strict in practical decisions
- more containing in human and psychological layers

The agent is not:

- a generic motivation bot
- a fixed template advisor
- tied to one interface or provider
- a substitute for licensed medical, legal, or financial professionals

## Builder note

If you are integrating this repo into a product, start from:

- `START-HERE.md`
- `manifests/load-order.md`
- `architecture/agent-spec.md`

If you are extending the repo itself, start from:

- `CONTRIBUTING.md`
- `examples/README.md`
- `evaluations/README.md`

## License

This repository is licensed under the MIT License.
See `LICENSE`.

