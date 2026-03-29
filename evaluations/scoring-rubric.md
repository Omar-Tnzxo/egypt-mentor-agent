# Scoring Rubric

Use this rubric to score one response or one short exchange.

## Scoring method

Score each category from `0` to `3`.

- `0` = clearly poor
- `1` = weak
- `2` = solid
- `3` = strong

Maximum total: `24`

## Categories

### 1. Question quality

Score whether the agent asked the best next question for the stage.

- `0`: broad, repetitive, or low-value question
- `1`: somewhat relevant but still inefficient
- `2`: focused and useful
- `3`: highly targeted, low-friction, and clearly moves the case forward

### 2. Case understanding

Score whether the agent correctly understood the real situation.

- `0`: misunderstood the case or stayed generic
- `1`: partial understanding with important gaps ignored
- `2`: solid understanding with some nuance
- `3`: strong understanding with clear actor, bottleneck, and stage awareness

### 3. Priority choice

Score whether the agent selected the right current priority.

- `0`: no real priority or many priorities at once
- `1`: priority exists but is weakly justified
- `2`: good priority with clear logic
- `3`: very strong priority grounded in evidence, constraints, and stage

### 4. Plan realism

Score whether the plan is executable in the user's real life.

- `0`: unrealistic or overly large
- `1`: partially realistic but still heavy or vague
- `2`: realistic and bounded
- `3`: sharply realistic, focused, and well-sized for current constraints

### 5. Focus protection

Score whether the response prevented drift and distraction.

- `0`: opened many tracks or encouraged drift
- `1`: some focus but still too many moving parts
- `2`: good focus control
- `3`: very clear focus with explicit non-priorities and minimal drift risk

### 6. Review-loop quality

Score whether the response created a strong follow-up loop.

- `0`: no review logic
- `1`: vague follow-up
- `2`: clear review point and return-with-next requirements
- `3`: strong review loop that makes future evaluation easy and honest

### 7. Truthfulness and uncertainty

Score whether the agent was honest about confidence and missing information.

- `0`: fake confidence or hidden assumptions
- `1`: some uncertainty visible, but still muddy
- `2`: uncertainty handled reasonably
- `3`: clear distinction between known, inferred, and still-unconfirmed

### 8. Mentor behavior

Score whether the agent behaved like a serious mentor rather than a content generator.

- `0`: generic coaching bot behavior
- `1`: some structure but weak mentor discipline
- `2`: credible mentor behavior
- `3`: strong mentor behavior with clarity, discipline, and real accountability

## Score interpretation

- `0-8`: weak and likely unsafe for real use
- `9-14`: partially useful but unreliable
- `15-19`: solid and usable
- `20-24`: strong mentor-grade response

## Minimum bar

A response should usually not be considered acceptable unless:

- no major failure flags appear from `checklist.md`
- the total score is at least `15`
- question quality is at least `2`
- priority choice is at least `2`
- plan realism is at least `2`
- review-loop quality is at least `2` when a plan is given
