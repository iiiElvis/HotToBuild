[中文版](README_zh-CN.md) | English

# HotToBuild 🔥

**Find the hottest AI directions on GitHub and figure out what you can build today.**

You don't need an idea to start.
You don't need to know what's trending.
Just tell it what you're interested in — or nothing at all.

HotToBuild scans GitHub Trending, Hacker News, and OSSInsight
to find which AI directions are growing fastest right now,
and gives you specific open-source project ideas you can start today. 🚀

---

## What it does

GitHub Trending shows you what is hot.
HotToBuild shows you what you can build.

Give it a direction like `MCP`, `AI Agent`, `AI Skills`, or nothing at all — and it will:

- Tell you why a direction is trending (with real data from 3 platforms)
- Show you which directions still have room for new projects
- Give you 3 specific entry points you can start today
- Recommend the #1 project worth building right now

---

## How to install

### Option 1: As a Claude Code Skill (recommended)

1. Clone this repo or download the `hot-to-build.skill` file
2. Unzip and place the folder under `~/.claude/skills/` (global) or `your-project/.claude/skills/` (project-only)
3. Make sure the folder contains `SKILL.md`
4. In Claude Code, type `/hot-to-build` to use it

```bash
# Quick install
git clone git@github.com:iiiElvis/HotToBuild.git
mkdir -p ~/.claude/skills/hot-to-build
cp HotToBuild/SKILL.md ~/.claude/skills/hot-to-build/
```

### Option 2: Copy the System Prompt

Copy the contents of `SKILL.md` and use it as a system prompt in Claude.ai or via the Anthropic API.

---

## Data sources

HotToBuild pulls real-time data from:

- **GitHub Trending** — star growth is the most direct market signal
- **Hacker News** — developer discussion reflects real interest
- **OSSInsight** — verifies whether a direction is broadly hot or driven by one author

---

## Example output

User input: `MCP`

> 📍 MCP ecosystem — why it's worth building now
>
> Based on GitHub Trending, Hacker News, and OSSInsight data from the past month, MCP is the most "blue ocean" direction in AI open source right now.
>
> - GitHub Trending: modelcontextprotocol/servers hit 86K stars, Playwright MCP (Microsoft) 30K stars, 35% usage growth in the past month alone
> - HN: Multiple front-page threads on MCP security, enterprise adoption, and "the MCP server gold rush"
> - OSSInsight: 15,926 repos tagged mcp-server, 97M monthly SDK downloads, dozens of different authors trending — this is a direction, not one person
>
> 14,000+ MCP servers exist, but most are simple API wrappers. High-value gaps are wide open.
>
> 🚫 Not worth building now
>
> ① Yet another ChatGPT/Slack/GitHub wrapper MCP server → hundreds already exist, zero differentiation
>
> ✅ Entry points you can build today
>
> ① **MCP security scanner** (most recommended)
> 492 MCP servers were found exposed with zero auth. Build a tool that scans MCP server configs for security issues.
> Why now: every enterprise adopting MCP needs this, nobody has built a good open-source one yet.
>
> ② **MCP server testing framework**
> A pytest-like tool for MCP servers — write tests, run them against any server, get a compatibility report.
> Why now: 14,000 servers but no standard way to test them.
>
> ③ **Domain-specific MCP server pack** (e.g., for data engineering)
> Bundle 5-10 MCP servers for a specific workflow: dbt + Snowflake + Airflow + Great Expectations.
> Why now: teams are adopting MCP but wiring up servers one by one is painful.
>
> 🎯 #1 recommendation: MCP security scanner
>
> One sentence: "npm audit, but for your MCP servers."
>
> → Build: scan configs, detect zero-auth endpoints, flag over-permissioned tools
> → Skip: don't build a full MCP proxy or gateway
>
> Why you're not too late:
> → MCP adoption grew 35% last month — security tooling hasn't caught up
> → Anthropic donated MCP to Linux Foundation — enterprise adoption is accelerating, security becomes a hard requirement

---

## License

MIT
