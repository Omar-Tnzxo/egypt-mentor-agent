# Skill: Healthcare Domain

Use this skill when the user's case touches:

- clinics
- hospitals
- diagnostics
- pharmacies
- telemedicine
- healthcare operations
- patient experience
- medical practice operations
- healthcare startups
- healthtech products
- healthcare services in Egypt

## Goal

Filter the recommendation through Egyptian healthcare reality instead of generic startup or operations advice.

## Core rule

In healthcare, growth alone is not enough.
The agent must distinguish between:

- patient safety
- clinical responsibility
- operational value
- trust
- access
- regulatory or accreditation constraints
- payer or provider incentives
- monetizable value

Do not assume one default actor inside healthcare.
Always identify who the current speaker is, who the patient is, who provides care, who pays, who decides, and where the real constraint sits.

## Safety-first rule

Healthcare is a sensitive domain.
If the case moves into diagnosis, treatment choice, medication advice, urgent symptoms, or patient-specific clinical judgment, the agent must not behave like a clinician.
It should clearly separate:

- operational or business guidance
- product or workflow guidance
- patient-safety or medical-risk issues that need a qualified professional

When risk is meaningful, the agent should say so clearly and avoid pretending that business logic can replace medical judgment.

## Actor examples in this domain

The speaker may be:

- a clinic owner
- a doctor
- a practice manager
- a hospital operator
- a lab or imaging operator
- a pharmacist
- a founder building a healthtech product
- an operations lead
- a patient
- a caregiver
- an insurer-side or payer-side stakeholder

## Egypt-specific domain realities

- trust and safety are central, not optional
- healthcare delivery often involves both public and private actors
- private providers can play an important role in access and service delivery
- accreditation, governance, and care quality can materially affect what is viable
- convenience may matter, but it cannot substitute for safety or credibility
- many healthcare ventures fail when they optimize growth before clarifying clinical responsibility, workflow fit, or quality control
- in many cases, operational discipline and patient trust matter as much as the technology itself

## Reality checks

Always inspect:

- who the main actor is
- whether the case is clinical, operational, commercial, educational, or product-related
- whether patient safety is directly affected
- who is legally or professionally responsible for care decisions
- whether the product or service improves a real healthcare workflow
- whether the workflow is frequent and painful enough to matter
- whether trust, privacy, quality, accreditation, or provider behavior are the real bottlenecks
- whether the case is B2C, provider-led, clinic-led, hospital-led, payer-led, or hybrid

## Important distinctions

Separate clearly between:

- patient demand
- patient safety
- clinical quality
- operational efficiency
- provider adoption
- monetization readiness
- scalable healthcare value

Do not confuse downloads, signups, inquiries, or patient interest with safe and sustainable healthcare value.

## Common useful questions

The agent should often determine:

- who the speaker is in the healthcare system
- what exact outcome matters now: better access, smoother operations, more patient trust, better retention, better utilization, stronger economics, or safer delivery
- whether the main bottleneck is trust, workflow friction, staff behavior, compliance, safety, adoption, or unit economics
- whether the user is solving for patients, providers, clinics, hospitals, payers, or multiple actors at once
- whether the product depends on clinician behavior change, patient behavior change, or institutional adoption
- whether the current model is operationally useful enough to deserve expansion

## Good near-term paths in this domain

Depending on the case, the agent may lean toward:

- proving one safe and workflow-aligned use case before broader expansion
- improving provider or clinic-side operations before chasing patient growth
- clarifying responsibility, quality controls, and trust before scaling distribution
- narrowing the scope to one high-friction healthcare workflow
- improving adoption among care providers before treating user interest as success
- distinguishing clearly between healthcare operations value and medical decision-making

## Output requirements

When this skill is active, include:

- primary actor in the current case
- relevant secondary actors
- whether the case is clinical, operational, commercial, or hybrid
- where the strongest current value exists
- where the main healthcare leak or risk exists
- what part of the model most threatens safety, trust, or adoption
- what should be tested next in the Egyptian healthcare context
