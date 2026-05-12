---
name: learning-research
description: Use when the user wants a practical research operating system for CV or ML paper work, especially around reading papers, finding problems, generating and filtering ideas, debugging experiments that do not work, writing papers and talks, handling rebuttals, or turning one paper into a coherent multi-paper roadmap.
---

# Learning Research

Use this skill to turn vague research ambition into an explicit operating loop:

`problem -> hypothesis -> experiment -> evidence -> paper -> next problem`

This skill is for execution and diagnosis, not motivation. It is optimized for `CV`, `3D vision`, `graphics`, and adjacent `ML` paper workflows, but the logic can generalize to nearby experimental fields. Use it when the user needs to:

- read papers with a "what next?" lens rather than only summarizing
- find research problems from prior work instead of jumping randomly
- turn an intuition into a testable idea
- diagnose why experiments do not work
- structure weekly research progress and discussion
- write a paper, rebuttal plan, or talk from evidence
- connect one project to the next as a coherent roadmap

## Default Outcome

Unless the user asks for a narrower slice, produce these artifacts:

1. `problem-statement`
2. `idea-card`
3. `experiment-plan`
4. `experiment-log`
5. `writing-claim-map`
6. `roadmap-step`
7. `paper-reading-note` when the user starts from literature
8. `rebuttal-response-plan` when the user is in review mode

## Core Workflow

1. **Start from the current paper or project.** Do not brainstorm in the abstract if the user already has work in progress.
2. **Separate observations from explanations.** First list what works, what fails, and where evidence is weak. Only then infer causes.
3. **Force testability.** A research idea is not valid until it includes a concrete validation path.
4. **Distinguish engineering problems from research problems.** Read `references/experiment.md` before recommending a pivot.
5. **Read papers for boundaries, not only summaries.** Read `references/paper-reading.md` when the user wants to extract gaps, claims, baselines, or next-step questions from literature.
6. **Write claims early.** Read `references/writing.md` once the user has partial results, not only at submission time.
7. **Plan rebuttals from reviewer claims and evidence gaps.** Read `references/rebuttal.md` when the user has reviewer feedback or wants a rebuttal workflow.
8. **Grow the next paper from the boundary of the previous one.** Read `references/roadmap.md` when the user wants a multi-paper direction.

## Operating Rules

- Prefer one-step-next questions over grand research agendas.
- Treat failure cases as assets only after they are categorized.
- Do not propose a new direction before checking whether the current result is blocked by data, code, training setup, or evaluation mistakes.
- In CV/ML settings, keep the benchmark, metric, and visual failure slices explicit. Do not discuss ideas without anchoring them to a dataset, task, or evaluation protocol when one already exists.
- Prefer reusable artifacts over free-form advice: tables, checklists, claim maps, and logs.
- If the user lacks context, narrow the scope to one dataset, one benchmark, one bottleneck, or one claim.

## Reference Guide

- Read `references/fixed-sop.md` when the user wants the standard end-to-end workflow or asks what to do next in a paper cycle.
- Read `references/idea.md` for problem finding, idea generation, and idea filtering.
- Read `references/experiment.md` for experiment design, debugging order, and failure diagnosis.
- Read `references/paper-reading.md` for structured paper reading and gap extraction.
- Read `references/writing.md` for claim-evidence structure, paper drafting, and talk framing.
- Read `references/rebuttal.md` for reviewer triage, response drafting, and evidence planning.
- Read `references/roadmap.md` for turning one project into a coherent research line.
- When the task becomes section-level paper rewriting or pre-submission self-review, hand off to the installed `$research-paper-writing` skill for Abstract / Introduction / Related Work / Method / Experiments / Conclusion-specific guidance.

## Templates

When the user wants concrete artifacts, use these templates in `assets/templates/`:

- `cvml-paper-sop-checklist.md`
- `idea-card.md`
- `experiment-log.md`
- `paper-reading-notes.md`
- `rebuttal-response-plan.md`
- `weekly-research-review.md`
- `roadmap.md`

## Output Preference

When using this skill:

- optimize for decisions, not inspiration
- make uncertainty explicit
- state assumptions when evidence is missing
- propose the smallest experiment that can falsify the idea
- keep recommendations tied to the user's actual project, not generic research folklore
