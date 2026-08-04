# Architectural Decisions

Permanent decisions. Do not re-debate. Challenge only if a constraint fundamentally changes.

*Instructions: This is the most important engineering file. Each decision should record: what was decided, why (including alternatives rejected), and the constraint it creates. Engineers should update this file as part of the PR when a significant architectural decision is made. Aim for 6–12 decisions that cover the platform's core choices.*

---

## 1. [DECISION_TITLE — e.g., "MACH Architecture — Non-Negotiable"]

**Decision:** [One sentence: what was decided.]
**Why:** [2–3 sentences: the actual reason — business and technical. What alternatives were considered and why they were rejected?]
**Constraint:** [One sentence: what engineers must not do because of this decision. This is the guardrail.]

---

## 2. [DECISION_TITLE — e.g., "Universal Data Model"]

**Decision:** [One sentence.]
**Why:** [2–3 sentences.]
**Constraint:** [One sentence.]

---

## 3. [DECISION_TITLE — e.g., "Human-in-the-Loop for Automated Actions"]

**Decision:** [One sentence.]
**Why:** [2–3 sentences: the risk model that drove this decision. What bad outcome does this prevent?]
**Constraint:** [One sentence: what can never be removed or bypassed.]

---

## 4. [DECISION_TITLE — e.g., "Customer Data Tenant Isolation"]

**Decision:** [One sentence.]
**Why:** [2–3 sentences.]
**Constraint:** [One sentence.]

---

## 5. [DECISION_TITLE — e.g., "Foundation Models Are Plug-Ins"]

**Decision:** [One sentence: LLMs/AI models are swappable infrastructure; the data/intelligence layer is permanent.]
**Why:** [2–3 sentences: why tight coupling to a specific model is dangerous.]
**Constraint:** [One sentence: what must be tested on every model upgrade.]

---

## 6. [DECISION_TITLE — e.g., "Event-Driven Cross-Module Communication"]

**Decision:** [One sentence.]
**Why:** [2–3 sentences.]
**Constraint:** [One sentence.]

---

## [REJECTED_DECISION_TITLE — e.g., "Rejected: [Alternative Architecture]"]

**Decision:** Rejected [ALTERNATIVE].
**Why:** [2–3 sentences: why the alternative was evaluated and dismissed. Record this so the same debate doesn't recur.]
**Constraint:** Revisit only if [CONDITION_THAT_WOULD_CHANGE_THIS].
