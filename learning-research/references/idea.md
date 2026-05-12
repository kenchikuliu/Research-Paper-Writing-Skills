# Idea

Use this file when the user needs help with problem finding, idea generation, or deciding whether an idea is worth pursuing.

## The Standard

A usable research idea must satisfy all three conditions:

1. The problem matters.
2. The hypothesis is explicit.
3. The hypothesis can be tested with feasible experiments.

If any of these are missing, the output is still a hunch, not an idea.

## Problem Sources

Prefer extracting problems from one of these sources:

1. A failure mode in the current project.
2. A boundary condition in the previous paper.
3. A mismatch between benchmark performance and real-case behavior.
4. A cost, robustness, or scaling limitation in the current method.
5. A mechanism gap: the method works, but the reason it works is unclear.

## Problem Review Pass

For any candidate problem, answer:

- What exactly is the object of study?
- Under what condition does the current method fail?
- Why is that condition important?
- How often does that condition appear?
- What evidence already exists that this is not just noise?

## Idea Card

Each candidate idea should fit this compact structure:

- Problem:
- Existing gap:
- Hypothesis:
- Minimal intervention:
- Validation path:
- Main risk:

If `validation path` is empty, reject or rewrite the idea.

## Filters

Score each candidate on `1-5` for:

- importance
- continuity with current work
- feasibility in the next 1-3 weeks
- clarity of evaluation
- upside if successful

Discard ideas that score high on ambition but low on continuity and testability.

## Common Failure Modes

- The "idea" is only a model tweak with no stated problem.
- The problem is broad but the evaluation only covers a narrow proxy.
- The user confuses novelty with complexity.
- The proposal changes too many factors at once.
- The user wants a new project before understanding why the current one failed.

## Next-Step Rule

When the user asks for the next paper direction, prefer the smallest meaningful step:

- previous work solves `Y` under condition `X`
- performance collapses under condition `Z`
- next work isolates why `Z` breaks the approach
- new method is justified only after that failure is evidenced
