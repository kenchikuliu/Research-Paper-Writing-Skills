# Experiment

Use this file when the user needs experiment design, debugging guidance, or help deciding whether "not work" indicates a bug, a weak setup, or a weak idea.

## Principle

Experiments exist to test hypotheses, not to generate random movement.

Before each experiment, write:

- what changed
- why it should matter
- which metric should move
- what result would weaken the hypothesis

## Minimum Experiment Record

Track at least:

- date
- code version
- data version
- config
- changed variables
- expected effect
- observed result
- interpretation
- next action

## Debugging Order

When results do not work, use this order:

1. Confirm the baseline can be reproduced.
2. Confirm the data pipeline and evaluation are correct.
3. Reduce to the smallest intervention.
4. Check training stability, hyperparameters, and ablations.
5. Inspect qualitative cases and failure clusters.
6. Only then judge whether the idea lacks signal.

Do not jump to "the idea is bad" before ruling out implementation and measurement issues.

## Engineering vs Research

Classify problems explicitly.

Engineering problems:

- code bug
- bad preprocessing
- wrong labels or splits
- unstable training setup
- evaluation mismatch
- resource bottleneck

Research problems:

- assumption fails under realistic conditions
- proposed signal is too weak
- problem formulation is misaligned with the benchmark
- objective and desired behavior diverge
- method improves one dimension while hurting the real target

If a result is blocked by engineering issues, do not use it to define the next paper.

## Diagnostic Questions

Ask these when results are weak:

- Did the method fail everywhere or only in a slice of the data?
- Did the gain disappear after correcting evaluation?
- Is the failure due to optimization difficulty or conceptual mismatch?
- Does the method help only because of added capacity or compute?
- What is the simplest baseline that already captures most of the gain?

## Escalation Rule

Escalate from debugging to research reframing only after:

- baseline is trusted
- evaluation is trusted
- minimal intervention was tested
- failure patterns are described, not guessed
