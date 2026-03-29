# Egypt Mentor Agent

Open-source prompts, skills, and evaluation assets for building a mentor-style AI agent focused on Egyptian users.

This project is designed for builders who want something more disciplined than a generic advice bot:

- better diagnosis before planning
- one real priority instead of many
- plans sized for real life constraints
- honest follow-up after weak execution
- Egypt-first market and life-context awareness

## What This Is

`egypt-mentor-agent` is a host-agnostic prompt pack for a long-term mentor-style agent.

It is meant to help an AI system answer questions like:

- What should this user focus on now?
- What is the actual bottleneck?
- What should happen next given time, money, and life constraints?
- What should the agent do when the user comes back with weak execution or changed reality?

The repo is structured so the same mentoring logic can be reused across:

- file-aware chat tools
- editor agents
- custom GPT-style environments
- local AI wrappers
- future runtime integrations

## What Makes It Different

This project is opinionated.

The agent is expected to:

- ask one meaningful question at a time
- avoid low-value or repetitive questions
- build a case map before giving a serious plan
- choose one main priority by default
- protect the user from drift
- separate practical problems from human-side problems
- use evidence and reality to settle disagreements
- maintain continuity when the host supports memory

It is explicitly not meant to be:

- a motivation bot
- a generic life-coach template
- a "10 ideas" machine
- a substitute for licensed medical, legal, or financial professionals

## Repository Contents

- `START-HERE.md`
  Bootstrap entrypoint for hosts that support file loading or mentions.
- `prompts/system.md`
  Core system behavior and mentoring rules.
- `prompts/response-contract.md`
  Internal quality contract for strong responses.
- `skills/core/`
  Reusable cross-domain decision and execution skills.
- `skills/domains/`
  Egypt-aware domain lenses such as real estate, fintech, ecommerce, and more.
- `governance/`
  Safety, memory, review, and long-term quality controls.
- `manifests/`
  Load order and host capability references.
- `examples/`
  Realistic worked cases that show intended behavior.
- `evaluations/`
  Checklists, scoring rubrics, and dry runs for quality control.
- `architecture/`
  Builder-facing structural references.
- `CONTRIBUTING.md`
  Rules for extending the repo without breaking its philosophy.

## Quick Start

If your host supports file mentions or file loading:

1. Start from `START-HERE.md`
2. Follow `manifests/load-order.md`
3. Load only the domain files that match the current case

If your host does not support file mentions:

1. Manually load `START-HERE.md` into the host context
2. Then follow `manifests/load-order.md`
3. Keep the same structure and behavior rules

If you want to understand the intended output quality fast:

1. Read `examples/founder-no-revenue.md`
2. Read `evaluations/dry-runs/founder-no-revenue-dry-run.md`
3. Review `evaluations/checklist.md`
4. Review `evaluations/scoring-rubric.md`

## Core Design Principles

- Egypt-first by default
- diagnosis before planning
- one main priority by default
- current-phase plans over giant roadmaps
- execution evidence over intention
- follow-up that reacts to reality, not wishful thinking
- actor-aware domain reasoning
- host-agnostic packaging

## Current Coverage

The prompt pack currently includes:

- core skills for diagnosis, validation, monetization, prioritization, growth, execution, and review
- domain lenses for real estate, fintech, ecommerce, education, career and work, creator and media, local services, healthcare, and tech
- realistic examples for founders, creators, career switches, service businesses, and weak-execution review loops
- evaluation assets for checking whether the system is actually behaving like a mentor

## What Is Not Included

This repository does not currently ship with:

- a bundled runtime
- a UI
- a database or persistence layer
- a memory backend
- a hosted API
- a provider-specific integration

That is intentional.
The goal is to keep the mentoring brain reusable across different environments.

## For Builders

If you want to integrate the repo into a product, start here:

- `START-HERE.md`
- `manifests/load-order.md`
- `prompts/system.md`
- `prompts/response-contract.md`
- `architecture/agent-spec.md`

If you want to extend the repo itself, start here:

- `CONTRIBUTING.md`
- `examples/README.md`
- `evaluations/README.md`

## Quality Standard

A strong implementation of this repo should consistently produce responses that:

- reduce confusion
- identify the real bottleneck
- fit the user's actual constraints
- avoid spreading effort across many tracks
- create a reviewable next step
- become smarter over time through continuity and evidence

## Status

This is an early but serious open-source foundation.

The repo already contains:

- a usable bootstrap structure
- modular prompt architecture
- examples
- evaluations
- contributor guidance

The next layer of maturity depends on how builders integrate it into real hosts and test it against live cases.

## Contributing

Contributions are welcome, but this repo should stay disciplined.

Before changing behavior, read:

- `CONTRIBUTING.md`

For meaningful changes, prefer updating:

- at least one example
- at least one evaluation artifact

That keeps the project grounded in real behavior instead of theory alone.

## License

MIT License.
See `LICENSE`.

