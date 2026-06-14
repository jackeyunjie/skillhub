# ai-daily-radar

## 来源

原文《教学文档---260612 Agent First：用Codex重新设计你的工作流》中明确点名的自动化 skill。

## 运行方式

- 每天早上 7 点自动运行
- 作为一个已存在 skill 被自动化调度

## 它在原文中的要求

1. 采集和整合多个信息来源
2. 优先使用一手来源
3. 标注缺失来源
4. 生成 Markdown 报告
5. 生成同目录 HTML 报告
6. 输出简短完成汇报

## 原文中的输入来源

- ApifyX Watchlist
- follow-builders
- video-info-radar
- huangshudaily

## 原文中的落盘路径

- Markdown：`01-内容生产/内容数据统计/AI每日情报/YYYY-MM-DD_AI每日情报.md`
- HTML：同目录下的 `YYYY-MM-DD_AI每日情报.html`

## 原文中的 HTML 要求

- 信息密度高
- 编辑部情报台质感
- 深浅色自适应
- 响应式布局
- 清晰的信息层级
- Top10 事件卡片
- 评分视觉化
- 来源覆盖状态

## 原文中的完成汇报要求

- Markdown 路径
- HTML 路径
- 今日主线
- 必看 Top10 数量
- 可做内容选题数量
- 失败或缺失的数据源

## 关联页面

- [../Workflows/daily-intel-pipeline.md](../Workflows/daily-intel-pipeline.md)
- [../Skills/automation-task-spec.md](../Skills/automation-task-spec.md)
- [../Skills/html-brief-generator.md](../Skills/html-brief-generator.md)
