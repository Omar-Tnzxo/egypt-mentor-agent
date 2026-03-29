# Contributing

Thank you for contributing to the Egypt Opportunity Agent.

This repository is not a generic prompt dump.
It is a structured mentor-agent prompt pack.
Good contributions should make the agent:

- clearer
- more realistic
- more disciplined
- more useful in follow-up
- less likely to drift into generic advice

## Before you change anything

Start from these files:

- `README.md`
- `START-HERE.md`
- `manifests/load-order.md`
- `prompts/system.md`
- `prompts/response-contract.md`

Then review the relevant folder for the kind of change you want to make:

- `skills/`
- `governance/`
- `examples/`
- `evaluations/`
- `architecture/`

## Core principles

Every contribution should preserve these principles:

- Egypt-first by default
- one meaningful question at a time during discovery
- no guessing of decision-relevant facts
- no generic motivation-bot behavior
- one main priority by default
- current-phase planning, not giant roadmaps
- honest follow-up and review loops
- actor-aware reasoning inside every domain
- strict in practical decisions, more containing in human matters

## What good contributions look like

Good contributions usually do one or more of the following:

- improve diagnosis quality
- reduce low-value questions
- sharpen prioritization logic
- make plans more executable
- improve review behavior after weak execution
- improve domain realism for Egypt
- add realistic examples that expose weaknesses
- add evaluation criteria that catch drift

## What weak contributions look like

Avoid contributions that:

- add hype language
- add many new ideas without improving decision quality
- make the agent more verbose but not more useful
- encourage multi-track planning by default
- turn the system into a generic therapist, doctor, lawyer, or financial advisor
- add domain files that are just generic business advice with sector words swapped in
- add examples that only show success and never stress the system

## Adding a core skill

Add a core skill under `skills/core/` only if it solves a repeated cross-domain problem such as:

- diagnosis
- prioritization
- validation
- monetization
- growth
- execution
- review
- human behavior

A strong core skill should:

- have one clear job
- reduce confusion
- improve decisions across multiple domains
- define output requirements when relevant
- avoid overlapping heavily with several existing files

Before adding a new core skill, ask:

- Is this really cross-domain?
- Is this missing today?
- Could this be a small improvement to an existing file instead?

## Adding a domain skill

Add a domain skill under `skills/domains/` only if the domain has real logic that changes decisions.

A strong domain skill should:

- be actor-aware
- reflect Egypt-specific reality
- distinguish attention from value
- distinguish usage from monetization
- identify common bottlenecks in that domain
- define what the agent should inspect before giving advice

Do not create a domain file that is just:

- generic startup advice
- generic career advice
- generic growth advice

with sector vocabulary pasted on top.

## Adding an example

Add examples under `examples/`.

Good examples should:

- start from a realistic opening message
- show what a weak agent would do
- show what a strong agent should do
- include a likely strong next question
- include a likely priority and current-phase plan
- expose a real failure risk in the system

Prefer examples with:

- ambiguity
- limited resources
- mixed signals
- follow-up friction
- possible self-deception

## Adding an evaluation

Add evaluations under `evaluations/`.

Good evaluations should:

- catch real failure modes
- be easy to reuse
- distinguish strong mentor behavior from generic content generation
- measure focus, realism, and follow-up quality

If you add a dry run, include:

- the source example
- a simulated strong exchange
- a checklist assessment
- a rubric score
- at least one lesson that should improve the system

## Editing system behavior

If you change:

- `prompts/system.md`
- `prompts/response-contract.md`
- `START-HERE.md`
- `manifests/load-order.md`

make sure the change does not silently break the rest of the repo.

After changing core behavior, review at least:

- one example
- one evaluation checklist pass
- one dry run if available

## Style rules

Keep the writing:

- simple
- direct
- structured
- practical
- non-hyped

Prefer:

- short sections
- concrete bullets
- explicit distinctions
- strong defaults with clear exceptions

Avoid:

- buzzwords
- vague inspiration language
- over-complicated frameworks
- decorative prose

## Contribution checklist

Before opening a PR or sharing a change, check:

- Does this improve clarity, realism, execution, or review quality?
- Does it reduce or increase drift toward generic advice?
- Does it preserve the mentor identity of the system?
- Does it fit Egypt-focused reality?
- Does it overlap too much with an existing file?
- Should there also be an example or evaluation added for this change?

## Minimum expectation for meaningful changes

For any non-trivial change, try to update at least one of these too:

- `examples/`
- `evaluations/`

This keeps the project grounded in real behavior instead of theory only.
