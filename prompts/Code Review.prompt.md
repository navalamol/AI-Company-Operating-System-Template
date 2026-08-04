# Code Review

Review changed files for correctness, [ARCHITECTURE_PRINCIPLE] compliance, and platform coherence.

Prioritize:
1. [ARCHITECTURE_PRINCIPLE] compliance — [what this means for this specific platform]
2. API design — [PROTOCOL] design standards, auth patterns, rate limit handling
3. [EVENT_SYSTEM] consistency — do new events follow the established naming convention?
4. [DATA_MODEL] integrity — do changes go through the [WORKFLOW_MECHANISM]? Are [AUDIT_FIELDS] populated?
5. [AI_SAFETY_CHECK — e.g., "Agent safety"] — do agent writes pass through [SAFETY_MECHANISM]?
6. [ISOLATION_CHECK — e.g., "Tenant isolation"] — no cross-[ISOLATION_UNIT] data leakage in queries, events, or caches.
7. Simplicity — prefer evolution over rewrite. If a change touches > 5 existing modules, review as architecture decision, not code review.

Only review changed files. Do not suggest refactoring untouched code unless directly related to the change.
