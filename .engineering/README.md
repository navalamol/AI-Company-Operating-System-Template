# Engineering Knowledge

## Purpose

This folder contains implementation knowledge for [COMPANY_NAME]'s [PRODUCT_NAME] platform.

These documents help engineers and AI understand **how the platform is built**, not **what the company should build**.

Product strategy belongs in `.product`.

Company principles belong in `.company`.

This folder is implementation-focused.

---

## Reading Order

Read only what is needed.

1. MODULE_INDEX.md — find where things live in the platform
2. ARCHITECTURE.md — understand system design before changing it
3. DECISIONS.md — understand permanent decisions before challenging them
4. SESSION_MEMORY.md — apply lessons before repeating mistakes
5. GLOSSARY.md — verify you are using the right domain vocabulary

---

## Folder Contents

### MODULE_INDEX.md
Quick navigation to major capability areas. Read before exploring the codebase.

### ARCHITECTURE.md
Complete platform architecture. Contains: [LIST_KEY_ARCHITECTURE_SECTIONS — e.g., "data model, API layer, event system, AI orchestration, deployment architecture"].

### DECISIONS.md
Permanent architectural decisions. Records why decisions were made, alternatives rejected, and constraints that must not be violated. Read before changing architecture.

### SESSION_MEMORY.md
Permanent engineering learnings — lessons, proven patterns, anti-patterns, surprising discoveries. Never use as a conversation log.

### GLOSSARY.md
Definitions for every domain term. [COMPANY_NAME]'s domain vocabulary is precise — understand the terms before using them.

---

## Engineering Principles

- [PRINCIPLE_1 — e.g., "MACH-first: every capability is API-accessible, headless, and cloud-native by default."]
- Prefer evolution over rewrites.
- Reuse [CORE_COMPONENTS] before designing new abstractions.
- Keep the architecture coherent and composable.
- [SAFETY_PRINCIPLE — e.g., "Human-in-the-loop for every agent decision that affects external systems."]
- Foundation models will change; [PERMANENT_ASSET] is permanent.

---

## Rule

Implementation should follow product strategy.

Architecture exists to support the platform.

The platform should never be constrained by accidental implementation details.
