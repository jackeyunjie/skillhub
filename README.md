# Agent Skills

[English](#english) | [简体中文](#中文简体)

---

<a name="中文简体"></a>
## 中文简体

全局、跨平台的 Agent Skill 仓库，覆盖商业公式分析、精益验证与 Codex 工作流。

## Skill 目录

### 商业公式

- `business-formula-core-contradiction-finder`：在做公式分析前，先找到真正的核心矛盾/瓶颈。
- `business-formula-paradigm-selector`：拆解指标前，先选对公式范式。
- `business-formula-parameter-deepener`：把宽泛指标下沉到可操作的 L3-L4 参数。
- `business-formula-qual-to-quant-converter`：把模糊的商业判断转化为可测量指标。
- `business-formula-causality-checker`：审视指标关系是否足够因果，足以指导决策。
- `business-formula-instrumentation-planner`：为公式设计数据节点与证据层。

### 建模（Modeling）

- `modeling-router`：当用户只说“建模”但层级不明时，路由到流程建模、抽象建模或本质提炼。
- `modeling-60-process`：把容易出错的重复任务沉淀为 checklist、SOP 或流程模型。
- `modeling-75-abstract`：把个人直觉/评审经验抽象为可复用的评估框架与评分维度。
- `modeling-85-essence`：把复杂话题压缩成能指导下一步决策的本质定义。

### 精益验证

- `lean-hypothesis-decomposer`：把想法拆分为可排序的验证假设。
- `lean-mvp-test-designer`：为高风险假设设计低成本验证实验。
- `lean-stage-gate-review`：判断验证证据是否足以支持下一阶段投入。
- `lean-evidence-review`：把原始反馈和数据整理为证据等级、结论与下一步行动。

### Codex 工作流

- `agent-first-vault-curator`：把 Agent First Obsidian 知识库整理为可复用知识资产。
- `codex-agent-first-workflow`：把重复性任务变成 Codex 可运行的工作流与自动化。
- `codex-automation-briefing`：设计并运行周期性 Codex 自动化简报与摘要任务。
- `codex-content-factory`：把单一来源转换为内容生产链路。
- `codex-knowledge-base-capture`：把一次成功的 Codex 运行沉淀为 Obsidian 知识资产。
- `codex-query-webapp`：把结构化业务数据变成可搜索的 Web 查询页。
- `codex-talking-head-video-edit`：清理口播/白板视频并重新生成字幕。

### Markdown Skill 笔记

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

## 目录结构

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md

skills/
  <skill-name>.md
```

这些 Skill 尽量避免平台特定的指令，以便不同 Agent 运行时复用。

---

<a name="english"></a>
## English

Global, platform-neutral Agent skills for business formula analysis, lean validation, and Codex workflows.

## Skills

### Business Formula

- `business-formula-core-contradiction-finder`: find the real bottleneck before formula work.
- `business-formula-paradigm-selector`: choose the right formula family before decomposing metrics.
- `business-formula-parameter-deepener`: push broad metrics down to actionable parameters.
- `business-formula-qual-to-quant-converter`: turn fuzzy business judgments into measurable indicators.
- `business-formula-causality-checker`: audit whether a metric relationship is causal enough for decisions.
- `business-formula-instrumentation-planner`: design data nodes and evidence layers behind formulas.

### Modeling

- `modeling-router`: route a modeling request to the right layer when the user is unclear.
- `modeling-60-process`: turn error-prone repeated tasks into checklists, SOPs, or process models.
- `modeling-75-abstract`: convert personal judgment into reusable evaluation frameworks and scoring dimensions.
- `modeling-85-essence`: compress complex topics into essence definitions that guide real decisions.

### Lean Validation

- `lean-hypothesis-decomposer`: decompose ideas into ranked validation assumptions.
- `lean-mvp-test-designer`: design low-cost tests for risky assumptions.
- `lean-stage-gate-review`: decide whether validation evidence supports the next investment stage.
- `lean-evidence-review`: review raw feedback and data into evidence level, status, and next action.

### Codex Workflows

- `agent-first-vault-curator`: curate an Agent First Obsidian vault into reusable knowledge assets.
- `codex-agent-first-workflow`: turn repeatable tasks into Codex-run workflows and automations.
- `codex-automation-briefing`: design and run recurring Codex automations for briefings and summaries.
- `codex-content-factory`: convert a source item into a content production chain.
- `codex-knowledge-base-capture`: turn a successful Codex run into reusable Obsidian knowledge assets.
- `codex-query-webapp`: turn structured business data into a searchable web app.
- `codex-talking-head-video-edit`: clean up talking-head videos and regenerate subtitles.

### Markdown Skill Notes

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

## Structure

```text
.agents/
  skills/
    <skill-name>/
      SKILL.md
      agents/openai.yaml
      references/*.md

skills/
  <skill-name>.md
```

These skills avoid platform-specific instructions and are intended to be reusable by different agent runtimes.
