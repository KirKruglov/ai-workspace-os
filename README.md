# AI Workspace OS

**A structured operating system for non-technical professionals working with AI agents.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/KirKruglov/ai-workspace-os?style=social)](https://github.com/[username]/ai-workspace-os)


Works with **Claude · ChatGPT · Gemini · any LLM chat tool**

---

## The Problem

You use AI every day. But every session starts from zero.

The agent doesn't know who you are, what project you're on, what was decided last week,
or how you like your outputs formatted.

You repeat yourself. You get generic results. You spend time editing instead of using.

---

## The Solution

AI Workspace OS is a folder system + set of templates that gives your AI agent
a persistent operating environment — without code, APIs, or automation.

Just text files. Copy, fill in, paste. That's it.

```
global/
  about-me.md           ← who you are, your role, your preferences
  global-rules.md       ← how the agent should behave and format output

projects/
  your-project/
    context/context.md  ← project background, goals, constraints
    logs/log.md         ← session history (agent writes this automatically)
    input/              ← raw materials
    output/             ← final deliverables

templates/
  session-start.md      ← paste this at the start of every AI session
  task-brief.md         ← structure your tasks for better output
  agent-instructions.md ← master prompt for any AI tool
```

---

## How It Works

```
1. Fill in global/about-me.md       → tell the AI who you are (once)
2. Fill in global/global-rules.md   → set output standards (once)
3. Create a project folder          → add context per project
4. Start session with session-start.md → agent reads everything, ready to work
5. Give tasks with task-brief.md    → structured input = structured output
6. Agent logs the session           → history builds automatically
```

Every new session loads your context. No repetition. No reset.

---

## Quick Start

**1. Download**

```bash
git clone https://github.com/[username]/ai-workspace-os.git
```
Or: **Code → Download ZIP**

**2. Fill in your profile**

Open `global/about-me.md` and `global/global-rules.md` — edit the `[ ]` fields.

**3. Start a session**

Copy `templates/session-start.md`, fill in your project name and today's task, paste into Claude or ChatGPT.

**→ Full guide:** [docs/quick-start.md](docs/quick-start.md)

---

## Who Is This For

| If you are... | AI Workspace OS helps you... |
|---|---|
| Product Manager | run structured AI-assisted research, specs, and reviews |
| Marketer | maintain consistent brand voice and campaign context |
| Analyst | keep project context and session history in one place |
| Operations Manager | standardize how your team uses AI tools |
| Founder / Executive | delegate analytical and writing tasks with clear context |

No coding required. If you can edit a text file, you can use this.

---

## What's Included

| File | What it does |
|---|---|
| `global/global-rules.md` | Rules for how your AI agent behaves |
| `global/about-me.md` | Your profile, role, priorities, preferences |
| `projects/_template/` | Full project folder template — copy for each project |
| `templates/session-start.md` | Startup prompt for every AI session |
| `templates/task-brief.md` | Task assignment template |
| `templates/agent-instructions.md` | Master agent prompt + lightweight variants |
| `docs/quick-start.md` | 5-minute setup guide |
| `docs/how-it-works.md` | Methodology explained |
| `docs/faq.md` | Common questions |

---

## Why This Works

**Persistent context** — your agent always knows who you are and what you're working on.

**Structured output** — consistent rules = consistent formatting, every session.

**Session memory** — the agent logs its work. Next session, it reads the log. No amnesia.

**Tool-agnostic** — works with any AI that takes a text prompt.

**No lock-in** — plain `.md` files. Edit in any text editor. No special software required.

---

## Star History

If this is useful, ⭐ star the repo — it helps others find it.

---

## License

MIT — free to use, fork, and adapt. See [LICENSE](LICENSE).

---
