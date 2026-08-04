# Demo Script — AI Company Operating System
## For Coffee Chat Sessions & CTO Presentation

*Presenter: Amol Naval | Duration: 15–20 minutes | Audience: Any Syndigo employee or executive*

---

## Before You Start

Have these open and ready:
1. This template folder (`D:\AI\AI_Learning_Projects\template\`) — the blank canvas
2. `SETUP_PROMPT.md` — the magic prompt
3. The generated Syndigo OS (`D:\AI\AI_Learning_Projects\pim-company\`) — the result
4. Claude Code open on the `pim-company` folder

---

## Part 1 — The Opening Hook (2 minutes)

**Say this:**

> "Let me show you the most useful thing I've done with Claude this year — and it has nothing to do with generating code.
>
> Every time most people open a chat with Claude, they start from scratch. They explain what their company does, what product they're building, what the constraints are. Five minutes of setup before you get a useful answer.
>
> What if Claude already knew all of that? What if, the moment you opened a conversation, it already knew our company objectives, our product roadmap, our architectural decisions, and our competitive position — and every answer it gave you was grounded in that context?
>
> That's what I'm going to show you."

**Show:** The `pim-company` folder structure in a file explorer. 32 files. Nothing special looking.

> "This is an AI Company Operating System. 32 markdown files. Each one is a permanent record of something important about Syndigo — strategy, product state, engineering decisions. Claude Code reads them automatically before every conversation."

---

## Part 2 — The Problem It Solves (2 minutes)

**Say this:**

> "Here's the real problem. We have institutional knowledge scattered everywhere — in people's heads, in Confluence pages nobody reads, in Slack messages that scroll away, in a PowerPoint from last quarter that's already out of date.
>
> A new engineer joins. They spend three weeks trying to understand why we made certain architecture decisions. A product manager needs to explain our competitive position to a new stakeholder. An executive wants a strategic review before a board meeting.
>
> In every case, the knowledge exists — but the cost of accessing it is too high.
>
> This system makes that knowledge free to access. Instantaneous. Always current."

---

## Part 3 — Show the Template (2 minutes)

**Show:** Open `D:\AI\AI_Learning_Projects\template\`

> "Here is the raw template. Before I populated it with any Syndigo information, this is what it looked like."

**Open:** `.product/01_CEO_DASHBOARD.md` from the template folder

> "See these placeholders — `[COMPANY_NAME]`, `[OBJECTIVE_1]`, `[NORTH_STAR_METRIC]`? This is the blank canvas. The structure is universal. The content is yours to fill in."

**Say:**

> "The structure never changes. The thinking framework, the conversation modes, the context loading strategy — that's the operating system. The company-specific content is the data you load into it."

---

## Part 4 — The Magic Prompt (2 minutes)

**Show:** Open `SETUP_PROMPT.md`

> "Here is the exact prompt I used to go from this blank template to a fully populated Syndigo operating system. Three steps.
>
> Step 1: Tell Claude to research the company website.
> Step 2: Paste in the BetterWork objective scores.
> Step 3: Point it at the template and the output location.
>
> That's it. One prompt. Claude does the rest."

**Emphasize:**

> "I gave it the BetterWork objective scores directly — those are our real numbers. Accelerate Product Innovation at 8%. That's our real gap. Claude didn't make that up. It uses exactly what you give it.
>
> For publicly available information — what Syndigo does, what Synapse is, what our competitive position is — Claude searched the web. For internal information — your real strategy, your actual architectural decisions — that's where UPDATE_PROMPT comes in."

---

## Part 5 — Live Demo by Role (8 minutes)

**Say:** "Let me show you what this looks like for four different people at Syndigo."

---

### Demo 1 — For a Developer (2 min)

**In Claude Code (pim-company folder), type:**

```
I'm designing a new API endpoint that lets external systems subscribe to 
Content Readiness Score changes for a specific brand. What architectural 
decisions should I follow, and what existing patterns should I reuse?
```

**Point out in the response:**
- References EventGrid eventing (from DECISIONS.md)
- References the Thing Model entity structure (from ARCHITECTURE.md)
- References the existing OAuth2 pattern (from engineering docs)
- Says "don't build a new event type — use entity-changed with syndication-status" — a real decision

> "A junior engineer got an answer in 30 seconds that would have taken them an afternoon of Confluence searching. And it's correct — because those decisions are in the engineering files."

---

### Demo 2 — For a Product Owner (2 min)

**Type:**

```
Run a Strategic Review. Our Innovation objective is at 8%. We just shipped 
Synapse. Does our current roadmap make sense, or are we missing the highest 
ROI next step?
```

**Point out in the response:**
- Reads the actual objective scores from CEO_DASHBOARD.md
- References the current mission from NEXT_MISSION.md
- Gives a recommendation grounded in real company context
- Mentions specific Syndigo products and decisions

> "This is a product review that would normally take a 2-hour meeting. In 30 seconds, grounded in our actual strategy."

---

### Demo 3 — For an Executive (2 min)

**Type:**

```
Our Integrate Companies objective is at 14%. We acquired 1WorldSync in 
September 2025. Nine months later, platform integration is still incomplete. 
What is the highest ROI decision we can make this quarter to advance this 
objective before year-end?
```

**Point out in the response:**
- Knows the acquisition context (1WorldSync, Sept 2025)
- Knows the platform architecture (dual data pools as the problem)
- Gives a specific recommendation with rationale
- References the network moat principle from Company Constitution

> "This is an executive briefing answer. Not a generic 'integrate faster' suggestion — a specific recommendation grounded in our architecture and competitive position."

---

### Demo 4 — For a New Employee (2 min)

**Type:**

```
I joined Syndigo last week as a backend engineer. I've heard about the 
Thing Model and Synapse but I don't understand how they connect. Can you 
explain the platform's core architecture in a way that helps me understand 
what I'm building and why the decisions were made this way?
```

**Point out in the response:**
- Explains Thing Model from ARCHITECTURE.md
- Connects it to Synapse from DECISIONS.md
- Explains WHY MACH was chosen
- Uses Syndigo's actual vocabulary (GDSN, GLN, golden record)

> "This is three weeks of onboarding in one conversation. The architectural decisions, the vocabulary, the 'why' behind every choice — it's all here."

---

## Part 6 — How to Make It Yours (3 minutes)

**Show the three levels:**

### Level 1 — Public Information (What was just demoed)
> "What you saw is built entirely from publicly available information. I gave Claude our BetterWork objective scores, pointed it at Syndigo's website, and it populated 32 files. This takes 15 minutes for any company."

### Level 2 — Real Internal Documents
> "For actual accuracy, you feed it real documents. Open `UPDATE_PROMPT.md`."

**Show UPDATE_PROMPT.md briefly:**

> "Give Claude your product roadmap, your ADRs, your QBR deck, your architecture wiki. This prompt tells Claude: 'Read these, extract permanent knowledge, update only the files where something genuinely changed.' The files become more accurate with every document you feed it."

### Level 3 — Continuous Updates
> "The system stays current because the team updates it. Engineers update DECISIONS.md when they make an architecture decision — as part of the PR. Product owners update NEXT_MISSION.md at sprint planning. The Strategic Review prompt runs monthly and tells you which files need updating.
>
> This is not a one-time setup. It is a living document system with an AI interface."

---

## Part 7 — For the CTO (Executive Framing) (3 minutes)

*Use this section when presenting to leadership.*

**Say:**

> "Here is why this matters at the company level — not just the individual level.

> **Alignment tax.** Every time an engineer makes a decision that doesn't align with our architecture principles, we pay a cost — in rework, in tech debt, in future constraints. This system reduces the alignment tax because the principles are always accessible and Claude applies them automatically.

> **Onboarding acceleration.** New hires reaching productive contribution in weeks instead of months. Not because we wrote better documentation — because the documentation is now conversational.

> **Decision quality at scale.** When a team of 50 engineers each make 10 decisions per day, the quality of those decisions is bounded by how much context each engineer carries. This system gives every engineer access to the full strategic and architectural context instantly.

> **The git repo integration.** This operating system lives in a git repo. It's versioned. It's reviewed. When an architectural decision is made in a PR, the PR description links to the DECISIONS.md update. The engineering record becomes part of the engineering process, not a separate documentation effort.

> **What it is not.** It is not a chatbot. It is not a search engine. It is institutional memory with an AI interface. The knowledge belongs to Syndigo. Claude is the interface to access it."

**Close with:**

> "I built this for my own product first. Then I realized it generalized. The template takes 15 minutes to populate for any team. I wanted to share it because I think it's the highest-leverage thing we can do with AI that most teams aren't doing yet."

---

## Frequently Asked Questions

**Q: Is this safe? Are we sending company secrets to Anthropic?**
A: Claude Code runs locally. The markdown files never leave your machine unless you explicitly share them. No data is sent to train Claude's models. This is the same as having a conversation with Claude — only the messages you type are sent.

**Q: What if the information in the files is wrong?**
A: The files are as accurate as the information you put in them. Level 1 (public info) is a starting point. Level 2 (real docs) is the accuracy upgrade. The UPDATE_PROMPT explicitly tells Claude to flag ambiguities rather than guess.

**Q: Does this work for teams?**
A: Yes. The folder lives in a shared git repo. Everyone on the team has the same context. Updates are PRs. The system gets better as the team contributes.

**Q: What about confidential product roadmaps?**
A: The folder is stored wherever you store confidential files. If it's in a private git repo with proper access controls, it's as confidential as any internal document. Claude Code does not transmit the file contents beyond the active conversation.

**Q: How long does it take to set up?**
A: Level 1 (public info): 15 minutes. Level 2 (with real docs): 1–2 hours for a thorough first pass. Ongoing updates: 15–30 minutes per sprint as a habit.

---

## Key Numbers for Executives

- **15 minutes** to bootstrap from template
- **32 files** covering company, product, engineering, and reflection
- **1 prompt** to regenerate from updated documents  
- **0 code** — this is documentation with an AI interface
- **∞ reusable** — the template works for any company, any team, any product
