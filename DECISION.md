# Decision — Niche Scout

**Date:** 2026-09-18  
**Decision:** `NEEDS EVIDENCE`

## 0. Phase A Output — Marketplace Selection

Full evidence is in `RESEARCH.md`, section A (A1–A5). This section only records the Phase A outcome: which marketplace proceeds to Phase B (keyword-level research). This is **not** a BUILD/REJECT decision — no keyword, pain, switching, or wedge research has been done yet.

**SELECTED MARKETPLACE: Atlassian Marketplace**

Strongest evidence supporting this choice:

1. **Only platform with a documented, official organic-newcomer-visibility mechanism.** Atlassian's "Rising Star" badge is explicitly designed to surface newer apps gaining traction, alongside "Spotlight" and "Bestseller" — no equivalent official newcomer mechanism was found for Wix, Shopify, or WordPress. (https://community.atlassian.com/forums/App-Central-articles/Same-Top-Searches-a-Different-Marketplace-What-s-Changed-for-App/ba-p/3247062, checked 2026-09-18)
2. **Fully platform-managed billing with no external payment dependency**, for "Paid via Atlassian" apps — Atlassian processes payment and recurring billing end-to-end. (https://developer.atlassian.com/platform/marketplace/pricing-payment-and-billing/, checked 2026-09-18)
3. **Documented, transparent revenue share** (84% to developer on Forge, up to 95–100% in year 1 up to $1M lifetime Forge revenue) — clearer and more generous than most SaaS platforms' defaults. (same source; https://www.atlassian.com/blog/development/updates-to-marketplace-revenue-share-2026, checked 2026-09-18)
4. **KYC/KYB and company-email requirements are a commonly cited solo-feasibility blocker; the user's existing German Gewerbe reduces some of this friction (registered business exists), but does NOT by itself confirm the specific "Paid via Atlassian" company-email requirement is met.** `CHECK PENDING`: Atlassian's guideline text says personal/generic domains (Gmail, Yahoo) are not permitted — this requires a company-domain email address, which is a distinct, unverified fact from having a Gewerbe. Needs direct verification (does the user have a company-domain email? does Gewerbe registration alone satisfy Atlassian's KYB vendor check?) before this can be marked resolved.
5. **Explicit, published ranking factors** (keyword relevance, semantic matching, engagement score) give a concrete, actionable target for Phase B keyword research, unlike Wix where no ranking documentation was found at all. (https://developer.atlassian.com/platform/marketplace/marketplace-search-results-and-rankings/, checked 2026-09-18)
6. **Marketplace scale supports a long-tail niche strategy**: 7,200–8,000+ apps and 1,800+ active vendors is large enough to have active competition/demand signal, but smaller than Shopify's 18,000+ apps, meaning less raw noise per category (secondary sources, checked 2026-09-18).

**B0 cold-start validation — CLOSED 2026-09-19.** Checked 18 live Rising Star apps and ran 8 real customer search queries directly against marketplace.atlassian.com (see RESEARCH.md A3 → "B0. Cold-start validation follow-up" for full detail, sources, and dated URLs). Result, stated as two separate claims — do not merge them:

- **Organic discovery via Marketplace search: EVIDENCED.** Rising Star apps surfaced in **7 of 8** real search queries, including **two #1 placements** ("smart assignment," "real time analytics") and one **#2** ("sprint retrospective"), ahead of apps with more reviews/installs. This is a mechanical property of the live search algorithm, not just Atlassian's own promotional collection page. The one query where no Rising Star app appeared ("time tracking") was the most saturated/generic category tested.
- **First-time unknown vendor success: UNKNOWN.** Every one of the 18 sampled Rising Star apps belongs to a vendor that already runs multiple other marketplace apps (2 to 17+ apps each), and at least one (Agile Pulse) is a paid upsell cross-promoted from an existing free product with 3,300+ installs. No example was found — positive or negative — of a Rising Star badge going to a genuinely first-time, single-app, unknown vendor. Mark `NEEDS EVIDENCE`, not `CONFIRMED IMPOSSIBLE` and not `CONFIRMED POSSIBLE` — CONTEXT.md's rule against treating an absence as proof applies in both directions.
- Security questionnaire / EULA / demo-account infrastructure was **observed among all sampled Rising Star vendors**; whether this is causally necessary for reaching similar placement, or merely correlated with being an established multi-app vendor, is **unknown** — do not treat it as a requirement ("table stakes") without further evidence.

**REJECTED:**

- **WordPress** — the wordpress.org plugin directory (the surface with real organic search/discovery, ~6,086 new plugins in 2025) **structurally forbids paid or gated code**; a paid tier must be sold through external checkout, which fails the project's Marketplace Gate requirement for marketplace-managed or platform-native billing. This confirms — with direct evidence from the official Plugin Directory guidelines — the previously unverified claim "WordPress не відповідає commercial model." (https://developer.wordpress.org/plugins/wordpress-org/detailed-plugin-guidelines/, checked 2026-09-18). WordPress.com Marketplace does have real billing but its discovery reach and new-entrant traction are unverified and likely much narrower than wordpress.org.
- **Meta** — no Meta surface fits the model for a general SaaS/productivity app. The Business Partner Directory is an agency listing, not a customer-facing app catalog. Meta Horizon Store is a genuine marketplace (search, billing, reviews) but is scoped to VR/AR hardware apps/games, a different product category, and has documented developer complaints about discovery favoring already-popular content. (https://www.facebook.com/business/partner-directory; https://skarredghost.com/2024/11/11/meta-quest-store-developers-problems/, both checked 2026-09-18)
- **Wix** — not rejected outright, kept as a documented fallback candidate. Commercial fit and billing are solid (confirmed platform-managed billing, generous first-year revenue share), but no official ranking-signal documentation and no evidence of any new-entrant gaining traction in the last 12 months were found in this pass. If Atlassian's Phase B research uncovers a fatal blocker, Wix is the next candidate to deep-research — not Shopify, because Shopify's evidenced cold-start friction (new apps need ~10 reviews in 30 days to rank, no newcomer-boost mechanism) is real and better documented than any blocker found for Wix.

**Note on Shopify:** Shopify was **not rejected** — it has the strongest solo-feasibility track record (multiple independently documented bootstrapped solo apps) and the best revenue-share terms found. It ranks second to Atlassian only because it lacks an official newcomer-visibility mechanism and has well-documented cold-start ranking friction for apps with zero reviews. It remains a credible alternative if Atlassian's Phase B research surfaces a blocker (e.g., the security-review overhead proves heavier in practice than expected).

## 0.5 Phase B1 Output — Search Landscape (2026-09-19)

Full evidence, all 22 query records, and the full PROMISING/WEAK/REJECT table are in `RESEARCH.md` under "Phase B1 — Search Landscape". This section records only the phase outcome. **No product or SaaS idea has been selected — this is not a BUILD-track decision.**

**Method:** 22 customer-intent queries were built from Atlassian's real live category taxonomy and natural customer language, deliberately not reusing B0's known Rising-Star examples. All were executed live on 2026-09-19 against `marketplace.atlassian.com/search`.

**Honest headline finding:** Rising Star badges are nearly absent from non-cherry-picked queries. Across 22 queries, exactly one Rising Star badge appeared (`okr tracking jira`, position ~9, "Bazz-OKR" by a single-app vendor, 4 reviews/47 installs) — a positive but single, unreplicated data point for the still-open "first-time unknown vendor success" question (see Section 0). The large majority of queries are dominated by PLATINUM/GOLD partner veterans with Bestseller/Spotlight badges and installs in the thousands to tens of thousands.

**Classification result (of 22 queries):** 4 PROMISING outright, 1 PROMISING-on-visibility-but-NEEDS-EVIDENCE-on-demand, 9 WEAK, 7 REJECT, 1 NEEDS EVIDENCE (ambiguous query-intent match). This is fewer clean PROMISING results than the 5–10 the task anticipated; reported as observed rather than stretched.

**Selected search intents to carry into Phase C/D (maximum 5, per instruction):**

1. `user access review` (Jira) — PROMISING. Tiny/new apps (12–46 installs) occupy the top ranks with zero veteran or badge presence.
2. `gdpr compliance confluence` — PROMISING. Small/mid GOLD/SILVER vendors throughout, no PLATINUM incumbent.
3. `confluence page views analytics` — PROMISING. Small/unbadged vendors genuinely interleaved with PLATINUM incumbents, not excluded by them.
4. `hubspot integration jira` — PROMISING. All four genuine competing apps are small/SILVER-or-unbadged, no incumbent, no placement badges in category.
5. `audit log confluence` — PROMISING on search-visibility, but flagged `NEEDS EVIDENCE` on underlying demand strength (every competing app has single-digit-to-30 installs and no visible ratings — could mean "wide open" or could mean "no one wants this yet"; Phase C/D must resolve this, not assume it).

**Cross-cutting observation (not a conclusion):** 4 of these 5 selected intents (all but HubSpot integration) sit within the same admin/compliance theme on Atlassian Marketplace. This may indicate a genuinely underserved theme rather than four unrelated niches — a hypothesis for Phase C to test, not something to assume as confirmed.

**Explicitly not done in this phase, per instruction:** no SaaS idea chosen, no MVP scoped, no winner picked, no 3★-review analysis, no pain research beyond what was needed to read query intent.

## 0.6 Phase C Output — Demand Validation (2026-09-19)

Full evidence (per-app installs, reviews, review dates/content, release activity) is in `RESEARCH.md` under "Phase C — Demand Validation". This section records only the phase outcome. **No product or SaaS idea has been selected — this is not a BUILD-track decision.**

**Method:** for each of the 5 Phase B1 intents, individual app listing pages (overview + reviews tabs) were checked for 3–5 representative competitors per intent — not just search-result badges. Checked: payment model, release recency, review dates/content (not just star rating), explicit production-use/switching language. Explicit rule applied throughout: low competition alone is never treated as evidence of a good niche — it is marked `NEEDS EVIDENCE` until real demand (installs, reviews, proof of paying/long-term use) is shown.

**Verdicts:**

1. `user access review` — **NEEDS EVIDENCE.** Real, detailed, multi-year demand evidence exists (Multiplier: "used for a few years," explicit switching language vs. alternative IdP solutions, 177 installs, 19 reviews) — but Multiplier is a **broader IGA/access-management suite**, not the narrow "access review" point-solution the query names. The narrowly-scoped apps matching the literal intent (Access Reviewer360, Project Access Review, AuditAdmin — 10–46 installs) have only 0–2 thin reviews each, with no production-use or switching language. Demand is proven for an adjacent, broader category — not confirmed for this specific narrow intent. Per instruction, these two facts are not merged into a single PASS.
2. `gdpr compliance confluence` — **PASS.** All 3 sampled apps show genuine, dated customer reviews describing concrete regulatory outcomes (e.g., "official approval from our data protection department"; MedTech eQMS validation tied to AAMI standards), an active feedback→feature development loop (a 2022 feature request was later shipped, confirmed in the same review thread), and continued 2026 releases. Real competition across 3 differentiated sub-niches (general GDPR/PII, DLP/classification, MedTech validation), no PLATINUM incumbent.
3. `confluence page views analytics` — **PASS.** Strongest durable-demand evidence in the set: a customer reports continuous use "since 2012" of the category leader (Viewtracker, 2,374 installs, 62 reviews), and a second, much smaller vendor (view26, 306 installs) has an independent 2-year paid-usage testimonial. Small vendors are confirmed to coexist with (not be excluded by) the veteran. Caveat: the veteran is strong and actively adding AI features (Aug 2026), narrowing the wedge space versus GDPR compliance.
4. `hubspot integration jira` — **PASS, with a caveat.** 2 of 3 sampled apps show genuine reviews with concrete production-use description (one details a live Freshdesk→JSM+HubSpot migration). The third and largest-by-installs competitor (Korvex, 457 installs) has **zero reviews** — an install/review mismatch flagged as `NEEDS EVIDENCE` for that specific app, though it does not invalidate the intent since the other two competitors show real demand.
5. `audit log confluence` — **NEEDS EVIDENCE, strongly leaning toward insufficient demand.** Hard scrutiny requested (per instruction) because Phase B1 already showed thin installs. Result: all 4 genuine audit-log-specific apps have **zero reviews**, and 2 of the 4 are literally brand-new (first public release 2.5–3 weeks before this check). "Paid via Atlassian" is present on every one, but that reflects billing-model availability, not a completed purchase. No evidence of any paying or long-term user exists for this intent. Explicitly not downgraded to outright REJECT (too early to distinguish "no demand" from "too new"), but does not qualify as PASS.

**Result: 3 of 5 intents carried forward to Phase D (Pain + Switching), within the "maximum 3" instruction limit:**

- `gdpr compliance confluence`
- `confluence page views analytics`
- `hubspot integration jira`

**Explicitly not done in this phase:** no product selected, no MVP scoped, no winner picked, no 3★-review-driven analysis, no numerical scoring used.

## 0.7 Phase D Output — Pain + Switching Evidence (2026-09-19)

Full evidence (per-quote table: exact quote, app, date, URL, pain category, frequency, severity, workaround, switching language, product-vs-support) is in `RESEARCH.md` under "Phase D — Pain + Switching Evidence". This section records only the phase outcome. **No product or SaaS idea has been selected — this is not a BUILD-track decision.**

**Method:** collected genuine, dated, text-bearing customer statements (not star-only reviews) from multiple competitors per intent — 7–8 statements per intent, ~22 total. One review was excluded from the evidence base because the vendor publicly disputed its authenticity (no matching support record or LinkedIn profile). Ran 3 targeted secondary-source searches (Reddit/G2) for explicit switching language per intent — all three returned zero on-topic results, recorded as absence of additional evidence, not a signal either way.

**Honest headline finding: no intent produced an explicit "switched from X to Y" / "alternative to X" quote.** Per CONTEXT.md §7 ("complaint != willingness to switch"), this means none of the three intents can be marked PASS on the strict switching-evidence bar, regardless of how much other pain evidence exists.

**Verdicts:**

1. `gdpr compliance confluence` — **NEEDS EVIDENCE.** Real, specific pain found — a detailed, dated review describing manual bulk-classification pain across "thousands of individual pages," corroborated by a multi-year vendor feature-request→ship cycle in the same review thread — but zero switching language, and each specific pain point is backed by only one detailed source, not independently repeated across multiple customers.
2. `confluence page views analytics` — **NEEDS EVIDENCE.** Found switching-from-native evidence (two independent customers, 18 months apart, explicitly say Confluence's own built-in analytics was insufficient and drove them to a paid app) — a real but weaker signal than competitor-to-competitor switching, and it only re-confirms demand already established in Phase C rather than surfacing a new underserved pain. The category's veteran (Viewtracker) is strong and actively investing in new features, narrowing wedge space.
3. `hubspot integration jira` — **NEEDS EVIDENCE**, with the strongest signal of the three: one review contains explicit comparison-shopping language ("I tested a lot of integration tools to find the right one for us") plus a specific, named feature gap (missing multi-select/date field support). This is the closest to true switching evidence found in the whole research pass, but the associated wedge (deep HubSpot↔Jira field-type sync) carries a **HIGH support-trap rating** — integration/API apps are structurally prone to customer-specific configuration work and breakage from a third-party API (HubSpot) outside the developer's control, which is a direct Solo Gate concern (CONTEXT.md §10).

**Deliberately not concluded:** "more negative reviews" was not treated as "better opportunity" — the intent with the most positive reviews (HubSpot integration) produced the strongest switching signal, not the intent with the most complaints; this is called out explicitly in RESEARCH.md as a deliberate rejection of that naive heuristic. Competitor weakness (reliability bugs, missing features) was not treated as proof of demand.

**Maximum 2 pain/wedge hypotheses carried forward, per instruction:**

**Hypothesis 1 — GDPR/Confluence: narrow bulk/default PII-classification tool for large legacy Confluence spaces**
- Problem → admins of large/old Confluence instances cannot bulk- or default-classify pages by data sensitivity; manual classification of "thousands of individual pages" is described as "very painful."
- Evidence → 1 detailed, dated review (Compliance for Confluence, Feb 7 2022) + a confirmed multi-year vendor feature-request→ship cycle in the same thread — moderate, single-sourced.
- Switching signal → none found; only sustained frustration until the incumbent eventually shipped the feature.
- Minimal wedge → a narrow Forge app doing bulk PII scan-and-classify with CQL-style scoping, not a full DLP suite.
- Support risk → MEDIUM (bulk content actions need confirm/rollback UX to avoid "you broke my labels" tickets).
- Platform/API risk → LOW–MEDIUM (Confluence REST/Forge content search & labeling; specific limits not independently verified — NEEDS EVIDENCE).

**Hypothesis 2 — HubSpot↔Jira: reliable sync with full field-type support**
- Problem → existing HubSpot-Jira connectors don't support some field types (multi-select, date), forcing customers into manual workarounds or continued comparison-shopping across tools.
- Evidence → 1 detailed review with explicit comparison-shopping language (Getint, Oct 23 2024) — the strongest signal found in all of Phase D, but single-sourced.
- Switching signal → comparison-shopping language ("tested a lot of integration tools to find the right one for us") — the closest to true switching evidence in the whole corpus, though not a full "switched from X."
- Minimal wedge → correct, complete field-type mapping (multi-select, date, etc.) with no workaround required.
- Support risk → HIGH — integration apps systematically generate customer-specific configuration requests and depend on an external API (HubSpot) outside the developer's control; a direct Solo Gate concern.
- Platform/API risk → MEDIUM–HIGH — dual dependency on both HubSpot's API and Jira/Forge APIs, not just one.

**Explicitly not done in this phase:** no product selected, no MVP designed, no numerical scoring used, no intent marked PASS based on complaint volume, no competitor weakness treated as proof of our own demand.

**Note on switching-evidence methodology (added 2026-09-19):** per user instruction, the absence of a literal "switched from X to Y" quote is no longer treated as an automatic fail. Switching evidence is now classified as: **A** — direct replacement, **B** — comparison-shopping, **C** — replacement intent, **D** — pain only. Retroactively applied to Phase D: Anne Dietz (HubSpot/Getint) = B; Craig Parsons / Thilini Rathnayake = weak/implicit B; Andy Gladstone / Natalie Dolce (confluence-analytics, switching from native tooling) = A, but against a "no tool" baseline rather than a competitor; most other quotes = D (pain only). Full detail in RESEARCH.md.

## 0.8 Phase E Output — Wedge Kill Test (2026-09-19)

Full evidence (competitor-by-competitor feature comparison, sourced and dated) is in `RESEARCH.md` under "E. Phase E — Wedge Kill Test". This section records only the outcome. **`confluence page views analytics` is moved to `HOLD`** per instruction — not researched further until a concrete unmet job is found; no research budget spent on it in this phase.

**Method:** for each of the 2 active Phase D hypotheses, checked 7–8 existing Marketplace apps for exact feature overlap, not just competitor existence — the explicit goal was to try to kill each hypothesis, not confirm it.

**Hypothesis 1 — GDPR/Confluence bulk PII classification: `KILLED`**

The literal job is already delivered, with active development, by at least 3 independent competitors: AppFox's Compliance for Confluence (CQL-scoped bulk classification, default classification, publish-time enforcement — shipped in direct response to the exact feature request found in Phase D), Actonic's Data Protection Toolkit (scheduled recurring scans with auto-redaction), and Polymetis's PII Protection and DLP for Confluence (space-level scan → classify → Confluence/Jira Automation trigger, SOC 2 Type II certified). A 4th (miniOrange's Data-PII-Scanner) explicitly lists scheduled/bulk scanning as "coming up," confirming the market is actively converging on this exact feature. Per direct instruction, a feature already offered by competitors cannot be called a wedge. One unverified, speculative alternative shape surfaced — a one-time "legacy cleanup" tool/engagement instead of a recurring compliance subscription — but zero customer evidence supports it; it is not a confirmed hypothesis, only a noted gap in how the category is currently packaged.

**Hypothesis 2 — HubSpot↔Jira reliable field-type sync: `KILLED`**

Checked 7 direct competitors plus HubSpot's own native, free Jira integration. Every possible narrow configuration is already occupied by a live, funded competitor: full two-way sync (Getint), configurable two-way/one-way/display-only (Korvex), read-only CRM-context display (Appsvio), embed + automation-trigger without full sync (resolution — a first-version app that already has 490 installs/11 reviews, itself a notable adjacent data point), and an enterprise no-code external option with explicit conflict/retry handling (OpsHub). The evidenced pain (missing multi-select/date field types, Phase D) turned out to be part of a systemic, cross-platform technical-debt pattern in Getint's whole multi-connector business (confirmed via their Sep 2026 changelog fixing equivalent field-handling bugs in Asana, ClickUp, and Freshservice connectors too) — an execution-quality gap the vendor is actively closing, not an unaddressed job. Per instruction not to propose a full two-way integration, every viable narrower slice (read-only, display-only, embed-trigger) was checked and found already occupied.

**Result: both active hypotheses killed. No live wedge candidate remains among the 3 intents researched in Phase C/D.** Per AGENTS.md §5 (Veto rules: "Wedge = veto"), this is not compensated by the real demand evidence found in Phase C or the volume of positive reviews found in Phase D — a missing wedge stops progress toward BUILD regardless of other positives. Neither hypothesis was designed into an MVP or architecture; both stopped at the hypothesis stage as instructed.

**Explicitly not done in this phase:** no MVP designed, no architecture designed, no coding started, no winner chosen by scoring.

## 0.9 Phase F Output — Fresh Keyword Expansion (2026-09-20)

Full evidence (per-query competitor table, first-pass and second-pass narrowing) is in `RESEARCH.md` under "Phase F — Fresh Keyword Expansion". This section records only the outcome.

**Method:** checked 35 new customer-intent queries (patterns: `automatically.../bulk.../validate.../enforce.../prevent.../notify.../clean.../compare.../export.../detect.../find...`), explicitly excluding the 3 closed-off topics (GDPR/Confluence, HubSpot↔Jira, `confluence page views analytics`). First pass narrowed 35 → 8 on job-clarity + non-saturation + Architecture Fit grounds. Second pass narrowed 8 → 3 by checking paid demand, real installs, active competitors, smaller/new-entrant presence, clear customer intent, Architecture Fit, and expected support burden.

**Headline finding:** the Atlassian Marketplace is heavily saturated for generic bulk/export/enforce/notify operations on Jira/Confluence — 15 of 35 queries were REJECT (dominated by established players with thousands of installs, several with RISING STAR/SPOTLIGHT/BESTSELLER badges: Appfire, K15t, eazyBI, Agile Pulse). Badge placement was observed exclusively on large incumbents across all 35 queries — never on a small/new candidate — confirming Marketplace promotional visibility is not itself a signal of open niches.

**3 candidates carried into the next Pain/Switching phase:**

1. **`enforce definition of done jira`** — a Jira workflow-gate blocking issue transition until a Definition-of-Done checklist is satisfied. Evidence: 4 independent small vendors (ReDo, Definition of Done & Ready, Definition of Ready, Definition of Done) attempted this exact narrow job, all with weak execution (2–63 installs; the one with the most installs has the worst rating, 2.8/5). Repeated independent attempts at the same job, none executed well, is treated as a genuine demand signal — not the "few competitors = good niche" fallacy, since here multiple real vendors already validated that customers search for and try to solve this. Architecture Fit: LOW (Forge-native workflow condition).
2. **`prevent issue reopening jira`** — carried forward with an explicit open question rather than a settled verdict: the two existing competitors (Reopening Counter, Reopen Receipt) both chose to build *tracking/visibility* tools, not an actual *hard gate* blocking reopening. This could mean the hard-gate niche is genuinely open, or it could mean real customers specifically avoid a punitive blocking mechanism and prefer visibility — the Pain/Switching phase must resolve which. Architecture Fit: LOW, but support burden is flagged HIGH (a workflow blocker that misfires generates urgent, high-visibility tickets).
3. **`compare confluence page versions`** — carried forward with an explicit native-feature-overlap risk: Confluence already ships built-in comparison for adjacent page versions, so the one near-zero-traction competitor (1 install) may only be capturing a narrower unmet slice (non-adjacent-version or cross-page diff) than the query implies. Architecture Fit: LOW.

**Deliberately NOT carried forward — `find unused custom fields jira`:** this query returned **zero** competing apps, the single strongest "gap" signal of the whole batch — and is explicitly *not* promoted to the top 3 for that exact reason. Per the project's standing veto against concluding "few/no competitors = good niche," zero competitors is equally consistent with "nobody will pay for this" as with "open niche." Custom-field bloat is a commonly discussed pain in Jira admin communities outside the Marketplace itself, but that is unverified external evidence, not Marketplace-internal evidence. This is recorded as a flagged idea for a future keyword round if external (community-forum) evidence of willingness to pay emerges — not as a rejected idea and not as a hidden BUILD candidate.

**Also explicitly rejected at the second-pass stage** (see RESEARCH.md for full reasoning): `automatically assign reviewer jira` (job-definition ambiguity — Jira-native reviewer vs. PR/code reviewer requiring Bitbucket/GitHub, which would flip Architecture Fit to HIGH), `detect duplicate pages confluence` (Architecture Fit MEDIUM — likely needs external text-similarity/ML — combined with zero competitor attempts, a worse combination than a LOW-fit empty niche), `enforce naming convention jira` (not empty — already solvable by generalist automation platforms like ScriptRunner, 34.8k installs), `prevent accidental page deletion confluence` (Confluence's native 60-day trash/restore already covers most of the literal query, narrowing real unmet pain to a much smaller slice than asked).

**Explicitly not done in this phase:** no product chosen, no MVP designed, no architecture designed, no numeric scoring, no deep review mining.

## 0.10 Phase G Output — Native Capability Kill Test (2026-09-20)

Full evidence (native mechanism citations, per-app install/review tables, sourced and dated) is in `RESEARCH.md` under "F2. Phase G — Native Capability Kill Test". This section records only the outcome.

**Method:** for each of the 3 Phase F candidates, checked official Atlassian documentation for native workflow conditions, validators, forms, required fields, automation, transition restrictions, subtask-blocking, and Confluence native version history/compare — explicitly trying to KILL each candidate via native functionality and/or existing Marketplace saturation, not to confirm it.

**Verdicts — all 3 KILLED:**

1. **`enforce definition of done jira` — KILLED.** Native only provides `basic transition gating` (Field Required Validator on individual fields, Permission/Group/Value-Field conditions, Sub-Task Blocking Condition) — there is no native checklist field type and no single mechanism for structured multi-item DoD enforcement, confirming the distinction the user asked to isolate. However, that exact residual gap is already occupied — and not thinly. **Checklists for Jira (Pro) by HeroCoders (7,887 installs, 264 reviews, 4.5/5)** explicitly markets itself for "enforce DoD and acceptance criteria" via its own checklist workflow validators that block transitions. Two smaller apps (Definition of Done by Chasing Agility, 63 installs; Enterprise Checklists for Jira by Cognitiff) do the identical job. This corrects Phase F, which searched only literal "definition of done"-named apps (2–63 installs) and missed the much larger functional "Checklist for Jira" category that already dominates the exact job.
2. **`prevent issue reopening jira` — KILLED.** Native comprehensively covers the literal "prevent/block" job: full removal of the reopen transition (no app needed), role/group restriction via Permission Condition or the native "Restrict who can move a work item" rule (available even in Team-managed projects), time-limited reopen via Date Compare Validator, conditional reopen via Value Field Condition, and a documented native automation-rule workaround for the one confirmed gap (JSM customer-portal transitions ignore validators). The only real native gaps are (a) no audit trail of *blocked* reopen attempts and (b) no native count/report of how many times an issue was reopened — but this narrower "reopen analytics" job (a different job than "prevent") is already served by both a small dedicated app (Reopening Counter, 48 installs) and a large generalist incumbent (Timepiece – Time in Status, 4,477 installs, 270 reviews, 4.8/5) whose "Status Count report" explicitly surfaces "reopens and rework loops."
3. **`compare confluence page versions` — KILLED.** The literal job is fully native: Version History lets a user select **any two arbitrary versions** of the same page (not only adjacent ones) and view a highlighted diff (additions/deletions/formatting changes, unchanged text collapsed). Per the user's own stated rule, a literal job fully closed by native functionality is killed without further pain research. The only confirmed native gap — automatic cross-page comparison (diffing two *different* pages) — is a distinct, unverified job with zero customer evidence found, and is not actually solved by either existing low-traction Marketplace app (Diff for Confluence, 6 installs; diff, 12 installs — both require manually pasted text/git patches, not live page content).

**No candidate was rescued via artificial narrowing.** In each case, a possible narrower alternative (regulated-industry DoD templates; reopen-count analytics; cross-page diff) was explicitly logged as a *separate*, unverified job-to-be-done with no customer evidence — not as a hidden surviving version of the researched candidate, per direct instruction.

**Result: all 3 Phase F candidates are dead. No live wedge candidate currently exists on Atlassian Marketplace among any intent researched across Phase C through Phase G.**

**Explicitly not done in this phase:** no MVP designed, no architecture designed, no numeric scoring, no Pain/Switching research conducted for any of the 3 candidates (killed before that stage, per instruction).

## 0.11 Phase H Output — Operational Pain Discovery (2026-09-20)

Full evidence (10-class first-pass catalogue with citations, 5-class search-test tables, all sourced and dated) is in `RESEARCH.md` under "G. Phase H — Operational Pain Discovery". This section records only the outcome. **No blind keyword sweep was run** — this phase started from real, currently-listed Marketplace apps (2026 releases, low/moderate installs, Rising Star collection) and worked backward to the underlying operational problem, per direct instruction.

**Methodology correction (documented honestly):** the first search-test pass used `WebFetch` directly on `marketplace.atlassian.com/search`, which returned **identical top-8 results for 5 unrelated queries** — verified via `curl` to be a static, client-side-rendered JS shell (472,865 bytes, byte-identical regardless of query string). That pass was discarded as unreliable (likely small-model hallucination, not real page content) and **redone with a real rendered browser (Playwright)**, which produced correct, query-distinct results. This is recorded so the lesson isn't lost: `marketplace.atlassian.com/search` cannot be trusted via plain WebFetch.

**Method:** built a 10-class catalogue of real operational-pain problem classes, each anchored to at least one currently-listed Marketplace app plus a native-capability check and a saturation check (per class: example app, evidence URL, native gap, marketplace saturation, initial status). Stopped at 10 classes rather than padding to 15 with weakly-evidenced filler (two explored directions — sprint/board hygiene, notification/webhook failure monitoring — turned up no dedicated app or clear customer-pain source and were dropped, per AGENTS.md §2). Narrowed 10 → 5 PROMISING classes, ran a real browser-rendered search test (1-2 queries each) for those 5, then narrowed 5 → 3.

**10-class first-pass result:** 1 REJECT (custom field/config bloat cleanup — dominated by an established incumbent, Optimizer for Jira, 1,133 installs/33 reviews/4.6; native Site Optimizer already covers Enterprise/Premium plans), 1 WEAK (Confluence broken links/orphaned attachments — real, Atlassian-acknowledged native gap via an open, unresolved feature request CONFCLOUD-16577, but a credible Gold-partner incumbent already holds 147 installs), 3 NEEDS EVIDENCE (automation rule silent-failure monitoring, Cloud-specific license/inactive-user audit, Marketplace app usage/spend audit — all have real confirmed customer pain but no verified, currently-active dedicated competitor was found, so none was promoted on unverified-competition grounds), and 5 PROMISING carried to the search-test stage.

**Search-test result (5 → 3):** the search test surfaced an important, honest correction — two of the five PROMISING classes turned out to already be crowded with 10-13 near-identical, independently-launched 2026-vintage competitors each:
- **Configuration change audit trail** (before/after diff for admin changes) — 13 direct competitors found in one search, mostly 0-20 installs, launched within roughly a 6-month window (March-August 2026); one vendor (Shtern Consulting OÜ) and another (AppForge.ai) are each independently running two near-identical apps in this space, and a third small vendor (keelapps) is building narrow apps across two different classes. The strongest confirmed native gap in the whole phase ("Jira's native audit log can't tell you which admin changed a scheme, and it keeps no before/after history," plus a separate vendor's own copy: "beyond Jira's 180-day log") — but too crowded for a new solo entrant to differentiate against 13 existing near-twins.
- **Access/permission review & certification** — 10 direct competitors found, and this is **not a fresh discovery**: it is the same macro-niche as Phase C's `user access review` (already NEEDS EVIDENCE there, anchored on Multiplier, a broader IGA suite with 177 installs). Phase H confirms the niche is now even more densely populated with fresh 2026 entrants than Phase C observed, not more open.

**Final 3 problem classes carried into the next Pain/Switching phase (all Jira/Confluence Cloud, Atlassian Marketplace only):**

1. **Orphaned digital artifacts after user/project lifecycle events (Jira)** — filters, dashboards, issues, and project leadership left behind by deactivated users or archived projects. Only 2 direct competitors found (Orphaned-Owner Cleanup, Leaver Cleanup & Owner Reassignment for Jira — both brand-new, 0 installs/reviews, functionally near-identical). Native gap confirmed by Atlassian's own support KB, which offers only a manual/scripted workaround, not a UI feature.
2. **Issue-level data quality / hygiene drift after creation (Jira)** — a periodic re-scan of existing issues for data-quality decay (blanked required fields via bulk edit/API, staleness), distinct from the one-time, transition-time Field Required Validator. Only 3 direct competitors found (Data Health for Jira, Data Quality Score for Jira, Issue Quality for Jira), all near-zero installs, none dominant.
3. **Confluence stale/outdated content detection & review cadence** — distinct from the already-`KILLED` page-version-comparison job (Phase G). 3-4 direct competitors found (Stale Page Finder, Evergreen, Keep Docs Updated, Page Review Manager); the one prior established incumbent (Outdated for Confluence) has since been **archived/discontinued**, reducing rather than raising competitive pressure. Native gap confirmed: Confluence's own content-review-reminder capability (via Automation) is Premium/Enterprise-tier-gated only.

**Not carried forward, with reasons recorded (not silently dropped):** Configuration change audit trail and Access/permission review & certification (both real, both native-gap-confirmed, both killed at this stage purely on saturation/prior-research-overlap grounds, not on demand or native-capability grounds); custom field/config bloat cleanup (REJECT — saturated, partially native); broken links/attachments (WEAK — credible incumbent present); automation-failure monitoring, Cloud license audit, and Marketplace app spend audit (NEEDS EVIDENCE — real pain, no verified competitor found, not promoted on that basis per the project's anti-fabrication rule).

**Explicitly not done in this phase:** no product chosen, no MVP designed, no architecture designed, no numeric scoring, no deep review-mining (individual dated customer quotes are reserved for the next, not-yet-started Pain/Switching phase).

## 0.12 Phase I Output — Pain / Switching / Wedge Test (2026-09-20)

Full evidence (per-class Buyer/Trigger/Workaround/Economics/Existing-paid-behavior tables, 30 total dated customer quotes across the 3 classes, wedge tests) is in `RESEARCH.md` under "H. Phase I — Pain / Switching / Wedge Test". This section records only the outcome. No new keyword sweep was run; no previously-`KILLED` intent was revisited; Atlassian Marketplace remains the marketplace.

**Method:** for each of the 3 Phase H problem classes, established buyer role, trigger/frequency, current workaround, economic/risk consequence, existing paid behavior (real pricing pulled live via a rendered browser — WebFetch again proved unable to show interactive price calculators), 7-14 genuine dated customer statements per class (sourced from Atlassian Community threads and Marketplace review pages, not fabricated), a native-capability re-check, and up to 2 narrow wedges per class with full field breakdown (Problem/Buyer/Trigger/Current workaround/Existing paid alternative/Unmet job/Minimal wedge/Why pay/Why not native/Support burden/API risk/Architecture Fit).

**Verdicts:**

1. **Orphaned digital artifacts after user/project lifecycle events (Jira) — NEEDS EVIDENCE.** Buyer confirmed (Jira Cloud site admin/IT ops, self-identified across multiple 2018-2025 community threads). Native gap confirmed continuously unaddressed for 7+ years (official Atlassian Team answer, 2018: private filters/dashboards can only be reassigned via reactivate-and-impersonate). Real economic case, including a direct historical willingness-to-pay quote ("you can do it but only if you spend another $1,000 on yet another plug-in," 2019) and a governance-risk quote about departed employees still appearing as accountable owners in reports. However: **zero confirmed paid transactions** — both direct competitors (Orphaned-Owner Cleanup, $90/mo@100 users; Leaver Cleanup & Owner Reassignment, $100/mo@100 users) have 0 installs and 0 reviews — and the most obvious wedge angle (bulk reassignment) is already explicitly claimed by Leaver Cleanup's own listing copy, narrowing differentiation room. Not `KILLED` (every other link in the chain is real) and not `SURVIVES` (the existing-paid-behavior link is unproven).
2. **Issue-level data quality/hygiene drift after creation (Jira) — KILLED.** Not killed by native capability (a real gap exists — Field Required Validator only fires at transition time) but by the pain/switching chain failing on multiple links at once: buyer role is diffuse (no self-identified role found, unlike the other two classes), pain evidence is indirect and bleeds into two already-explored themes (backlog/abandoned-issue cleanup, and custom-field bloat — already `REJECT` in Phase H for saturation), and all 3 independently-launched dedicated apps (Data Health for Jira, Data Quality Score for Jira, Issue Quality for Jira) show zero confirmed transactions (0-3 installs, 0 reviews each) — a weaker signal than Class 1, not a stronger one, because it isn't paired with a clear buyer or a distinct economic story.
3. **Confluence stale/outdated content detection & review cadence — SURVIVES.** Every required link in the chain is independently confirmed: buyer (a real user explicitly self-identifies, 2024-06-12: "i am Knowledge Manager here"), recurring problem with an explicit admin-set cadence ("quarterly/monthly/yearly review," 2025-01-03), existing paid behavior (the directly-adjacent Confluence approval/content-governance category has established, well-reviewed incumbents at real scale — Page Approval for Confluence, 1,700 installs/73 reviews; Approvals for Confluence, 983 installs/21 reviews — proving real budget exists for this class of tool even though the literal "staleness detection" sub-niche is still young), credible reason to pay (an Atlassian Community expert confirms native Automation sends "50 separate emails" for 50 expired pages — a governance process that silently fails at scale — and one user explicitly describes comparison-shopping toward a paid plugin after native fell short, a type-B switching signal), a native gap confirmed on three independent points (Automation is Premium/Enterprise-tier-gated; even there it fires once per cycle rather than persisting until confirmed; there is no native "review date" property at all), LOW support burden (notification/reporting only, no destructive bulk action), and a viable, still-open wedge angle (a per-owner consolidated digest, persistent until confirmed, available on Free/Standard tier — not explicitly claimed by any of the 4 existing tiny competitors' own descriptions).

**Stop condition NOT triggered:** Class 3 independently satisfies every required element (confirmed buyer, recurring/relevant problem, existing paid behavior, credible reason to pay, native gap, LOW/MEDIUM support burden, viable solo wedge) simultaneously, so `ATLASSIAN WEDGE SEARCH FAILED` does not apply. No fourth wedge was invented and Class 2 was not artificially rescued.

**Final 2 concrete wedges carried forward (no winner chosen by score):**

1. **Confluence Review Cadence Digest** (Class 3) — primary candidate: adds an Owner + Review Date property to Confluence pages (absent natively), sends one consolidated digest per owner per cycle instead of one email per page, persists until explicit confirmation, and works on Free/Standard tier (unlike native Automation).
2. **Jira Departure Sweep / Orphaned-Ownership Cleanup** (Class 1) — secondary candidate, explicitly flagged `NEEDS EVIDENCE`: daily/on-demand scan of deactivated users' owned filters/dashboards/issues/project-leads into a per-departed-owner work queue with bulk reassignment and an audit-ready export; requires proof that customers will actually pay before proceeding further, since neither direct competitor has any installs yet.

**Explicitly not done in this phase:** no winner chosen by numeric score, no code written, no MVP designed, no architecture designed, no new keyword sweep.

## 0.13 Phase J Output — Competition Gap Validation (2026-09-20)

Full evidence (corrected feature/scale profile of all 5 named competitors, gap-by-gap analysis against escalation/accountability/audit-evidence/cross-space/exceptions/SLA-enforcement) is in `RESEARCH.md` under "I. Phase J — Competition Gap Validation". This section records only the outcome. No new marketplace sweep was run; the problem class itself was not re-litigated (`Confluence stale/outdated content detection & review` remains `SURVIVES`, per user instruction); only the search for a surviving wedge *within* that class continued.

**Critical correction to Phase I:** deeper research revealed that **Better Content Archiving and Analytics for Confluence (Midori)** — treated in Phase I as a minor adjacent app mentioned in community threads — is actually the **dominant incumbent** in this space: **1,196 installs, 4.8/5 across 155 reviews**, Platinum Marketplace Partner, Cloud Fortified. It already does scheduled/event-triggered owner notifications, multi-owner management, auto-archiving, and space-level analytics — and a real customer review (Phil Sanford, 2025-04-11) confirms it is already used to send consolidated alerts to department heads, not per-page spam. This directly confirms the user's correction that `Review Cadence Digest` is `COLLIDED`, not a gap.

**Method:** re-profiled all 5 named competitors (Better Content Archiving, Page Review Manager, Evergreen, Stale Page Finder, Keep Docs Updated) on their actual confirmed feature sets, then checked 6 "beyond feature checklist" gap directions named in the brief (notification overload, escalation, accountability/audit evidence, cross-space governance, exceptions, SLA/deadline enforcement) against: customer evidence, coverage by the 5 named apps, coverage by other real (non-named) Atlassian Marketplace apps, and whether a customer would actually pay.

**Result — every gap direction failed on the same criterion (unmet job), for one of two reasons:**
- **Already solved by one of the 5 named apps directly:** cross-space governance (Better Content Archiving's space-level analytics; Keep Docs Updated's explicit "Monitor outdated pages across ALL spaces" Global View) and exceptions/never-expire overrides (Evergreen's per-space-and-per-page threshold override).
- **Already solved commercially by a different, real, active Atlassian Marketplace vendor** (not one of the 5, but real and confirmed): escalation-to-manager (Workflows for Confluence, AppFox — "escalation rules can send reminders or escalate to a manager"); version-locked review/approval evidence for audit purposes (ApprovalFlow for Confluence, and Compliance for Confluence / Workflows for Confluence marketed explicitly for ISO 27001/SOC 2 evidence assembly — a genuine, precisely-articulated gap was found here, "review 'completion' is typically a status label someone sets manually; there is no enforced record of who reviewed which version" (Flowdence, community, 2026-03-20), but it is already being actively sold into by named competitors in that adjacent category).
- **SLA/deadline enforcement (blocking access for overdue reviews, not just notifying)** is the one direction with no confirmed existing competitor among the 5 or elsewhere — but it also has **no direct customer evidence** requesting blocking/gating rather than reminders, so it was not promoted, per the project's standing rule against inventing an unmet job without customer evidence.

**Verdict: KILLED** — not for lack of pain (the problem class itself remains `SURVIVES`, unchanged per instruction) but because no specific unmet job survived scrutiny: every checked direction either collided with one of the 5 named apps or with a different real, active competitor already selling into that exact job on the same marketplace. No narrower wedge was artificially constructed to rescue the search.

**Practical consequence for the project's wedge pipeline:** of the 2 concrete wedges carried forward from Phase I (Section 0.12), the primary one (**Confluence Review Cadence Digest**) is now fully invalidated (`COLLIDED` → `KILLED` after deeper search for alternatives). The secondary one (**Jira Departure Sweep / Orphaned-Ownership Cleanup**, `NEEDS EVIDENCE`) is untouched by this phase, since Phase J was explicitly scoped only to the Confluence stale-content class. **This leaves exactly one live, unresolved candidate in the entire project: the Jira orphaned-ownership wedge**, still pending proof that customers will actually pay for it.

**Explicitly not done in this phase:** no MVP, no new marketplace/keyword sweep, no numeric scoring, no artificial rescue of the rejected wedge.

## 1. Target

**Marketplace:** Atlassian Marketplace (selected for Phase B deep research — see Section 0; not yet a BUILD target)

**Exact customer query / intent:** all 6 keyword-based intents researched across Phase C–G are closed (Sections 0.8, 0.10). Phase H's 3 operational-pain problem classes went through Pain/Switching/Wedge testing in Phase I (Section 0.12) and then Competition Gap Validation in Phase J (Section 0.13) for the one survivor: **Confluence stale/outdated content detection & review cadence — problem class still `SURVIVES`, but its proposed wedge (review-cadence digest) is `KILLED`** after deeper research showed the dominant incumbent (Better Content Archiving, 1,196 installs) and several other real, active Marketplace vendors already commercially serve every checked angle (escalation, audit-evidence, cross-space governance, exceptions). **Orphaned digital artifacts after user/project lifecycle events (Jira) remains `NEEDS EVIDENCE`** (untouched by Phase J, which was scoped only to the Confluence class). **Issue-level data quality/hygiene drift after creation (Jira) is `KILLED`** (Phase I).

**Candidate product:** none chosen — the only remaining live candidate is the Jira orphaned-ownership wedge (`NEEDS EVIDENCE`); the Confluence wedge is dead. No MVP or architecture designed for anything, per instruction not to pick a winner by score

**One-sentence wedge:** the only surviving candidate is a **Jira orphaned-ownership cleanup sweep** for departed users' filters/dashboards/issues/project-leads — real buyer (Jira Cloud admin), a native gap unaddressed for 7+ years, and a direct historical willingness-to-pay quote, but not yet proven because neither direct competitor has a single install; the Confluence review-cadence-digest candidate that looked strongest after Phase I has since been fully invalidated in Phase J

## 2. Hard Gates

| Gate | PASS / FAIL / UNKNOWN | Evidence |
|---|---|---|
| Marketplace commercial fit | PASS (Phase A, marketplace-level) | Atlassian processes payment + recurring billing end-to-end for Paid-via-Atlassian apps; RESEARCH.md A3 |
| Organic discovery via Marketplace search | EVIDENCED | Confirmed via live search test 2026-09-19: Rising Star apps rank #1/#1/#2 on 3 of 8 real queries. RESEARCH.md A3 → B0 |
| First-time unknown vendor success | UNKNOWN — NEEDS EVIDENCE | All 18 sampled Rising Star apps came from vendors with 2–17+ other marketplace apps already live; no true first-time single-app vendor example found, positive or negative. RESEARCH.md A3 → B0 |
| Company-email requirement (Paid via Atlassian) | UNKNOWN — CHECK PENDING | Atlassian requires a company-domain email for Paid-via-Atlassian apps (personal/generic domains not permitted). User's Gewerbe registration is a separate fact from having a company-domain email; not yet verified. RESEARCH.md A3 |
| Keyword opportunity | PARTIALLY EVIDENCED | 5 of 22 tested search intents classified PROMISING (or PROMISING-on-visibility); majority (16/22) are WEAK/REJECT/saturated-by-veterans. RESEARCH.md → Phase B1 |
| Demand validation (3 of 5 narrowed intents) | PARTIALLY EVIDENCED | 3 of 5 Phase B1 intents show real, dated, non-generic customer evidence (production use / regulatory outcomes / multi-year retention) at app level; 2 of 5 (`user access review`, `audit log confluence`) demoted to NEEDS EVIDENCE after app-level scrutiny — low competition alone was not treated as proof of demand. RESEARCH.md → Phase C |
| Repeated pain | EVIDENCED but not exclusive | Specific, dated pain found for both tested hypotheses, but each pain point is already being actively addressed by existing competitors, not left open. RESEARCH.md → Phase D, Phase E |
| Switching signal | Reclassified 2026-09-19 using A/B/C/D taxonomy (direct replacement / comparison-shopping / replacement intent / pain only) — see note above Section 1. No type-A competitor-to-competitor replacement found; closest signals are type B (comparison-shopping, HubSpot intent) and type A-against-native-tooling (analytics intent, now on HOLD). RESEARCH.md → Phase D | |
| **Clear wedge** | **FAIL (Confluence digest, killed in Phase J); NEEDS EVIDENCE (Jira orphaned-ownership, untouched by Phase J)** | Original 2 hypotheses killed in Phase E; Phase F's 3 replacements killed in Phase G. Phase H found 3 operational-pain problem classes; Phase I (Section 0.12) found 1 SURVIVES (Confluence stale-content/review-cadence), 1 NEEDS EVIDENCE (Jira orphaned-ownership), 1 KILLED (issue-level data quality drift). Phase J (Section 0.13) then killed the Confluence class's proposed wedge specifically — every checked gap direction (escalation, audit evidence, cross-space governance, exceptions) is already commercially served by the dominant incumbent (1,196 installs) or another real Marketplace vendor. The problem class itself stays `SURVIVES`; only its wedge is dead. RESEARCH.md → Phase E, Phase F, Phase G, Phase H, Phase I, Phase J |
| Solo feasibility | Only assessed for the one remaining candidate (Jira orphaned-ownership) | MEDIUM support burden (bulk reassignment carries mis-assignment risk), LOW API/policy risk (internal Jira REST/Forge data), HIGH Architecture Fit. Not yet proven — zero installs on both direct competitors. RESEARCH.md → Phase I |
| Support burden | MEDIUM (only remaining candidate) | RESEARCH.md → Phase I, Phase J |
| Native replacement risk | UNKNOWN | |
| Policy/API risk | UNKNOWN | |
| Dependency risk | UNKNOWN | |
| Monetization | UNKNOWN | |

## 3. Veto Rules

`FAIL` in any of these normally means `REJECT`:

- marketplace commercial fit;
- organic discovery evidence;
- clear wedge;
- solo feasibility.

A serious platform/policy dependency may also be a veto.

## 4. Funnel Hypothesis

`search/view → install → activation → payment`

**Expected first validation event:** 

**Unknowns still blocking BUILD:** 

## 5. Economics

**Proposed price:** UNKNOWN

**Customers for 3 payments:** UNKNOWN

**Customers for €100 MRR:** UNKNOWN

**Estimated support minutes/customer/month:** UNKNOWN

**Critical third-party costs:** UNKNOWN

## 6. Strongest Evidence

(Marketplace-selection evidence — see Section 0 for full detail and sources)

1. Atlassian is the only platform of the five screened with an official, named organic-newcomer-visibility mechanism ("Rising Star" badge).
2. Atlassian fully manages payment processing and recurring billing for Paid-via-Atlassian apps — no external payment dependency.
3. WordPress.org (the organically-discoverable WordPress surface) is confirmed, via official guidelines, to forbid paid/gated code — a structural commercial-fit failure, not an assumption.
4. Meta has no marketplace surface matching the discovery→install→pay model for a general SaaS app; Meta Horizon Store is a real marketplace but scoped to VR/AR apps and games.
5. The user's existing German Gewerbe reduces some solo-feasibility friction (a registered business exists), but the specific "Paid via Atlassian" company-email requirement is a separate, unverified `CHECK PENDING` — not resolved by Gewerbe alone.
6. Live cold-start validation (2026-09-19): organic discovery via Marketplace search is EVIDENCED — Rising Star apps ranked #1 on real customer search queries in 2 of 8 tests, and #2 in a third. First-time unknown vendor success remains UNKNOWN — no sampled example was a true first-time single-app vendor (see Section 0 for the scoped gap).

## 7. Main Risks

1. 
2. 
3. 

## 8. Stop-Loss / Next Experiment

**Current bottleneck:** 

**Next cheapest test:** 

**Kill/pivot condition:** 

## 9. Final Decision

Choose exactly one:

- `BUILD`
- `REJECT`
- `NEEDS EVIDENCE`

**Decision:** `NEEDS EVIDENCE`

**Reason:** Phase A/B0 selected Atlassian Marketplace (Section 0). Phase B1→C→D→E killed both surviving keyword-based wedges (Section 0.8); Phase F's 3 replacements were killed in Phase G (Section 0.10). Phase H (Section 0.11) discovered 3 operational-pain problem classes by working backward from real 2026 Marketplace apps. Phase I (Section 0.12) ran Pain/Switching/Wedge testing on those 3, sourcing 30 dated customer quotes, and found 1 SURVIVES (Confluence stale-content/review-cadence), 1 NEEDS EVIDENCE (Jira orphaned-ownership), 1 KILLED (issue data quality drift). Phase J (Section 0.13) then took the one survivor and went deeper: comparing it against all 5 of its named direct competitors plus real adjacent Marketplace vendors, specifically hunting for an unmet job beyond the already-rejected "daily digest" idea (escalation, accountability/audit evidence, cross-space governance, exceptions, SLA enforcement). **Every direction checked was already commercially solved** — either by one of the 5 named competitors directly (cross-space governance, per-page exceptions), or by a different real, active Marketplace vendor selling into the exact same job (Workflows for Confluence for escalation; ApprovalFlow for Confluence / Compliance for Confluence for version-locked audit evidence) — and the one direction with no existing competitor (blocking access for overdue reviews) had no supporting customer evidence either, so it was not promoted. **Result: the Confluence wedge is now `KILLED`, even though the underlying problem class remains `SURVIVES`** — real pain exists, but no defensible, un-served product wedge does. This leaves exactly **one live, unresolved candidate in the whole project**: the Jira orphaned-ownership cleanup sweep (`NEEDS EVIDENCE`, Section 0.12) — a real buyer, a 7-year-unaddressed native gap, and a direct willingness-to-pay quote, but zero installs on either of its two direct competitors, so payment is not yet proven. The stop condition (`ATLASSIAN WEDGE SEARCH FAILED`) does not apply — a live, evidence-backed (if unproven) candidate still exists, so the search is not exhausted. This stays `NEEDS EVIDENCE` rather than `BUILD` or `REJECT`: not `BUILD` because the sole remaining candidate has no proof customers will pay and has not been scoped into an MVP; not `REJECT` because the marketplace itself (Section 0) is unaffected and one candidate with real (if incomplete) evidence is still alive. The next step, not yet started, is resolving that one open question — proof of willingness to pay for the Jira orphaned-ownership wedge — not inventing a new candidate to replace the just-killed Confluence one.
