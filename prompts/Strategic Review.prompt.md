# Strategic Review

Trigger this after every major product milestone, before starting any new multi-week mission, or at minimum monthly.

## Context Loading

Read in this order before answering anything:

1. `.company/00_COMPANY_CONSTITUTION.md`
2. `.company/02_EXECUTIVE_COUNCIL.md`
3. `.product/00_PRODUCT_VISION.md`
4. `.product/01_CEO_DASHBOARD.md`
5. `.product/04_NEXT_MISSION.md`
6. `.product/07_FEATURE_BACKLOG.md`
7. `.product/08_WEEKLY_REVIEW.md`
8. `.product/09_COMPANY_SCORECARD.md`

---

## Review Questions

Answer ALL of the following from the Executive Council perspective. Do not ask the user to answer these — you answer them with a recommendation for each.

1. **Objective alignment:** Which company objective has the lowest score? Does the current next mission directly advance it? If not, what mission would?

2. **[CUSTOMER_BALANCE_CHECK — e.g., "Two-sided network check"]:** Does the current mission improve outcomes for [CUSTOMER_SEGMENT_A] AND [CUSTOMER_SEGMENT_B]? If only one side, is that intentional?

3. **Feature bloat check:** Are we building platform capabilities or point features? List any queued work that does not compound [PLATFORM_ASSET] or advance a company objective.

4. **Highest ROI next step:** Given the current objective scores, what is the single highest ROI next initiative? Is it what's currently Active?

5. **Roadmap change:** Should the roadmap change? If yes, state specifically what moves, what gets dropped, and what the new sequence is.

6. **[PLATFORM_HEALTH_CHECK — e.g., "Network strengthening"]:** Does the current mission increase [METRIC_1], [METRIC_2], or [METRIC_3]? If none, reconsider.

7. **Document updates:** Which documents need to be updated based on this review? List only documents where something has changed.

---

## Output Format

- Answer each question directly. Give a recommendation — not options.
- Flag any misalignment between CEO Dashboard objective scores and the Active mission.
- End with: recommended document changes (if any) and ask for approval before writing them.
- Keep the entire review under 700 words unless the roadmap change is significant.

---

## When to Skip

Skip if no major milestone has completed since the last review and less than 30 days have passed.
