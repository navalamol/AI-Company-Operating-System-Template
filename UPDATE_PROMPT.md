# Update Prompt — Upgrade from Public Info to Real Internal Knowledge

## What This Is

After running SETUP_PROMPT, your operating system is populated with publicly available information. This prompt upgrades it to real internal accuracy using your company's actual documents.

Use this when you have:
- Product roadmaps or sprint plans
- Architecture Decision Records (ADRs) or engineering RFCs
- Quarterly Business Review (QBR) or strategy decks
- Engineering wiki / Confluence exports
- OKR updates more recent than what was used to generate the files
- Competitive analysis documents
- Customer research or win/loss analysis
- Onboarding guides or technical documentation

---

## The Prompt — Copy Everything Below This Line

---

I have real internal documents for **[COMPANY_NAME]** that contain more accurate information than the publicly-available version. Use them to update the AI Company Operating System at:

`[PATH_TO_YOUR_OS — e.g., D:\AI\AI_Learning_Projects\pim-company\]`

---

**Documents I'm providing:**

```
[LIST WHAT YOU HAVE — examples:]

1. Product roadmap Q3 2026 (attached PDF / pasted below)
2. Architecture Decision Record: migration to MACH (pasted below)
3. QBR deck August 2026 — executive summary (pasted below)
4. Updated OKR scores as of [DATE] (pasted below)
5. Engineering onboarding guide (link / pasted below)
6. [ADD YOURS]
```

[PASTE OR ATTACH DOCUMENT CONTENT BELOW]

---

**Instructions:**

For each document:

1. **Read it carefully.** Extract only permanent knowledge: decisions, strategic direction changes, lessons learned, architectural constraints, competitive insights, roadmap priorities.

2. **Identify which OS file(s) should be updated.** Use this mapping:
   - Strategic direction, priorities, objectives → `.product/01_CEO_DASHBOARD.md`
   - Product mission, roadmap → `.product/00_PRODUCT_VISION.md`, `.product/04_NEXT_MISSION.md`
   - Feature list, backlog → `.product/07_FEATURE_BACKLOG.md`, `.product/05_WORK_QUEUE.md`
   - Architecture choices → `.engineering/DECISIONS.md`, `.engineering/ARCHITECTURE.md`
   - Technical vocabulary → `.engineering/GLOSSARY.md`
   - Engineering lessons → `.engineering/SESSION_MEMORY.md`
   - Company principles that changed → `.company/00_COMPANY_CONSTITUTION.md`
   - Competitive position changes → `.product/00_PRODUCT_VISION.md`

3. **Update ONLY files where the document adds new knowledge.** Never update a file just because a document was provided. Only update when the document changes, corrects, or significantly enriches the existing content.

4. **Handle conflicts carefully.** If a document contradicts existing OS content:
   - State the contradiction explicitly in the updated file
   - Mark it: `*Note: This conflicts with [source]. Verified by [document name] on [date].*`
   - Ask me which version to keep if the conflict is significant

5. **Never speculate.** If a document is ambiguous about a fact, write the ambiguity into the file:
   - `*[Inferred from QBR deck — not explicitly stated. Verify with product team.]*`

6. **After completing all updates:**
   - List every file that was changed
   - For each changed file, summarize in one sentence what changed and why
   - Flag any files that should be reviewed by a human before treating as authoritative
   - Recommend any additional documents that would improve accuracy further

---

## Periodic Update Prompt (Monthly / After Major Milestones)

Use this lighter version when you just want to keep the OS current:

---

Our company objectives have been updated. Review the AI Company Operating System at `[OS_PATH]` and update only the files that have changed.

New objective scores as of [DATE]:
```
[PASTE UPDATED OBJECTIVES AND SCORES]
```

Additionally, since the last update:
- [DESCRIBE ANY MAJOR PRODUCT OR STRATEGY CHANGES]
- [DESCRIBE ANY ARCHITECTURE DECISIONS MADE]
- [DESCRIBE ANY COMPETITIVE MOVES]

Update the relevant files, then run the Strategic Review prompt to check whether the current next mission still makes sense given these changes.

---

## What to Feed It — Priority Order

If you only have time to provide one type of document, use this priority:

| Priority | Document Type | Files Updated |
|---|---|---|
| 1 | Updated OKR/objective scores | CEO Dashboard, Company Scorecard |
| 2 | Product roadmap or sprint plan | Next Mission, Feature Backlog, Work Queue |
| 3 | Architecture Decision Records | Engineering Decisions, Architecture |
| 4 | QBR or strategy deck | CEO Dashboard, Product Vision, Current State |
| 5 | Engineering wiki / Confluence | Architecture, Glossary, Session Memory |
| 6 | Competitive analysis | Product Vision, Company Constitution |
| 7 | Customer research | Product Vision, CEO Dashboard, Product Brain |

---

## The Goal

After running this prompt with good internal documents, the OS should be accurate enough that a new engineer could read the engineering files and make architecture decisions that align with what the team actually does — not just what Claude inferred from a website.

That is the bar: **good enough to onboard someone.**
