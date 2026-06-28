# Agent SkillHub

[English](#english) | [简体中文](#中文简体)

一个跨平台、可复用的 Agent Skill 集合仓库，覆盖商业分析、精益验证、Codex 工作流，以及精选的外部高质量技能集。

---

<a name="中文简体"></a>
## 中文简体

### 这是什么

SkillHub 收集并整理可在 Kimi、Claude、Codex、Cursor 等多种 Agent 运行时中复用的 Skill。

仓库包含三类内容：

1. **`.agents/skills/`** —— 结构化的 OpenAI Agents SDK 格式 Skill，每个 Skill 包含 `SKILL.md`、可选的 `agents/openai.yaml` 与 `references/` 参考资料。
2. **`skills/`** —— 单文件 Markdown Skill，便于快速复制、粘贴和修改。
3. **`mattpocock-skills/`** —— 精选导入的 [mattpocock/skills](https://github.com/mattpocock/skills) 仓库，面向真实工程场景，包含 35 个 Skill。

---

### 原生 Skill 目录

#### 商业公式

#### 商业公式

- `business-formula`（根目录）：一堂方法论，用业务公式把拆解、假设管理、验证迭代串成可执行操盘方法。
- `business-formula-core-contradiction-finder`：在做公式分析前，先找到真正的核心矛盾/瓶颈。
- `business-formula-paradigm-selector`：拆解指标前，先选对公式范式。
- `business-formula-parameter-deepener`：把宽泛指标下沉到可操作的 L3-L4 参数。
- `business-formula-qual-to-quant-converter`：把模糊的商业判断转化为可测量指标。
- `business-formula-causality-checker`：审视指标关系是否足够因果，足以指导决策。
- `business-formula-instrumentation-planner`：为公式设计数据节点与证据层。

#### 建模（Modeling）

- `modeling-router`：当用户只说“建模”但层级不明时，路由到流程建模、抽象建模或本质提炼。
- `modeling-60-process`：把容易出错的重复任务沉淀为 checklist、SOP 或流程模型。
- `modeling-75-abstract`：把个人直觉/评审经验抽象为可复用的评估框架与评分维度。
- `modeling-85-essence`：把复杂话题压缩成能指导下一步决策的本质定义。

#### 精益验证

#### 精益验证

- `key-hypothesis-prioritizer`（根目录）：把模糊业务问题排序为按阶段、依赖与致死风险排列的假设清单。
- `lean-mvp-experiment-design`（根目录）：为业务假设设计最低成本可证伪/支持的精益实验。
- `lean-validation-triage`（根目录）：为业务不确定性选择最低成本的验证手段（常识、专家、竞品、调研、实验）。
- `validation-milestone-review`（根目录）：复盘验证证据，决定样本是否足够、是否进入下一阶段。
- `lean-hypothesis-decomposer`：把想法拆分为可排序的验证假设。
- `lean-mvp-test-designer`：为高风险假设设计低成本验证实验。
- `lean-stage-gate-review`：判断验证证据是否足以支持下一阶段投入。
- `lean-evidence-review`：把原始反馈和数据整理为证据等级、结论与下一步行动。

#### Codex 工作流

#### Codex 工作流

### S级私董会

- `npc-ai-practice-system`（根目录）：把 S 级私董会/NPC 练习流程落地为可执行工作流、检查清单、Prompt 系统或 Agent 设计。
- `s-private-board-grouping`（根目录）：整理私董会分组规则、NPC 角色设计、案主准备度、S1/S2/S3/S4 选拔逻辑与行为权重治理。

- `agent-first-vault-curator`：把 Agent First Obsidian 知识库整理为可复用知识资产。
- `codex-agent-first-workflow`：把重复性任务变成 Codex 可运行的工作流与自动化。
- `codex-automation-briefing`：设计并运行周期性 Codex 自动化简报与摘要任务。
- `codex-content-factory`：把单一来源转换为内容生产链路。
- `codex-knowledge-base-capture`：把一次成功的 Codex 运行沉淀为 Obsidian 知识资产。
- `codex-query-webapp`：把结构化业务数据变成可搜索的 Web 查询页。
- `codex-talking-head-video-edit`：清理口播/白板视频并重新生成字幕。

#### Markdown Skill 笔记

#### Markdown Skill 笔记

- `course-to-obsidian`（根目录）：把课程/文档链接整理为完整参考文档 + 一页速查双笔记，并更新 Obsidian README 索引。
以单文件 Markdown 形式保存的 Skill 规范。

- `ai-daily-radar`：自动化每日情报雷达。
- `automation-task-spec`：自动化任务规格。
- `codex-intel-collector`：用 Codex 收集并结构化情报。
- `codex-workflow-builder`：构建可复用的 Codex 工作流。
- `html-brief-generator`：从来源生成 HTML 简报。
- `obsidian-vault-curator`：为 Agent 使用整理 Obsidian 知识库。
- `paper-board-html`：将看板内容渲染为 HTML。
- `query-webapp-builder`：从结构化数据构建查询 Webapp。
- `videocut-skills`：视频剪辑与清理 Skill。
- `课程能力转AI工具`：把一门课程的方法论迁移为可复用 AI 工具 / PRD。
- `AI调研教练对话`：用结构化多轮对话完成证据型调研。
- `证据型追问`：把 AI 的推理型回答升级为证据型回答。
- `如何做成好的Skill`：判断课程资料是否值得做 Skill，并做出可测试、可安装、可迭代的 Skill。

---

### 精选外部技能集：Matt Pocock Skills

仓库已完整导入 [`mattpocock/skills`](https://github.com/mattpocock/skills)，位于 `mattpocock-skills/` 目录。

这些 Skill 面向真实工程场景，小而可组合，可在 Codex、Claude Code、Cursor 等环境中通过 `/` 命令调用。主要分类：

#### Engineering

- `/ask-matt`：把棘手工程问题交给结构化分析流程。
- `/codebase-design`：为变更做系统化代码库设计。
- `/diagnosing-bugs`：结构化定位和修复 Bug。
- `/domain-modeling`：构建领域模型并产出 ADR / CONTEXT 文档。
- `/grill-with-docs`：在动手前通过提问对齐需求，并建立共享语言。
- `/implement`：在已明确规格后执行实现。
- `/improve-codebase-architecture`：系统性改进代码库架构。
- `/prototype`：快速原型并验证想法。
- `/resolving-merge-conflicts`：处理合并冲突。
- `/setup-matt-pocock-skills`：初始化配置（Issue 追踪器、标签、文档位置）。
- `/tdd`：测试驱动开发。
- `/to-issues`：把对话内容转换为 Issue。
- `/to-prd`：把对话内容转换为 PRD。
- `/triage`：对 Issue 进行分类和优先级排序。

#### Productivity

- `/grill-me`：非代码场景的需求对齐提问。
- `/grilling`：通用 grilling 框架。
- `/handoff`：生成清晰的任务交接文档。
- `/teach`：把知识整理为教学材料。
- `/writing-great-skills`：写出高质量的 Skill。

#### Misc / Personal / In-progress / Deprecated

还包括 Git 护栏、Obsidian Vault、pre-commit 设置、写作辅助等 Skill，以及若干实验和已弃用 Skill。详见 `mattpocock-skills/README.md`。

---

### 目录结构

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md

skills/
  <skill-name>.md

mattpocock-skills/
  .claude-plugin/plugin.json
  skills/
    engineering/
    productivity/
    misc/
    personal/
    in-progress/
    deprecated/

# 根目录独立 Skill（来自 main 分支）
business-formula/
course-to-obsidian/
key-hypothesis-prioritizer/
lean-mvp-experiment-design/
lean-validation-triage/
npc-ai-practice-system/
s-private-board-grouping/
validation-milestone-review/
```

这些 Skill 尽量避免平台特定的指令，以便不同 Agent 运行时复用。

> 注意：`business-formula`、`course-to-obsidian`、`key-hypothesis-prioritizer`、`lean-mvp-experiment-design`、`lean-validation-triage`、`npc-ai-practice-system`、`s-private-board-grouping`、`validation-milestone-review` 位于仓库根目录，是早期在 `main` 分支维护的独立 Skill，现已合并到 `master`。

---

### 快速使用

**在 Kimi Code CLI 中使用**

Kimi 会自动识别项目内的 `.agents/skills/`、`.codex/skills/`、`.kimi/skills/` 等目录中的 Skill。启动 Kimi 后，Agent 会根据任务自动读取相关 `SKILL.md`，你也可以手动调用：

```bash
/skill:<skill-name>
```

例如：

```bash
/skill:grill-with-docs
/skill:codex-agent-first-workflow
```

**在 Codex / Claude Code 中使用**

Codex 会通过 `.claude-plugin/plugin.json` 加载 `mattpocock-skills/` 中的 Skill。首次使用建议运行：

```bash
/setup-matt-pocock-skills
```

---

### 贡献与更新

- 新增原生 Skill：在 `.agents/skills/` 或 `skills/` 中按现有结构添加。
- 更新外部技能集：重新导入 `mattpocock/skills` 并覆盖 `mattpocock-skills/` 目录。
- 保持 Skill 尽量平台无关，便于跨 Agent 复用。

---

<a name="english"></a>
## English

### What is this

SkillHub is a cross-platform, reusable collection of Agent Skills for Kimi, Claude, Codex, Cursor, and other agent runtimes.

The repository contains three types of content:

1. **`.agents/skills/`** — Structured OpenAI Agents SDK-style skills. Each skill includes `SKILL.md`, optional `agents/openai.yaml`, and `references/` docs.
2. **`skills/`** — Single-file Markdown skills for quick copy-paste-modify usage.
3. **`mattpocock-skills/`** — Curated import of [mattpocock/skills](https://github.com/mattpocock/skills), with 35 skills for real engineering work.

---

### Native Skill Catalog

#### Business Formula

#### Business Formula

- `business-formula` (root): a one-course methodology that turns business decomposition, hypothesis management, and validation iteration into an executable operating system.
- `business-formula-core-contradiction-finder`: find the real bottleneck before formula work.
- `business-formula-paradigm-selector`: choose the right formula family before decomposing metrics.
- `business-formula-parameter-deepener`: push broad metrics down to actionable parameters.
- `business-formula-qual-to-quant-converter`: turn fuzzy business judgments into measurable indicators.
- `business-formula-causality-checker`: audit whether a metric relationship is causal enough for decisions.
- `business-formula-instrumentation-planner`: design data nodes and evidence layers behind formulas.

#### Modeling

- `modeling-router`: route a modeling request to the right layer when the user is unclear.
- `modeling-60-process`: turn error-prone repeated tasks into checklists, SOPs, or process models.
- `modeling-75-abstract`: convert personal judgment into reusable evaluation frameworks and scoring dimensions.
- `modeling-85-essence`: compress complex topics into essence definitions that guide real decisions.

#### Lean Validation

#### Lean Validation

- `key-hypothesis-prioritizer` (root): turn a fuzzy business question into a ranked hypothesis list ordered by stage, dependency, and fatal risk.
- `lean-mvp-experiment-design` (root): design the lightest experiment that can disconfirm or support a business hypothesis.
- `lean-validation-triage` (root): choose the cheapest reliable validation method for a business uncertainty.
- `validation-milestone-review` (root): review validation evidence and decide whether to continue, stop, pivot, or enter the next stage.
- `lean-hypothesis-decomposer`: decompose ideas into ranked validation assumptions.
- `lean-mvp-test-designer`: design low-cost tests for risky assumptions.
- `lean-stage-gate-review`: decide whether validation evidence supports the next investment stage.
- `lean-evidence-review`: review raw feedback and data into evidence level, status, and next action.

#### Codex Workflows

#### Codex Workflows

### S-Level Private Board

- `npc-ai-practice-system` (root): land S-level private-board / NPC practice into executable workflows, checklists, prompt systems, or agent designs.
- `s-private-board-grouping` (root): structure private-board grouping rules, NPC roles, case-owner readiness, S1/S2/S3/S4 selection logic, and behavior-weight governance.

- `agent-first-vault-curator`: curate an Agent First Obsidian vault into reusable knowledge assets.
- `codex-agent-first-workflow`: turn repeatable tasks into Codex-run workflows and automations.
- `codex-automation-briefing`: design and run recurring Codex automations for briefings and summaries.
- `codex-content-factory`: convert a source item into a content production chain.
- `codex-knowledge-base-capture`: turn a successful Codex run into reusable Obsidian knowledge assets.
- `codex-query-webapp`: turn structured business data into a searchable web app.
- `codex-talking-head-video-edit`: clean up talking-head videos and regenerate subtitles.

#### Markdown Skill Notes

#### Markdown Skill Notes

- `course-to-obsidian` (root): turn a course or document link into a full reference note plus a one-page quick-reference note, and update the Obsidian README index.
Standalone skill specifications kept as single Markdown files.

- `ai-daily-radar`: automated daily intelligence radar.
- `automation-task-spec`: task specification for automations.
- `codex-intel-collector`: collect and structure intelligence with Codex.
- `codex-workflow-builder`: build reusable Codex workflows.
- `html-brief-generator`: generate HTML briefs from sources.
- `obsidian-vault-curator`: curate Obsidian vaults for agent use.
- `paper-board-html`: render paper board content as HTML.
- `query-webapp-builder`: build query webapps from structured data.
- `videocut-skills`: video editing skills for cutting and cleanup.
- `course-to-ai-tool`: turn a course methodology into a reusable AI tool / PRD.
- `ai-research-coach-chat`: complete evidence-based research through structured multi-turn dialogue.
- `evidence-pusher`: upgrade AI reasoning answers into evidence-based answers.
- `good-skill-maker`: judge whether course material is worth turning into a skill, and build a testable, installable, iterable skill.

---

### Curated External Skill Collection: Matt Pocock Skills

The repository includes a full import of [`mattpocock/skills`](https://github.com/mattpocock/skills) under `mattpocock-skills/`.

These skills are designed for real engineering: small, composable, and callable via `/` commands in Codex, Claude Code, Cursor, and similar tools. Main categories:

#### Engineering

- `/ask-matt`: hand tricky engineering problems to a structured analysis flow.
- `/codebase-design`: do systematic codebase design before changing code.
- `/diagnosing-bugs`: locate and fix bugs with a structured process.
- `/domain-modeling`: build domain models and produce ADR / CONTEXT docs.
- `/grill-with-docs`: align on requirements through questions and build a shared language.
- `/implement`: execute implementation after specs are clear.
- `/improve-codebase-architecture`: systematically improve codebase architecture.
- `/prototype`: rapidly prototype and validate ideas.
- `/resolving-merge-conflicts`: handle merge conflicts.
- `/setup-matt-pocock-skills`: initial setup (issue tracker, labels, docs location).
- `/tdd`: test-driven development.
- `/to-issues`: turn a conversation into issues.
- `/to-prd`: turn a conversation into a PRD.
- `/triage`: classify and prioritize issues.

#### Productivity

- `/grill-me`: non-code requirement alignment through questioning.
- `/grilling`: general grilling framework.
- `/handoff`: produce clear handoff documents.
- `/teach`: turn knowledge into teaching materials.
- `/writing-great-skills`: write high-quality skills.

#### Misc / Personal / In-progress / Deprecated

Also includes Git guardrails, Obsidian Vault, pre-commit setup, writing aids, and several experimental or deprecated skills. See `mattpocock-skills/README.md` for details.

---

### Structure

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md

skills/
  <skill-name>.md

mattpocock-skills/
  .claude-plugin/plugin.json
  skills/
    engineering/
    productivity/
    misc/
    personal/
    in-progress/
    deprecated/

# Root-level standalone skills (from main branch)
business-formula/
course-to-obsidian/
key-hypothesis-prioritizer/
lean-mvp-experiment-design/
lean-validation-triage/
npc-ai-practice-system/
s-private-board-grouping/
validation-milestone-review/
```

These skills avoid platform-specific instructions and are intended to be reusable by different agent runtimes.

> Note: `business-formula`, `course-to-obsidian`, `key-hypothesis-prioritizer`, `lean-mvp-experiment-design`, `lean-validation-triage`, `npc-ai-practice-system`, `s-private-board-grouping`, and `validation-milestone-review` live at the repository root. They were originally maintained on the `main` branch and have now been merged into `master`.

---

### Quick Start

**Using with Kimi Code CLI**

Kimi automatically discovers skills in project-level directories such as `.agents/skills/`, `.codex/skills/`, and `.kimi/skills/`. After launching Kimi, the Agent reads relevant `SKILL.md` files based on the task, or you can invoke them manually:

```bash
/skill:<skill-name>
```

Examples:

```bash
/skill:grill-with-docs
/skill:codex-agent-first-workflow
```

**Using with Codex / Claude Code**

Codex loads skills from `mattpocock-skills/` via `.claude-plugin/plugin.json`. For first-time setup, run:

```bash
/setup-matt-pocock-skills
```

---

### Contributing and Updates

- Add native skills under `.agents/skills/` or `skills/` following the existing structure.
- Update the external collection by re-importing `mattpocock/skills` and overwriting the `mattpocock-skills/` directory.
- Keep skills as platform-agnostic as possible so they remain reusable across agents.
