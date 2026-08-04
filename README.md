# AI Company Operating System — Template

## What This Is

A set of markdown files that transforms Claude from a generic chatbot into a persistent AI partner with complete company context — strategy, product roadmap, engineering decisions, competitive position — loaded automatically in every conversation.

**The idea:** Instead of explaining your company every time you open a chat, Claude already knows. You ask a question. It answers from your company's perspective.

---

## The 3-Step Process

```
Step 1: Copy this template folder to a new location
        (e.g., D:\AI\AI_Learning_Projects\my-company-os\)

Step 2: Open SETUP_PROMPT.md
        Fill in [COMPANY_NAME], [COMPANY_WEBSITE], and your objectives
        Paste the prompt into Claude Code
        Claude researches the company and populates all 28+ files

Step 3: Open the generated folder in Claude Code
        Ask anything about your company
        Claude answers from your strategic context
```

That is the entire setup. 10–15 minutes for a publicly-traded or well-documented company.

---

## What's In This Folder

| File | Purpose |
|---|---|
| `DEMO_SCRIPT.md` | Coffee chat + CTO presentation script — read this first if you're presenting |
| `SETUP_PROMPT.md` | The exact prompt to generate a company-specific OS from this template |
| `UPDATE_PROMPT.md` | Prompt to upgrade the OS with real internal documents |
| `CLAUDE.md` | Template operating system entry point (auto-loaded by Claude Code) |
| `.company/` | Company principles, decision frameworks, executive council |
| `.product/` | Product vision, CEO dashboard, roadmap, feature backlog |
| `.engineering/` | Architecture, decisions, module index, glossary |
| `.reflection/` | Strategic review and escalation prompts |
| `prompts/` | Reusable slash commands for common workflows |

---

## Live Example

The Syndigo AI Company Operating System at `D:\AI\AI_Learning_Projects\pim-company\` was generated from this template in a single Claude Code session.

- Template: this folder (generic placeholders)
- Input: company name + BetterWork objective scores
- Output: 32 company-specific files, production-quality
- Time: approximately 15 minutes of prompting

See `DEMO_SCRIPT.md` for the full walkthrough including live demo prompts.

---

## How to Maintain It Over Time

- **After every major decision:** Update `.engineering/DECISIONS.md`
- **After every sprint planning:** Update `.product/04_NEXT_MISSION.md`
- **Monthly:** Run the Strategic Review prompt (`prompts/Strategic Review.prompt.md`)
- **When strategy changes:** Update `.product/01_CEO_DASHBOARD.md` and `.product/00_PRODUCT_VISION.md`
- **When you have real internal docs:** Use `UPDATE_PROMPT.md`

The system gets smarter with every update. The more accurate the files, the better Claude's answers.
