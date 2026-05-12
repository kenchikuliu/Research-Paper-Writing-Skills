# Paper Reading

Use this file when the user wants to read CV/ML papers in a way that produces next-step research value instead of passive summary.

## Goal

Read papers to extract:

- the exact problem formulation
- the claimed contribution
- the evidence that supports the claim
- the hidden assumptions and boundaries
- the most natural next question

## Reading Pass

For each paper, force these fields:

- Task:
- Setting:
- Dataset or benchmark:
- Main claim:
- Method intuition:
- Strongest evidence:
- Most relevant baseline:
- Where the method seems fragile:
- What is not explained:
- Most natural next-step question:

If the user cannot fill `strongest evidence` or `most relevant baseline`, the paper has not been read closely enough.

## CV/ML-Specific Checks

For vision and ML papers, explicitly inspect:

- what data regime the method assumes
- which baselines are omitted or weak
- whether gains are global or only on selected slices
- whether compute, capacity, or augmentation explains the gain
- whether qualitative examples align with the numeric claim
- whether the method is robust to distribution shift, viewpoint shift, noise, or temporal inconsistency when those matter

## Boundary Extraction

The most useful next-paper signals often come from:

- datasets where the method underperforms
- ablations that show a weak or unstable module
- visual failure modes hidden behind average metrics
- missing stress tests
- claims that rely on intuition but are under-validated

## Reading Modes

Use one of three modes:

1. `landscape mode`
   Use for reading many papers to map a direction.
   Output: problem clusters, method families, benchmark norms.

2. `replication mode`
   Use when the user wants to reproduce or extend one paper.
   Output: assumptions, implementation risks, key ablations, likely failure points.

3. `roadmap mode`
   Use when the user already has a paper and wants the next one.
   Output: which paper boundary matters most and what evidence is still missing.

## Anti-Patterns

- summarizing architecture details without identifying the central claim
- confusing leaderboard wins with solved problems
- reading papers without comparing to the user's current stack
- proposing next steps without locating a concrete failure boundary
