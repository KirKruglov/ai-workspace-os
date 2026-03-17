# How It Works — AI Workspace OS

The methodology behind the system.

---

## The Core Problem

AI tools are powerful — but most people use them like a search engine:
one question, one answer, no memory, no structure.

Every session starts from zero. The agent doesn't know:
- Who you are
- What project you're on
- What was decided last week
- How you like your outputs

So you repeat yourself. You get generic outputs. You spend time editing instead of using.

---

## The Solution: Structured Context

AI Workspace OS gives your agent a persistent operating environment.

Three layers of context:

```
LAYER 1: Global (who you are)
  → about-me.md + global-rules.md
  → Loaded every session
  → Defines identity, preferences, output standards

LAYER 2: Project (what you're working on)
  → context/context.md + project-rules.md
  → Loaded per project
  → Defines goals, background, constraints, history

LAYER 3: Task (what to do now)
  → task-brief.md or session-start.md
  → Written per session
  → Defines today's specific task
```

Each layer is a markdown file you write once, then reuse.

---

## The Session Flow

```
Start session
    ↓
Paste session-start.md prompt
    ↓
Agent reads: about-me → global-rules → context → log
    ↓
Agent confirms understanding
    ↓
You describe the task (or use task-brief.md)
    ↓
Agent works
    ↓
Agent logs output in logs/log.md
    ↓
End session
```

The log becomes a searchable history of every session.
Next session, the agent reads the log and knows what was already done.

---

## Why This Works

**For non-technical users:**
No code, no APIs, no automation. Just text files and copy-paste prompts.
Works with any AI tool that accepts text input.

**For consistent output quality:**
The agent always works from the same behavioral rules.
No need to re-explain your preferences every session.

**For project continuity:**
The log + context files act as persistent memory.
Even if you switch AI tools, the context travels with you.

**For teams:**
Context files can be shared. One team → one shared `global/` folder → consistent AI behavior across the team.

---

## Design Principles

**1. Text files only.**
No databases, no special software. Everything is `.md` files you can open in any editor.

**2. Human-readable.**
Files are written to be read by both humans and AI. You can edit them manually anytime.

**3. Progressive detail.**
Start with just `about-me.md` and `global-rules.md`. Add projects and templates as needed.
The system works at any level of completeness.

**4. AI-agnostic.**
Works with Claude, ChatGPT, Gemini, or any model that accepts a text prompt.

**5. Opinionated defaults, easy to override.**
Default rules cover 80% of professional use cases.
Override anything in `project-rules.md` without touching global settings.

---

## What This Is Not

- Not an automation tool (no scripts run automatically)
- Not an integration platform (no API connections)
- Not a database (everything is plain text)
- Not a finished product (it's a framework — you customize it)
