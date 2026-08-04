# Setup Prompt — Generate a Company Operating System

## What This Is

This is the exact prompt used to generate the Syndigo AI Company Operating System from the raw template. Copy it, fill in the `[BRACKETS]`, paste it into Claude Code, and Claude will generate a fully populated operating system for your company.

**Requirements:**
- Claude Code installed and open in the template folder
- Internet access (Claude will research the company)
- Your company's objective/OKR scores (from BetterWork, Lattice, Workday, or whatever your team uses)

**Time:** 10–20 minutes depending on how much public information exists about the company.

---

## The Prompt — Copy Everything Below This Line

---

I want to create an AI Company Operating System for **[COMPANY_NAME]**.

This is a set of markdown files that gives Claude complete company context so it can act as a persistent AI partner — answering questions about strategy, product, architecture, and competitive position with the accuracy of someone who has worked here for years.

---

**STEP 1 — Research the company**

Search the web for **[COMPANY_WEBSITE]** and gather:
- What the company does (product or service, in plain language)
- Who their customers are (primary and secondary segments)
- What their competitive moat is (why customers stay, why competitors can't easily copy)
- What their core technology stack or platform concepts are
- Recent strategic moves (acquisitions, product launches, pivots in the last 2 years)
- Competitive landscape (top 3–5 competitors and how this company differentiates)
- Company size, funding stage, or revenue range (if publicly available)
- Any industry-specific terminology or vocabulary that engineering and product teams use

---

**STEP 2 — Company objectives (paste your real scores)**

These are our current company objectives and progress scores from **[PERFORMANCE_SYSTEM — e.g., BetterWork / Lattice / Workday / OKR tracker]** as of **[DATE]**:

```
[PASTE YOUR OBJECTIVES AND SCORES HERE — example format:]

- Objective 1: [Name]: [Score]%
- Objective 2: [Name]: [Score]%
- Objective 3: [Name]: [Score]%
- Objective 4: [Name]: [Score]%
- Objective 5: [Name]: [Score]%
- Objective 6: [Name]: [Score]%
```

---

**STEP 3 — Generate the operating system**

Using the raw template at:
`D:\AI\AI_Learning_Projects\template\`

Create a complete AI Company Operating System at:
`D:\AI\AI_Learning_Projects\[COMPANY_FOLDER_NAME]\`

(Create the target folder if it doesn't exist.)

Replace every `[PLACEHOLDER]` in the template with company-specific, accurate content. Follow these rules:

**For `.company/` files:**
- Encode the company's real competitive principles — not generic startup advice
- The Company Constitution must reflect what actually makes this company different
- The Executive Council perspectives must be grounded in the company's real two-sided dynamics (brands vs. retailers, brands vs. consumers, enterprise vs. SMB — whatever applies)
- The Kill List must name real anti-patterns specific to this industry

**For `.product/` files:**
- CEO Dashboard: use the exact objective scores from Step 2 — do not round or paraphrase
- Product Vision: use the researched roadmap, competitive position, and north star
- Current State: list all known shipped capabilities based on research
- Next Mission: identify what the company appears to be building next based on public signals
- Feature Backlog: organize known and logical next features by priority

**For `.engineering/` files:**
- Architecture: describe the known or inferred technical architecture
- Decisions: encode the key architectural decisions the company has made (inferred from stack, job postings, documentation, engineering blog posts)
- Glossary: define every domain-specific term with precision
- Session Memory: encode 3–5 engineering lessons specific to this platform type

**Quality rules:**
- No generic filler. Every sentence must be company-specific.
- If information is inferred rather than confirmed, note it as "inferred from [source]"
- The files must be useful enough that an employee reading them learns something real
- Do not copy-paste marketing language — synthesize it into operational truth

**Output:** 28+ markdown files, production-quality, ready to open in Claude Code.

---

## Real Example — How This Generated the Syndigo OS

This exact prompt (with Syndigo filled in) generated the 32-file operating system at `D:\AI\AI_Learning_Projects\pim-company\`. The only inputs were:

1. Company: Syndigo
2. Website: https://syndigo.com
3. BetterWork objectives:
   - Accelerate Product Innovation: 8%
   - Drive Operational Excellence: 28%
   - Optimize the Customer Experience: 19%
   - High-Performance Sales Engine: 31%
   - Strengthen Organization Health: 66%
   - Successfully Integrate Companies: 14%
4. Template path: this folder

Claude researched Syndigo's platform (PIM, MDM, Synapse, 1WorldSync acquisition), populated all placeholders with accurate content, and created files useful enough to use as onboarding material for real Syndigo engineers.

---

## After Generation — Accuracy Upgrade

The generated files are based on public information. For real accuracy, use `UPDATE_PROMPT.md` to feed in internal documents:
- Product roadmap
- Architecture decision records (ADRs)
- Quarterly business review decks
- Engineering wiki or Confluence pages
- Org chart

See `UPDATE_PROMPT.md` for the exact prompt.
