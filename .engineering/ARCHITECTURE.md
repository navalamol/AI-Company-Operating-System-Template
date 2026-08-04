# Architecture Guide

*Last updated: [DATE]*

*Instructions: Describe the actual architecture, not aspirational architecture. Include a simple diagram if it helps. Cover the data model, API layer, event system, and any AI/automation components. This is what Claude reads before making architectural recommendations.*

---

## Platform Overview

[COMPANY_NAME]'s [PRODUCT_NAME] is a [ARCHITECTURE_TYPE — e.g., "MACH-architecture SaaS platform on Azure" / "event-driven microservices platform" / "local-first Electron application"].

```
[HIGH_LEVEL_ARCHITECTURE_DIAGRAM — ASCII art or mermaid diagram]

Example:
User Interface (Headless)
        ↓
API Gateway ([PROTOCOL — e.g., GraphQL Federation / REST])
        ↓
┌─────────┬─────────┬─────────┐
│ [SVC_1] │ [SVC_2] │ [SVC_3] │
└─────────┴─────────┴─────────┘
        ↓
[EVENT_BUS — e.g., Azure EventGrid / Kafka / SQS]
        ↓
[DATA_LAYER — e.g., Thing Model / PostgreSQL / Vector Store]
```

---

## Core Data Model — [DATA_MODEL_NAME — e.g., "The Thing Model" / "The Entity Graph"]

[PARAGRAPH: Describe the core data model. What is the universal abstraction? What are the key entities? What are the key relationships? Why was this model chosen over alternatives?]

Key concepts:
- **[CONCEPT_1]**: [definition]
- **[CONCEPT_2]**: [definition]
- **[CONCEPT_3]**: [definition]

---

## API Layer

[PARAGRAPH: Describe the API architecture. REST? GraphQL? gRPC? Auth model? Rate limits? How are modules exposed?]

Key details:
- Auth: [AUTH_MODEL — e.g., "OAuth2 client-credentials per tenant"]
- Rate limits: [RATE_LIMITS]
- [OTHER_API_DETAIL]

---

## Event System

[PARAGRAPH: How do components communicate asynchronously? What are the key event types? What triggers them?]

Key event types:
- `[EVENT_1]` — [what triggers it, what subscribes to it]
- `[EVENT_2]` — [what triggers it]
- `[EVENT_3]` — [what triggers it]

---

## [AI/AUTOMATION_COMPONENT — if applicable]

[PARAGRAPH: Describe the AI or automation layer. How are agents orchestrated? What do they have access to? What are the safety constraints?]

---

## Extend Existing Modules — Never Rewrite

[PARAGRAPH: What is the core principle for making changes? What should engineers check before adding something new?]
