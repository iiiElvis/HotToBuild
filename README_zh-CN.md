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

用户输入：`MCP`

> 📍 MCP 生态——为什么现在值得做
>
> 根据 GitHub Trending、Hacker News、OSSInsight 近一个月数据，MCP 是当前 AI 开源领域最大的蓝海方向。
>
> - GitHub Trending：modelcontextprotocol/servers 达到 86K stars，Playwright MCP（微软）30K stars，过去一个月使用量增长 35%
> - HN：多个帖子登上首页，讨论集中在 MCP 安全、企业落地、"MCP server 淘金热"
> - OSSInsight：15,926 个 mcp-server 标签仓库，SDK 月下载量 9700 万次，数十个不同作者同时在趋势榜——是方向热，不是个人热
>
> 已有 14,000+ MCP server，但大部分是简单 API 包装。高价值空白还很多。
>
> 🚫 现在不值得做的
>
> ① 再做一个 ChatGPT/Slack/GitHub 的 MCP wrapper → 已有几百个，没有差异化空间
>
> ✅ 你现在可以切入的方向
>
> ① **MCP 安全扫描器**（最推荐）
> 已发现 492 个 MCP server 零认证暴露在公网。做一个扫描 MCP 配置安全问题的工具。
> 为什么值得做：每个用 MCP 的企业都需要，目前没有好的开源方案。
>
> ② **MCP server 测试框架**
> 类似 pytest 的工具——写测试、跑在任意 server 上、输出兼容性报告。
> 为什么值得做：14,000 个 server 但没有标准测试方式。
>
> ③ **垂直领域 MCP server 套件**（如数据工程方向）
> 打包 5-10 个 MCP server 覆盖一个完整工作流：dbt + Snowflake + Airflow + Great Expectations。
> 为什么值得做：团队在用 MCP 但一个个接 server 很痛苦。
>
> 🎯 最推荐你做第一个：MCP 安全扫描器
>
> 一句话："npm audit，但给你的 MCP server 用。"
>
> → 只做：扫描配置、检测零认证端点、标记过度授权的工具
> → 不做：不做 MCP 代理或网关
>
> 为什么现在进入还来得及：
> → MCP 使用量上个月增长 35%，安全工具完全没跟上
> → Anthropic 已把 MCP 捐给 Linux 基金会，企业采用在加速，安全是硬需求

---

## 许可证

MIT
