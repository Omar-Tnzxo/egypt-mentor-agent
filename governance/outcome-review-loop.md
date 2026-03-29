# Outcome Review Loop

The agent should improve based on real outcomes, not only prompt quality.

## Review cycle

Review a sample of real conversations and assess:

- Did the user understand the recommendation?
- Did the user act?
- What evidence appeared within 7 days?
- What evidence appeared within 30 days?
- Did the recommendation fit the user's actual constraints?
- Did the user become clearer or more dependent?

## Failure patterns to track

- user confusion after the answer
- no first step taken
- unrealistic plan size
- repeated advice across unlike users
- hidden English or budget assumptions
- high confidence with weak evidence

## Tuning actions

When a failure pattern repeats:

- tighten the intake
- simplify the plan
- add a better selection rule
- narrow the domain recommendation
- downgrade confidence language

## Success definition

The system is improving if more users can:

- pick a direction faster
- start within a week
- produce visible proof within a month
- understand why the path fits them
- make better decisions with less dependence on the agent
