# Skills: Research Paper Writing and Learning Research

[中文介绍](./README_zh.md).

> Important Attribution
> Most research and writing methodology in this repository comes from Prof. Peng Sida's open study notes:
> https://pengsida.notion.site/c1a22465a0fa4b15a12985223916048e
> Prof. Peng's original repository:
> https://github.com/pengsida/learning_research
> I sincerely thank Prof. Peng for openly sharing these valuable experiences.
> The contribution in this repository is curation, skill packaging, workflow structuring, and agent-friendly adaptation.

## Repository Overview

This repository now provides two complementary skill packages:

- `learning-research/`
  - practical research operating system for `CV`, `3D vision`, `graphics`, and adjacent `ML`
  - covers paper reading, problem finding, idea filtering, experiment diagnosis, claim mapping, roadmap design, and rebuttal planning
  - includes a fixed cross-skill SOP in `references/fixed-sop.md`
- `research-paper-writing/`
  - section-level academic writing and self-review skill for `ML/CV/NLP`-style papers
  - covers `Abstract`, `Introduction`, `Related Work`, `Method`, `Experiments`, `Conclusion`, paragraph flow, and reviewer-style self-review

The intended split is:

- use `$learning-research` to decide what the project is, what the evidence means, and what the next research step should be
- use `$research-paper-writing` to turn a stable story and claim map into reviewer-facing paper sections

Do not reverse that order.

## Fixed SOP

The standard workflow is documented in:

- `learning-research/references/fixed-sop.md`
- `learning-research/assets/templates/cvml-paper-sop-checklist.md`

Recommended flow:

1. Scope the problem with `$learning-research`
2. Read papers for boundaries with `$learning-research`
3. Write an `idea-card`
4. Run baseline and minimal experiments
5. Iterate with weekly research review
6. Lock the paper story and claim map
7. Draft sections with `$research-paper-writing`
8. Run pre-submission self-review with `$research-paper-writing`
9. Build rebuttal responses with `$learning-research`

## Typical Use Cases

### `learning-research`

- read papers with a "what next?" lens
- find the next problem from a current project
- separate engineering failures from research failures
- create a claim map before writing
- build a multi-paper roadmap
- classify reviewer comments and plan rebuttal work

### `research-paper-writing`

- rewrite or draft `Abstract`, `Introduction`, `Method`, `Experiments`, or `Conclusion`
- improve paragraph flow and section logic
- run claim-evidence alignment checks
- perform adversarial self-review before submission

## Installation

Assume you are in the repository root.

### 1) Codex

Install both skills:

```bash
mkdir -p "$CODEX_HOME/skills"
cp -R learning-research "$CODEX_HOME/skills/"
cp -R research-paper-writing "$CODEX_HOME/skills/"
```

Usage examples:

```text
Use $learning-research to follow the fixed SOP for my current CV/ML project.
```

```text
Use $research-paper-writing to rewrite my Introduction based on this claim map and evidence.
```

### 2) CC (Claude Code)

Use either a global or project-level installation.

Global:

```bash
mkdir -p "$HOME/.claude/skills"
cp -R learning-research "$HOME/.claude/skills/"
cp -R research-paper-writing "$HOME/.claude/skills/"
```

Project-level:

```bash
mkdir -p .claude/skills
cp -R learning-research .claude/skills/
cp -R research-paper-writing .claude/skills/
```

Recommended prompts:

- `Please use the learning-research skill to decide my next experiment.`
- `Please use the research-paper-writing skill to rewrite my Method section.`

### 3) Gemini

Copy both skills into your Gemini skills directory:

```bash
mkdir -p "$HOME/.gemini/skills"
cp -R learning-research "$HOME/.gemini/skills/"
cp -R research-paper-writing "$HOME/.gemini/skills/"
```

Then ask concrete tasks such as:

- `Use $learning-research to classify my current project stage and next artifact.`
- `Use $research-paper-writing to improve my Abstract and run claim-evidence checks.`

## Recommended Entry Prompts

```text
Use $learning-research to turn my current paper/project into the next-step experiment plan.
```

```text
Use $learning-research to read these papers and extract the most natural boundary to attack next.
```

```text
Use $research-paper-writing to rewrite my Introduction based on this claim map and evidence.
```

```text
Use $research-paper-writing to self-review my full draft like a skeptical reviewer.
```

## Credits

Again, this repository is primarily based on Prof. Peng Sida's open notes, while the work here focuses on curation, Skills packaging, SOP design, and cross-agent adaptation.
Prof. Peng's original repository: https://github.com/pengsida/learning_research

## License

This project is licensed under the MIT License. See [LICENSE](./LICENSE).
