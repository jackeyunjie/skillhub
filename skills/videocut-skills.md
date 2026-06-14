# videocut-skills

## 来源

原文中明确点名并给出 GitHub 安装方式的剪口播 skill。

## 安装方式

原文中的安装命令：

```text
帮我安装：https://github.com/Backtthefuture/videocut-skills
```

## 使用方式

原文中的使用示例：

```text
Videocut：剪口播 /Users/superhuang/Documents/Screen Studio Presets/Codex自动剪辑.mp4
```

## 它在原文中的职责

1. 识别废话、停顿、重复
2. 自动剪掉这些内容
3. 基于剪后音频重新生成字幕
4. 做文字校对，修正常见错词

## 原文中的输出

- 成片：`Codex自动剪辑_auto_cut.mp4`
- 最终字幕：`Codex自动剪辑_auto_cut_final.srt`

## 原文中的校验标准

- SRT 结构通过
- 字幕条数可校验
- 时间戳未改坏
- 常见错词扫描通过

## 原文中的定位

- 不是替代最后人工精修
- 是先完成最耗时的粗剪
- 后续仍可继续导入剪映做少量修改

## 关联页面

- [../Workflows/video-editing-pipeline.md](../Workflows/video-editing-pipeline.md)
- [../Agents/content-agent.md](../Agents/content-agent.md)
