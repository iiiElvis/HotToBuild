中文 | [English](README.md)

# HotToBuild 🔥

**把最热的 AI 开源趋势，变成你今天就能动手做的项目。**

你不需要先有想法。
你不需要知道什么在流行。
只需要告诉我你感兴趣的方向——或者什么都不说。

HotToBuild 会扫描 GitHub、Hacker News 和 OSSInsight，
找到当前最热的 AI 方向，
告诉你今天可以做什么。🚀

---

## 它能做什么

GitHub Trending 告诉你什么在火。
HotToBuild 告诉你你能做什么。

给它一个方向，比如 `MCP`、`AI Agent`、`AI Skills`，或者什么都不给——它会：

- 用真实数据告诉你一个方向为什么在火
- 帮你看哪些方向还有新项目的空间
- 给你 3 个今天就能开始的具体切入点
- 推荐一个最值得做的项目

---

## 如何使用

### 方式一：作为 Claude Skill 使用（推荐）

在 Claude Code 或任何兼容 Claude Skill 的环境中安装 `hot-to-build.skill`。

### 方式二：复制系统提示词

复制 `SKILL.md` 的内容，在 Claude.ai 或通过 Anthropic API 作为系统提示词使用。

---

## 数据来源

HotToBuild 从以下平台获取实时数据：

- **GitHub Trending** — star 增长数是最直接的市场信号
- **Hacker News** — 开发者讨论热度反映真实关注度
- **OSSInsight** — 验证是方向在火还是某个人在火

---

## 输出示例

> 📍 AI Skills 方向——为什么现在值得做
>
> 基于三个平台近一个月的数据，AI Skills 是 AI 开源领域增长最快的新品类。
>
> - GitHub Trending：本月新增 +9,200 stars，vs MCP 方向 +3,800 stars
> - HN：讨论量高，多个帖子进入 Top 10
> - OSSInsight：50+ 不同作者同时在趋势榜——是方向热，不是个人热
>
> ✅ 你今天可以切入的方向：
> 1. 为内容创作者做一个 Claude Code Skill（最推荐）
> 2. 为产品经理做一个 Skill 合集
> 3. 写一份新手入门指南：如何写你的第一个 Skill

---

## 许可证

MIT
