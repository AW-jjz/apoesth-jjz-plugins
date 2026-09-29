---
name: 技能示例
id: skill-context-mgmt
version: 1.0.0
author: APOESTH EXT
description: 说明 SKILL.md 的 front-matter 元数据头与正文规范，供 skill 型插件下载落盘。
---

# 使用说明

本文件是 **skill 型插件**的正文格式规范示例。安装此类插件时，前端仅拉取本文件的
文本并落盘到浏览器 IndexedDB（不执行任何可执行体），正文供 Hermes/Chat 消费。

## 元数据头（front-matter）

顶部必须使用 `---` 包裹的 YAML 风格头，字段固定为：

```yaml
name: 技能名
id: 全局唯一 id（在 manifest 中与插件条目一致）
version: 语义化版本 1.0.0
author: 作者标识
description: 一句话描述
```

## 正文

从 front-matter 之后开始为技能正文，建议以 Markdown 书写，包含：目标、流程、
约束、示例。这里仅作占位示例，无需丰富。

## 参考

- 存放位置：IndexedDB（数据库 `aposth_skill_db`，存储 `skills`）
- 本文件自身可作为 skill 安装的下载源。