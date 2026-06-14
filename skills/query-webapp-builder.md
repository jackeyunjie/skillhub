# Query Webapp Builder Skill

## Purpose

Turn a structured spreadsheet into a searchable web app with clear query keys, safe data handling, and a repeatable update path.

## Best Use Cases

- 快递查询
- 订单查询
- 客户查询
- 库存查询
- 活动报名查询

## Input Contract

- Data file path
- Main lookup keys
- Optional disambiguation keys
- Fields to show in results
- Privacy constraints
- Local preview requirement
- Deployment target

## Output Contract

- Local runnable app
- Query form with business-friendly fields
- Server-side data handling when needed
- Update method for new spreadsheet drops
- Deployment notes

## Working Rules

- 先识别数据结构，再设计查询字段
- 只暴露查询结果所需字段
- 敏感数据不要直接打进前端静态文件
- 本地先验证再部署
- 给出下一次增量更新的方法

## Prompt Shape

```text
把这份结构化数据做成一个查询网页。

Data file: ...
Users query by: ...
Optional filter: ...
Show fields: ...
Privacy constraints: ...
Need local preview: yes/no
Need deployment: local only / GitHub + Vercel
```

## Quality Gates

- 查询字段足够少，用户能直接理解
- 返回结果准确，不泄露无关数据
- 本地地址可访问
- 线上部署时数据不裸露在公开静态文件里

## Failure Modes

- 把原始数据整个暴露给前端
- 查询条件设计得太技术化
- 忽略数据清洗和空值
- 没有后续更新方案

## Related Notes

- [Workflows/query-webapp-pipeline.md](../Workflows/query-webapp-pipeline.md)
- [Concepts/capability-boundaries.md](../Concepts/capability-boundaries.md)
- [Concepts/agent-first-decision-rules.md](../Concepts/agent-first-decision-rules.md)
