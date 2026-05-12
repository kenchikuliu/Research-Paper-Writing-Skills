# Skills：Research Paper Writing 与 Learning Research

[English README](./README.md)

> 重要归属说明
> 本仓库中的大部分科研与写作方法论来自彭思达老师公开的学习笔记：
> https://pengsida.notion.site/c1a22465a0fa4b15a12985223916048e
> 彭老师原始仓库：
> https://github.com/pengsida/learning_research
> 非常感谢彭老师公开分享这些宝贵经验。
> 本仓库的主要工作是资料整理、Skills 封装、固定 SOP 设计，以及面向 Codex / Claude Code / Gemini 的适配。

## 仓库介绍

当前仓库提供两个互补的 skill：

- `learning-research/`
  - 面向 `CV`、`3D vision`、`graphics` 及相邻 `ML` 场景的科研操作系统
  - 覆盖读论文、找问题、筛 idea、实验诊断、claim map、roadmap 和 rebuttal 规划
  - 内置固定流程文档：`references/fixed-sop.md`
- `research-paper-writing/`
  - 面向 `ML/CV/NLP` 风格论文的章节级写作与自审 skill
  - 覆盖 `Abstract`、`Introduction`、`Related Work`、`Method`、`Experiments`、`Conclusion`、段落流畅性与 reviewer 视角自审

推荐的分工是：

- 先用 `$learning-research` 决定项目是什么、证据说明了什么、下一步该做什么
- 再用 `$research-paper-writing` 把已经稳定的 story 和 claim map 写成 reviewer-facing 的论文文本

不要反过来。

## 固定 SOP

标准流程在下面两个文件里：

- `learning-research/references/fixed-sop.md`
- `learning-research/assets/templates/cvml-paper-sop-checklist.md`

推荐流程如下：

1. 用 `$learning-research` 定义问题
2. 用 `$learning-research` 读论文并提取边界
3. 写 `idea-card`
4. 跑 baseline 和最小实验
5. 进入周循环复盘
6. 锁定 paper story 和 claim map
7. 用 `$research-paper-writing` 写各章节
8. 用 `$research-paper-writing` 做投稿前自审
9. 用 `$learning-research` 做 rebuttal 规划

## 常见使用场景

### `learning-research`

- 用“下一步是什么”的视角读论文
- 从当前项目里长出下一个问题
- 区分工程问题和研究问题
- 在写论文前先做 claim-evidence 对齐
- 设计多篇论文的 roadmap
- 分类 reviewer 意见并制定 rebuttal 策略

### `research-paper-writing`

- 撰写或重写 `Abstract`、`Introduction`、`Method`、`Experiments`、`Conclusion`
- 改善段落流畅性与章节逻辑
- 做 claim-evidence 对齐检查
- 从 reviewer 视角做投稿前自审

## 安装方式

以下命令默认在仓库根目录执行。

### 1）Codex

建议两个 skill 一起安装：

```bash
mkdir -p "$CODEX_HOME/skills"
cp -R learning-research "$CODEX_HOME/skills/"
cp -R research-paper-writing "$CODEX_HOME/skills/"
```

使用示例：

```text
Use $learning-research to follow the fixed SOP for my current CV/ML project.
```

```text
Use $research-paper-writing to rewrite my Introduction based on this claim map and evidence.
```

### 2）CC（Claude Code）

可选择全局安装或项目级安装。

全局安装：

```bash
mkdir -p "$HOME/.claude/skills"
cp -R learning-research "$HOME/.claude/skills/"
cp -R research-paper-writing "$HOME/.claude/skills/"
```

项目级安装：

```bash
mkdir -p .claude/skills
cp -R learning-research .claude/skills/
cp -R research-paper-writing .claude/skills/
```

推荐提示词：

- `Please use the learning-research skill to decide my next experiment.`
- `Please use the research-paper-writing skill to rewrite my Method section.`

### 3）Gemini

可将两个 skill 一起复制到 Gemini 的技能目录：

```bash
mkdir -p "$HOME/.gemini/skills"
cp -R learning-research "$HOME/.gemini/skills/"
cp -R research-paper-writing "$HOME/.gemini/skills/"
```

随后可直接提问：

- `Use $learning-research to classify my current project stage and next artifact.`
- `Use $research-paper-writing to improve my Abstract and run claim-evidence checks.`

## 推荐入口提示词

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

## 致谢

再次说明：仓库核心知识主要来自彭思达老师公开笔记；这里的工作重点是整理、Skills 化、SOP 设计与多 Agent 适配。
彭老师原始仓库：https://github.com/pengsida/learning_research

## 许可证

本项目采用 MIT License，详见 [LICENSE](./LICENSE)。
