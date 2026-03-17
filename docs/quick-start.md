# Quick Start — AI Workspace OS

Get up and running in 5 minutes.

---

## What This Is

AI Workspace OS is a folder system + set of templates that turns any AI chat tool
(Claude, ChatGPT, etc.) into a structured work assistant.

Instead of starting every session from scratch, you give your AI a consistent context:
who you are, how you work, what project you're on, and what was done before.

**Result:** better outputs, less repetition, faster sessions.

---

## Step 1 — Download

Click **Code → Download ZIP** on the GitHub repository page, then extract the folder.

Or if you use Git:
```bash
git clone https://github.com/[username]/ai-workspace-os.git
```

---

## Step 2 — Fill In Your Profile

Open `global/about-me.md` and fill in:
- Your name, role, and company
- Your current priorities
- How you like to communicate

Open `global/global-rules.md` and adjust:
- Language (English or Russian by default)
- Output format preferences
- Any rules you want to change

> These two files are the foundation. The better you fill them in, the better your AI will perform.

---

## Step 3 — Create Your First Project

1. Copy the folder `projects/_template/`
2. Rename it to your project name — e.g. `projects/product-launch/`
3. Open `projects/product-launch/context/context.md`
4. Fill in: project name, goals, background, constraints

---

## Step 4 — Start Your First Session

Open `templates/session-start.md`, copy the prompt, fill in the blanks, and paste it into Claude or ChatGPT.

The agent will:
1. Read your global context
2. Read your project context
3. Confirm its understanding
4. Start working

---

## Step 5 — Give It a Task

Use `templates/task-brief.md` to structure your task.
A well-written brief takes 2-3 minutes and saves 3-5 back-and-forth messages.

---

## Folder Structure at a Glance

```
ai-workspace-os/
├── global/                    ← Who you are + how the agent behaves
│   ├── about-me.md
│   └── global-rules.md
├── projects/
│   └── your-project/          ← One folder per project
│       ├── context/           ← Background, goals, rules
│       ├── input/             ← Raw materials (documents, data)
│       ├── output/            ← Final deliverables
│       └── logs/              ← Session history
├── templates/                 ← Ready-to-use prompts
│   ├── session-start.md
│   ├── task-brief.md
│   └── agent-instructions.md
└── docs/                      ← You are here
```

---

## Tips

**Keep context files short and current.**
If `context.md` is outdated, the agent will work from stale information.

**Let the agent log its work.**
At the end of each session, ask: *"Log what we did in logs/log.md"*.
This builds a history you can reference later.

**One project folder per topic.**
Don't mix unrelated work in one project folder. Create separate folders.

**Use task briefs for complex tasks.**
For simple questions, you don't need a brief. For anything that takes more than one message — use `task-brief.md`.

---

## Troubleshooting

**The agent ignores my context files.**
→ Make sure you're pasting the file content directly into the chat, not just mentioning the filename.
Some AI tools don't have file access — paste content manually.

**Output quality is low.**
→ Check `global/global-rules.md` — add more specific format requirements.
→ Fill in `global/about-me.md` more thoroughly.

**I don't know how to structure a new project.**
→ Start by filling in only `context.md` in the project folder. That's enough to begin.

---

## Next Steps

- Read `docs/how-it-works.md` for the methodology behind this system
- Check `docs/faq.md` for common questions
- Star ⭐ the repo to get updates
