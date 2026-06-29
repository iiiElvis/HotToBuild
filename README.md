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

> 📍 AI Skills direction — why it's worth building now
>
> Based on data from 3 platforms over the past month, AI Skills is the fastest-growing new category in the AI open source space.
>
> - GitHub Trending: +9,200 stars this month vs MCP direction +3,800 stars
> - HN: High discussion volume, multiple threads in top 10
> - OSSInsight: 50+ different authors trending simultaneously — direction is hot, not one person
>
> ✅ Entry points you can build today:
> 1. A Claude Code Skill for content creators (most recommended)
> 2. A Skill pack for product managers
> 3. A beginner's guide to writing your first Skill

---

## License

MIT
