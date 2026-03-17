# FAQ — AI Workspace OS

---

**Does this work with ChatGPT?**
Yes. Copy-paste the file contents into your ChatGPT conversation.
If you use ChatGPT Projects, you can upload files directly to the project knowledge base.

**Does this work with Claude?**
Yes. Use Claude Projects to upload your global files once.
Then paste the session-start prompt at the beginning of each conversation.

**Do I need to know how to code?**
No. Everything is plain text files (`.md`). You edit them like any document.
The only technical skill needed: copy and paste.

**How do I share this with my team?**
Put the folder in a shared drive (Google Drive, Dropbox, Notion, etc.).
Team members can copy the `global/` folder and adjust `about-me.md` for themselves.
Share a common `global/global-rules.md` to align AI behavior across the team.

**What if the AI doesn't read my files?**
Some AI tools don't support file uploads. In that case:
open the file, copy all the text, and paste it directly into your message.

**Can I use this with multiple projects at once?**
Yes. Each project has its own folder. Use a separate AI project/conversation per project,
and load the relevant context at the start of each session.

**How often should I update context.md?**
After any major decision, change in direction, or completed milestone.
Aim to keep it accurate — if it's outdated, your AI will work from wrong information.

**The agent forgets things between sessions. Is that normal?**
Yes — AI models don't have persistent memory between conversations.
That's exactly what this system solves: you re-load context at session start.
Use the session log to capture what was done so it can be reloaded next time.

**Can I add my own rules or files?**
Absolutely. The system is fully customizable.
Add files to `global/`, create new template variants, extend `project-rules.md` however you need.

**Is there a premium version?**
No. This is open source under MIT license — free to use, fork, and adapt.
