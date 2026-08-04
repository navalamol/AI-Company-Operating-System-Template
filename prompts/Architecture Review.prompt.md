# Architecture Review

Review proposed or existing architecture for [PRIMARY_ARCHITECTURE_PRINCIPLE] compliance and platform coherence.

Verify:
1. Is every new capability accessible via [API_TYPE — e.g., "the GraphQL Federation or REST API"]?
2. Does cross-module communication use [EVENT_SYSTEM — e.g., "EventGrid events"] (not internal service calls)?
3. Does the design reuse [CORE_DATA_MODEL] for entity representation?
4. Are [AI_COMPONENT — e.g., "Synapse agent"] decisions protected by [SAFETY_MECHANISM — e.g., "human-in-the-loop approval gates"]?
5. Is customer data strictly isolated per [ISOLATION_UNIT — e.g., "tenant"]?
6. Can this module be licensed standalone (composability check)?
7. Is there a foundation model dependency that violates [DECISION_NUMBER] (LLMs are plug-ins)?

For any [ARCHITECTURE_PRINCIPLE] violation found:
- State the violation precisely
- Recommend the compliant alternative
- Estimate the refactoring cost vs. the long-term maintenance cost of the violation

Never recommend a new [DATA_ENTITY], [EVENT_TYPE], or [API_ENDPOINT] without first checking MODULE_INDEX.md to confirm an existing one cannot be extended.
