# Session Start Prompt

> **How to use:**
> Copy and paste this prompt at the beginning of every AI session.
> Fill in the `[ ]` fields before sending.
> The agent will load your context and be ready to work.

---

## Prompt (copy this)

```
You are my strategic AI assistant. Before we start, read the following files in order:

1. global/about-me.md        — who I am and my work context
2. global/global-rules.md    — how you should behave and format output
3. projects/[PROJECT]/context/context.md    — current project context
4. projects/[PROJECT]/logs/log.md           — what was done previously

Today's date: [YYYY-MM-DD]

---

Today's task:
[Describe what you want to accomplish in this session — 1-3 sentences]

---

Constraints:
- [Any time limits, format requirements, or things to avoid]
- [Or write "none" if no constraints]

---

Output format:
- [What should the deliverable look like: document, table, brief, analysis, etc.]
- [Approximate length or level of detail]

Confirm you've read the files and state your understanding of the task before starting.
```

---

## Example (filled in)

```
You are my strategic AI assistant. Before we start, read the following files in order:

1. global/about-me.md
2. global/global-rules.md
3. projects/product-launch/context/context.md
4. projects/product-launch/logs/log.md

Today's date: 2026-03-11

---

Today's task:
Prepare a competitive analysis for our Q2 product launch. Focus on 3 direct competitors
and identify our top 2 differentiators.

---

Constraints:
- Output should be suitable for a board presentation
- No more than 2 pages

---

Output format:
- Structured .md document
- Table: competitor comparison matrix
- Bullet list: our differentiators with supporting evidence

Confirm you've read the files and state your understanding of the task before starting.
```
