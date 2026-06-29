中文 | [English](README.md)

# HotToBuild 🔥

**在 GitHub 上找到最热的 AI 方向，搞清楚你今天能做什么。**

你不需要先有想法。
你不需要知道什么在流行。
只需要告诉它你感兴趣的方向——或者什么都不说。

HotToBuild 会扫描 GitHub Trending、Hacker News 和 OSSInsight，
找到当前增长最快的 AI 开源方向，
给你具体的项目切入点，今天就能动手。🚀

---

## 它能做什么

GitHub Trending 告诉你什么在火。
HotToBuild 告诉你你能做什么。

给它一个方向，比如 `MCP`、`AI Agent`、`AI Skills`，或者什么都不给——它会：

- 用三个平台的真实数据告诉你一个方向为什么在火
- 帮你看哪些方向还有新项目的空间
- 给你 3 个今天就能开始的具体切入点
- 推荐一个最值得做的项目

---

## 如何安装

### 方式一：作为 Claude Code Skill 安装（推荐）

1. Clone 本仓库或下载 `hot-to-build.skill` 文件
2. 解压后将文件夹放到 `~/.claude/skills/` 目录下（全局生效）或项目根目录的 `.claude/skills/` 下（仅该项目生效）
3. 确保文件夹中包含 `SKILL.md` 文件
4. 在 Claude Code 中输入 `/hot-to-build` 即可使用

```bash
# 快速安装
git clone git@github.com:iiiElvis/HotToBuild.git
mkdir -p ~/.claude/skills/hot-to-build
cp HotToBuild/SKILL.md ~/.claude/skills/hot-to-build/
```

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
