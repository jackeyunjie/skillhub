# Automation Task Spec

## Purpose

Use this when a repeated task is stable enough to be scheduled and archived automatically.

## 适用场景

- 每日情报
- 周报生成
- 数据巡检
- 目录变更总结
- 定时执行某个已存在的 skill

## 输入模板

```text
Task name:
Goal:
Trigger time:
Frequency:
Input sources:
Processing rules:
Output path:
Output format:
Completion summary:
Failure handling:
```

## 输出要求

- 自动化名称清晰
- 触发时间明确
- 输入源可枚举
- 产出路径固定
- 完成汇报简短可扫读
- 失败时能说明缺了什么

## 设计规则

- 优先从已经手工跑通的任务开始
- 输出路径必须显式写出
- Completion summary 只保留最重要的结果
- 如果有多数据源，要标记覆盖率和缺失源
- 高风险输出保留人工 review 点

## 推荐提示词

```text
请把下面这个重复任务设计成一个可定时运行的自动化。

Task name: ...
Goal: ...
Trigger time: ...
Frequency: ...
Input sources: ...
Processing rules: ...
Output path: ...
Output format: ...
Completion summary: ...
Failure handling: ...
```

## 常见失败

- 只有目标，没有输入源
- 只有内容要求，没有落盘路径
- 让自动化承担了太多互相无关的任务
- 没定义失败后的最小反馈

## 相关页面

- [Workflows/daily-intel-pipeline.md](../Workflows/daily-intel-pipeline.md)
- [Concepts/automation-first.md](../Concepts/automation-first.md)
- [Concepts/agent-first-decision-rules.md](../Concepts/agent-first-decision-rules.md)
