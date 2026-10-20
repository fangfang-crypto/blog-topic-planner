# Topic pack and writer brief

Use the structure below for each run. Adapt field names to the user's tracker instead of replacing its existing schema without a request.

## Run header

- Product brief supplied by the user; brief date or version.
- Research cutoff, market, language, target count, output destination, and categories chosen for this run.
- Coverage of topic history, live archive, product pages, demand data, and current search results. State any gaps.
- Publishing capacity and existing scheduled originals, when the user supplied them.

## Candidate log

Keep candidate-stage research separate from approved briefs. For each candidate record:

| Field | Meaning |
| --- | --- |
| Candidate ID | Stable identifier within the run. |
| Category / reader job | User-defined or derived category and the specific question or decision. |
| Proposed keyword / intent | Query and informational, comparison, or transactional intent. |
| Demand evidence | Numeric metric with provenance or labeled qualitative signal. |
| Product connection | Verified capability, page, or customer workflow. |
| Closest existing topic | Tracker row or published URL and why it might overlap. |
| Dedup outcome | Pass, Re-angled, Duplicate, or Cannibalization risk, with rationale. |
| Score | Five 1–5 dimensions and total out of 25, or a user-defined rubric. |
| Decision | Finalist, Hold, or Discard, with reason. |

## One complete finalist brief

Keep this information with the primary topic record when the destination supports it:

1. **Identity:** stable topic ID, run ID, category, status, target publication window if capacity is known.
2. **Reader and thesis:** audience, job, search intent, distinct promised answer, and why current content does not already serve it.
3. **Search plan:** primary keyword, useful secondary queries assigned to relevant sections, market, metric source and capture time, and qualitative demand signal if numeric data is unavailable. Blank metrics remain blank.
4. **Editorial metadata:** working title, proposed slug, H1, suggested summary or meta description when requested. Character counts are governed by the user's platform, not a built-in universal limit.
5. **Information gain:** the test, dataset, comparison method, firsthand example, decision aid, or reusable template the writer will create; who can produce it and where it appears in the outline.
6. **Ordered outline:** H2 sections in reader order. Each H2 has an objective, the claim or decision it answers, optional H3 subtopics, specific evidence or example to include, and writer instructions. Use as many sections as the task needs; avoid boilerplate headings.
7. **Evidence ledger:** for every decisive claim, source title, publisher, URL, published/updated date if shown, checked date, source tier, exact supported claim, and limitations. Mark time-sensitive facts for refresh.
8. **Link and next-step plan:** verified relevant internal destinations, proposed inbound links when the site allows them, descriptive anchors, and a product next step that fits the article. A proposed link is not an implemented link.
9. **Overlap review:** closest historical, live, and same-batch matches; keyword/intent decision; outline section-job comparison; material difference achieved through re-angling if needed.
10. **Quality verdicts:** Reader value, Evidence, and Execution each marked Pass, Fail, or Blocked with evidence, corrections, and final state.
11. **Open work:** unanswered product facts, source conflicts, unavailable metrics, content assets to produce, and a review date for volatile facts.

## Delivery states

- `Ready`: all three quality verdicts pass and the brief is writer-executable.
- `Hold`: a known gap, conflict, duplicate risk, or failed gate remains.
- `Provisional`: useful early research, but product input, archive coverage, or another prerequisite is incomplete.

When writing to a persistent tracker, retain its IDs and current fields. Re-read the destination before append, use a stable run/topic key for retries, and verify the resulting record and complete outline. Do not change production status from `Planned` to `Written` or `Published` without direct evidence of the draft or live page.
