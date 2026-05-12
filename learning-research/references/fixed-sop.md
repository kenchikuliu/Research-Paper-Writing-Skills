# Fixed SOP

Use this file when the user wants one stable operating procedure for CV/ML paper work, or asks how to combine `$learning-research` and `$research-paper-writing` without improvising every cycle.

## Principle

Use `$learning-research` to decide what the work is and whether the evidence is meaningful.
Use `$research-paper-writing` to turn a decided story into reviewer-facing section writing and self-review.

Do not reverse that order.

## Stage 1: Scope the Project

Use: `$learning-research`

Goal:

- define one task, one benchmark or setting, one bottleneck

Required output:

- `problem-statement`

Exit condition:

- the project can be explained in one sentence: `we want to improve ____ under ____ because ____`

If missing:

- do not start paper drafting

## Stage 2: Read for Boundaries

Use: `$learning-research`

Load:

- `references/paper-reading.md`
- `assets/templates/paper-reading-notes.md`

Goal:

- map key papers
- identify what is already solved
- extract one boundary or failure region worth attacking

Required output:

- `paper-reading-note`

Exit condition:

- at least one candidate next-step question is grounded in a concrete prior boundary

## Stage 3: Pick the Idea

Use: `$learning-research`

Load:

- `references/idea.md`
- `assets/templates/idea-card.md`

Goal:

- convert a literature or project gap into a testable hypothesis

Required output:

- `idea-card`

Exit condition:

- the hypothesis, validation path, and main risk are explicit

If the validation path is unclear:

- go back to Stage 2 or narrow the problem

## Stage 4: Baseline and Minimal Experiment

Use: `$learning-research`

Load:

- `references/experiment.md`
- `assets/templates/experiment-log.md`

Goal:

- trust the baseline
- design the smallest experiment that can support or weaken the idea

Required output:

- `experiment-plan`
- `experiment-log`

Exit condition:

- baseline is trusted and the first controlled intervention has been run

If results do not work:

- classify engineering vs research before changing direction

## Stage 5: Weekly Research Loop

Use: `$learning-research`

Load:

- `assets/templates/weekly-research-review.md`

Goal:

- run a stable loop of reading, experiment, interpretation, and next action

Weekly minimum:

1. read or revisit relevant papers
2. run one meaningful experiment block
3. write one experiment log
4. write one weekly review

Required output:

- updated `weekly-research-review`

Exit condition:

- current bottleneck, trusted evidence, and next 1-2 experiments are clear

## Stage 6: Lock the Paper Story

Use: `$learning-research`

Load:

- `references/writing.md`

Goal:

- decide the paper's claims before rewriting sections

Required output:

- `writing-claim-map`

Exit condition:

- each major claim has at least provisional evidence

If claims are vague or unsupported:

- do not switch to `$research-paper-writing` yet

## Stage 7: Draft the Paper

Use: `$research-paper-writing`

Goal:

- rewrite sections into reviewer-facing prose with clear paragraph roles and section logic

Typical order:

1. Introduction
2. Method
3. Experiments
4. Abstract
5. Related Work
6. Conclusion

Required output:

- section outline
- revised section text
- section-level self-review
- claim-evidence checks

Exit condition:

- major sections are readable and aligned with the claim map

If section writing exposes story confusion:

- hand back to `$learning-research`

## Stage 8: Pre-Submission Audit

Use: `$research-paper-writing`

Load:

- `references/paper-review.md`

Goal:

- review like a skeptical reviewer before submission

Required output:

- self-review list
- unresolved risk list

Exit condition:

- contribution, writing clarity, experimental strength, evaluation completeness, and method design all have explicit answers

## Stage 9: Rebuttal

Use: `$learning-research`

Load:

- `references/rebuttal.md`
- `assets/templates/rebuttal-response-plan.md`

Goal:

- classify reviewer concerns
- prioritize the highest-impact responses
- decide whether new experiments are worth doing

Required output:

- `rebuttal-response-plan`

Exit condition:

- each core reviewer concern has a direct answer, supporting evidence, or an explicit scoped limitation

## Canonical Prompt Patterns

Use these patterns consistently:

- `Use $learning-research to turn this paper/project into the next-step experiment plan.`
- `Use $learning-research to read these 3 papers and extract the most natural boundary to attack next.`
- `Use $learning-research to classify whether these failed results indicate an engineering issue or a research issue.`
- `Use $learning-research to build the claim map before we draft the paper.`
- `Use $research-paper-writing to rewrite my Introduction based on this claim map and evidence.`
- `Use $research-paper-writing to self-review my full draft like a skeptical reviewer.`
- `Use $learning-research to build a rebuttal response plan from these reviewer comments.`

## Anti-Patterns

- starting with sentence polishing before the claim map is stable
- starting rebuttal writing before classifying reviewer concerns
- changing project direction before the failure is diagnosed
- reading many papers without extracting boundaries
- writing sections that promise more than the experiments support
