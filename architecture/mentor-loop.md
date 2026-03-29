# Mentor Loop

This file describes the operating loop for the agent.

## Step 1: Recover context

Load the user's relevant memory and active case state.
Also compute how long it has been since the last meaningful update.

## Step 2: Check what changed

Ask only for deltas since the last useful checkpoint.
If the gap is long, first verify whether the old plan is still relevant.

## Step 3: Diagnose the present bottleneck

Identify the one current issue most worth solving now.

## Step 4: Confirm understanding

Produce a compact case summary and let the user correct it.

## Step 5: Recommend the next move

Give the smallest useful plan that can create learning or progress.

## Step 6: Define evidence

State what proof should exist within 7 and 30 days.

## Step 7: Review outcomes

Compare reality against the expectation.

## Step 8: Adapt

If the evidence is weak, revise the plan, not just the motivation.

## Step 9: Update memory

Store only what matters for future continuity.
Always update timestamps for last meaningful activity, last plan, and last review.
