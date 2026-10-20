---
name: blog-topic-planner
description: Research, deduplicate, prioritize, and brief product-led blog topics using a user-supplied product profile. Use for an editorial calendar or writer-ready H1/H2/H3 briefs; do not use to draft or publish finished articles.
---

# Blog topic planner

Plan blog topics for the **user's** product. No product, audience, competitor, content category, publishing limit, keyword threshold, or destination is built into this skill. Keep each product profile in the user's working context or chosen private workspace; never add it to this skill package.

## 1. Obtain the product brief

Ask the user for the essentials in [Product brief](references/product-brief.md) before selecting or scoring topics. The user must supply the product/service description, core capabilities and limits, target readers and their jobs, market and language, and the business goal for the blog. A website can supplement these answers but cannot replace the user's product description. Ask only for missing essentials; accept concise answers and `unknown` for optional fields. Never infer a product from this skill's author, repository, or prior examples.

Confirm the requested deliverable: ideas only, prioritized calendar, writer-ready briefs, or an update to an existing topic tracker. Use the user's requested number of topics and schedule. If omitted, propose a small batch and leave publication dates unassigned until capacity is known. Use the user's preferred categories; otherwise derive practical categories from their audience, product, and search intent rather than imposing a fixed taxonomy.

## 2. Establish the evidence baseline

- Freeze a research cutoff date, target market, and language. Note when a source or metric was checked.
- Read the complete topic history or an export of it, plus the live published blog archive when available. Include draft/planned topics so they are not proposed again. Record coverage gaps. If history is inaccessible, label ideas provisional and do not claim deduplication is complete.
- Read relevant product pages and documentation to verify supplied capabilities, limits, terminology, and suitable conversion paths. Flag any conflict with the user's brief instead of silently choosing one.
- Map the current site's topic clusters and relevant pages when the site exists. A proposed internal link must point to a verified destination. A missing blog URL alone does not prove a content gap; check what the existing page already answers.
- Use only tools and accounts authorized in this task. A keyword platform, analytics account, CMS, or tracker is optional. Continue with clearly labeled qualitative evidence when a metric provider is unavailable.

## 3. Research candidates in two stages

**Stage 1 — candidate.** Generate more candidates than the requested final count across the chosen categories. For each, record the reader's question or decision, search intent, proposed keyword, product connection, supporting source or demand signal, likely information gain, and nearest existing topic. Time-sensitive news needs a dated event and a relevant user consequence. Comparisons need a named audience, workflow, and decision thesis. Educational topics need a task that existing content does not already solve.

Classify factual sources separately from research stage:

| Source tier | Use |
| --- | --- |
| 1 — primary | Official documentation, original data, public filings, standards, firsthand tests. Use for decisive product, price, policy, and availability claims. |
| 2 — reported research | Bylined, dated reporting or research with visible sourcing or methods. Use for context and corroboration. |
| 3 — limited corroboration | Reviews or editorial industry posts with attributable authorship. Bound claims to the observed sample. |
| 4 — lead only | Forums, anonymous posts, aggregators, snippets, or interested comparison pages. Use to discover leads, not as final factual support. |

For each source keep its title, publisher, URL, publication or update date if shown, access date, exact supported claim, and limitations. Verify the final page supports that claim. Recheck volatile facts near delivery. Resolve conflicting sources or remove the claim.

**Demand evidence.** Prefer available first-party query or site-search data, then authorized keyword-provider metrics, then observable questions such as People Also Ask, autocomplete, related searches, support tickets, or community discussions. Record provider, query, market, date, metric definition, and report URL or reproducible connector record for each numeric metric. Missing volume or difficulty stays `unknown`, never zero. Relative trend data is not absolute search volume. Do not invent metrics, report links, or competitive rankings. If the user supplies minimum-volume or difficulty rules, apply them; otherwise judge demand against observed intent and the business goal without presenting an arbitrary number as a universal SEO rule.

When a keyword fails an applicable rule, try up to two meaning-preserving variants. Preserve the reader job. Log the attempts and leave the slot empty if no variant is eligible.

## 4. Deduplicate and select

Compare candidates with the full accessible topic tracker, published archive, relevant product pages, and one another. Review keyword family, intent, audience, promised answer, entity, and likely H2 questions. Record the closest match and one outcome: `Pass`, `Re-angled`, `Duplicate`, or `Cannibalization risk`. String overlap is only a prompt for semantic review. A different title does not make the same answer new.

Score surviving candidates from 1 to 5 on demand, source strength, product fit, differentiation, and timeliness/durability; total out of 25. Explain non-obvious ratings. The score helps rank eligible topics; it cannot override unsupported claims, unresolved duplication, or lack of a feasible original contribution. Use the user's category targets, publishing capacity, and dates. If a category lacks qualified ideas, report the gap after one bounded additional research pass instead of filling a quota with a weak topic. A translation of one article is not a separate original topic.

**Stage 2 — finalist.** Reopen decisive sources, refresh available keyword evidence, inspect current same-intent search results, and check for an existing site page targeting the query. Learn useful structure from other articles without copying their wording, examples, claims, or ordered outline. Call a page high-performing only when a recorded performance signal supports it. Check each finalist's planned section jobs against prior briefs, the live archive, and the current batch. If the reader journey is substantially repeated, change the angle, evidence asset, and section purposes; synonym swaps do not resolve overlap. Apply a numeric outline-similarity limit only if the user supplied one.

## 5. Write the brief and run three independent reviews

Use [Topic pack](references/topic-pack.md) for the deliverable. Every finalist needs one H1 and an ordered H2/H3 framework with each section's objective and writer instructions. State the target reader, intent, promised answer, primary and secondary terms where supported, original information-gain asset, verified sources and claim boundaries, internal link plan, proportional next step, and update needs for volatile facts. Do not promise tests, datasets, screenshots, or product results that the writer cannot actually produce. Propose publication dates only within the user's stated capacity and existing schedule.

Record three separate verdicts for each finalist:

1. **Reader value:** complete intent, distinct answer, feasible original evidence or reusable aid, clear and non-repetitive structure.
2. **Evidence:** claims directly supported, source authority and freshness adequate, numbers and qualifiers match, keyword metrics traceable or clearly qualitative.
3. **Execution:** writer can obtain the proposed asset, links and destination are real, page does not conflict with existing content, schedule and required fields fit the user's workflow.

Each verdict is `Pass`, `Fail`, or `Blocked`, with a concrete reason and correction. A finalist is ready only when all three pass. Recheck after a substantive correction. Preserve unresolved ideas as `Hold`, not as approved rows.

## 6. Deliver and reconcile

- Show the research cutoff, product brief version or supplied inputs, source and archive coverage, shortlisted and held ideas, dedup decisions, score rationale, complete briefs, capacity assumptions, and open limitations.
- Write to the tracker or output format the user specified. If no destination is specified, deliver a reviewable Markdown topic pack in the conversation. Avoid creating a new external table by default. Keep the full H1/H2/H3 brief with its primary topic record where the destination supports it.
- Before appending to a persistent tracker, re-read its current rows and check for concurrent additions. Use a stable run/topic identity to avoid duplicate retries. Verify that every new row and its outline can be reopened.
- Reconcile `Written` or `Published` states only from an actual draft or live URL and edit only the intended status field. A title match or planned brief is insufficient evidence.
- This skill selects and briefs topics. Article writing, CMS edits, and publication require a separate request or workflow.
