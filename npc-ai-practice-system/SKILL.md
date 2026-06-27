---
name: npc-ai-practice-system
description: Use when designing, reviewing, or landing AI-assisted NPC/S级私董会 workflows, including 破冰评估、会前背调、会前推演、文本打磨、会后复盘、问答测评、双图传播、Skill/Agent 沉淀.
---

# NPC AI Practice System

Use this skill when the task is to turn NPC/private-board AI practice into an executable workflow, checklist, prompt system, or agent design. This is for landing documents and operational artifacts, not for general coaching.

## Core Workflow

Run NPC AI work as a staged chain:

1. **破冰启动**: structure member introductions, goals, pain points, resources, and commitments.
2. **会前背调**: research the case owner, industry, users, competitors, business model, and known constraints.
3. **文本打磨**: check whether the case material has a clear target outlet, sufficient context, and discussable tension.
4. **会前推演**: simulate case owner, 木梁, NPC, challenger, and methodology coach roles.
5. **会后复盘**: structure the meeting, score question quality, extract assumptions, and define next actions.
6. **传播资产**: generate group-photo/poster/praise-copy assets when consent and privacy conditions are satisfied.
7. **结营观察报告**: generate group assessment reports and personal observation cards from final group-interview transcripts.
8. **长期沉淀**: convert stable workflows into templates, skills, agents, and checklists.

## Sub Workflows

### 1. 破冰评估

Use when the input is an icebreaker meeting, opening call, or member introduction.

Output:

- Structured member map: goals, current stage, constraints, asks, resources.
- Qualitative evaluation: what worked, what was unclear, what needs follow-up.
- Quantitative evaluation: 0-5 score per dimension, with evidence.
- Action conversion: deliberate practice, mutual support, key assumptions, social copy.

### 2. AI 调研

Use AI as a research staffer, not as the final judge.

Keep this boundary:

- AI: scenario generation, secondary information, interview outline, theme extraction, hypothesis drafting.
- Human: first-hand interviews, trust building, context judgment, direction selection, final decision.

Recommended flow:

1. Generate 100 vertical scenarios or problem angles.
2. Human selects 10 likely directions.
3. AI deepens secondary information and competing approaches.
4. AI and human design interview questions.
5. Human interviews at least 5 real users.
6. AI extracts themes and user language.
7. Human selects 1-2 directions.
8. AI drafts storyboard, smoke test, or MVP copy.

### 3. 会前制胜

Highest leverage is before the meeting.

Timeline:

- Two weeks before: topic selection support.
- One week before: case text polishing.
- One to two days before: meeting simulation.
- Same day after: targeted action and follow-up plan.

Always ask AI to produce:

- What it understands.
- What it does not understand.
- What it would ask next.
- Where the meeting may go off track.

### 4. 上下文管理

Do not rely on a single prompt. Manage context with six elements:

- Goal
- Role
- Key information
- Behavior rules
- Output format
- Feedback mechanism

Check output quality with:

- Facts: source and traceability.
- Logic: whether conclusions follow from evidence.
- Demand fit: whether it answers the real task.
- Completeness: whether roles, constraints, and boundaries are missing.
- Executability: whether it becomes an action, question, or validation plan.

### 5. 问答测评

Use for private-board question/answer review.

Nine dimensions:

- Question: openness, inspiration, target relevance, future orientation, methodology relevance, value alignment.
- Answer: target-outlet relevance, blind-spot expansion, positive emotion.

Scoring method:

- Let AI do addition: propose dimensions, rubrics, and evidence.
- Let humans do subtraction: remove weak dimensions and set the final rubric.
- Use a scale that fits the task: binary, A/B/C, 0-5, or 0-100.
- Validate with real meeting outcomes.

### 6. 双图传播

Use after online meetings when the user wants emotional value and community cohesion.

Assets:

- AI cloud group photo: identity, ceremony, group memory.
- Q-style praise poster: recognition, positive feedback, shareability.

Guardrails:

- Obtain consent before using real portraits.
- Avoid embarrassing or exaggerated images.
- Keep image text short; place long text in the message body.

### 7. 结营群面观察报告

Use when the input is a final group-interview transcript and the output should be an observation report or card.

Output two artifacts:

- Group assessment report: group summary, discussion process, consensus formation, coach-style collaboration, boundary note.
- Personal observation card: participation overview, observable business-analysis behavior, observable collaboration behavior, boundary note.

Strict boundaries:

- Only describe behavior observable in this single simulated scene.
- Do not rank members.
- Do not certify ability level.
- Do not infer long-term capability or personality.
- Do not treat silence as low ability.

## Output Templates

### NPC Meeting Prep Package

```markdown
## Case Snapshot
- Case owner:
- Target outlet:
- Business stage:
- Known constraints:

## AI Research Map
| Topic | Findings | Evidence | Open Questions |
|---|---|---|---|

## Meeting Simulation
| Role | Likely View | Best Questions | Risks |
|---|---|---|---|

## NPC Intervention Plan
1.
2.
3.
```

### Post Meeting Review

```markdown
## Meeting Summary

## Question Quality Score
| Dimension | Score | Evidence | Improvement |
|---|---:|---|---|

## Key Assumptions
| Assumption | Evidence | Validation Action | Owner | Deadline |
|---|---|---|---|---|

## Follow-up
- Deliberate practice:
- Mutual support:
- Next meeting input:
```

### Agent Design

```markdown
## Agent Purpose

## Trigger

## Required Inputs

## Steps
1.
2.
3.

## Human Checkpoints

## Output Contract

## Failure Handling
```

## Related Vault Notes

- `03-参考文档/NPC内训-人工智能基本功L1-私董会NPC实战落地场景.md`
- `03-参考文档/NPC内训-私董会问答测评提示词优化.md`
- `03-参考文档/NPC内训-Day2小组共建-私董会问答测评工作流.md`
- `03-参考文档/NPC内训-高阶组官方AI行动指南.md`
- `03-参考文档/NPC内训-结营群面观察报告与个人观察卡模板.md`
- `03-参考文档/NPC内训-德龙-AI破冰评估.md`
- `03-参考文档/NPC内训-SiSi-如何用AI做调研.md`
- `03-参考文档/NPC内训-天末-AI会前制胜四步法.md`
- `03-参考文档/NPC内训-维东-从提示词到上下文管理.md`
- `03-参考文档/NPC内训-柴翔-双图引爆法.md`
- `03-参考文档/NPC内训-李蕊-从手搓Skill到Agent案例.md`
