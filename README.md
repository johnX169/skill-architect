# Skill Architect

Prompt 与 Agent 架构审查官 / Prompt & Agent Architecture Review

中文 | [English](#english)

`Skill Architect` 是一个用于审查 skill、agent、prompt system 和工程结构的 Codex Skill。它不是简单总结器，而是你的“Prompt 与 Agent 架构审查官”：先读全材料，再梳理结构、追踪执行流程、识别隐式依赖、评估风险，并给出可落地的重构建议。

## 适合什么场景

- 分析一个 Codex Skill 或 Agent 的设计是否清楚
- 检查 prompt system 的触发条件、执行流程和隐藏假设
- 找出技能目录中的隐式依赖、维护风险和安全边界
- 给已有 skill / prompt / agent 做架构审查
- 将复杂工程结构拆成组件、边界、数据流和风险点

## 输出内容

这个 skill 默认会输出：

- 分析范围：说明实际读取了哪些文件，以及结论边界
- 关键结论：先给 3-5 条最高价值发现
- 架构总览：组件、边界、关系图和设计模式
- 执行流程：触发、步骤、分支、产物和控制流
- 设计意图推断：解释为什么这样设计，以及换一种设计会坏在哪里
- 隐式依赖：工具、模型能力、环境、约定和知识依赖
- 风险评估：鲁棒性、可维护性、可扩展性、正确性和安全风险
- 重构建议：按优先级给出具体改法、收益和成本

## 仓库内容

- `skill-architect/SKILL.md`：Codex Skill 定义文件
- `skill-architect.zip`：打包好的 skill 目录

## 使用方式

把 `skill-architect/` 目录放到你的 Codex skills 目录中，或使用 `skill-architect.zip` 作为可分发版本。

典型触发语：

- “review this skill”
- “analyze this agent”
- “这个 prompt system 有什么风险？”
- “帮我检查这个 skill 的架构”
- “为什么这个 agent 要这样设计？”

## 安全说明

这个仓库只包含 `skill-architect` 本体。它刻意排除了本地 Wiki、个人记录、系统元数据和其他私有内容。

---

## English

`Skill Architect` is a Codex Skill for reviewing the architecture of skills, agents, prompt systems, and engineering structures. It is not a simple summarizer. Think of it as a prompt and agent architecture reviewer: it reads the relevant materials first, maps the structure, traces execution flow, identifies implicit dependencies, evaluates risks, and proposes grounded refactoring suggestions.

## When To Use It

- Review whether a Codex Skill or Agent is clearly designed
- Inspect trigger conditions, execution flow, and hidden assumptions in a prompt system
- Identify implicit dependencies, maintainability risks, and safety boundaries
- Perform an architecture review for an existing skill, prompt, or agent
- Break down a complex engineering structure into components, boundaries, data flow, and risks

## Output

The skill is designed to produce:

- Analysis Scope: what files or materials were actually read, and where the confidence boundary is
- Key Findings: 3-5 high-value findings up front
- Architecture Overview: components, boundaries, relationship diagram, and design patterns
- Execution Flow: triggers, steps, branches, outputs, and control flow
- Design Intent Inference: why the system is likely designed this way, and what would break if changed
- Implicit Dependencies: tools, model capabilities, environment, conventions, and knowledge assumptions
- Risk Assessment: robustness, maintainability, scalability, correctness, and security risks
- Refactoring Suggestions: prioritized changes with benefits and tradeoffs

## Repository Contents

- `skill-architect/SKILL.md`: the Codex Skill definition
- `skill-architect.zip`: packaged copy of the skill directory

## Usage

Place the `skill-architect/` directory in your Codex skills directory, or use `skill-architect.zip` as the distributable package.

Example trigger phrases:

- "review this skill"
- "analyze this agent"
- "what are the risks in this prompt system?"
- "check the architecture of this skill"
- "why is this agent designed this way?"

## Safety Note

This repository only contains the `skill-architect` skill itself. Local Wiki notes, personal records, OS metadata, and other private materials are intentionally excluded.
