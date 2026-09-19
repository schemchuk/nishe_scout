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

## 1. Target

**Marketplace:** Atlassian Marketplace (selected for Phase B deep research — see Section 0; not yet a BUILD target)

**Exact customer query / intent:** narrowed to 3 candidates in Phase C (see Section 0.6): `gdpr compliance confluence`, `confluence page views analytics`, `hubspot integration jira` — not yet narrowed to one; Phase D (Pain + Switching) is next

**Candidate product:** not yet researched — Phase C/D

**One-sentence wedge:** not yet researched — Phase E

## 2. Hard Gates

| Gate | PASS / FAIL / UNKNOWN | Evidence |
|---|---|---|
| Marketplace commercial fit | PASS (Phase A, marketplace-level) | Atlassian processes payment + recurring billing end-to-end for Paid-via-Atlassian apps; RESEARCH.md A3 |
| Organic discovery via Marketplace search | EVIDENCED | Confirmed via live search test 2026-09-19: Rising Star apps rank #1/#1/#2 on 3 of 8 real queries. RESEARCH.md A3 → B0 |
| First-time unknown vendor success | UNKNOWN — NEEDS EVIDENCE | All 18 sampled Rising Star apps came from vendors with 2–17+ other marketplace apps already live; no true first-time single-app vendor example found, positive or negative. RESEARCH.md A3 → B0 |
| Company-email requirement (Paid via Atlassian) | UNKNOWN — CHECK PENDING | Atlassian requires a company-domain email for Paid-via-Atlassian apps (personal/generic domains not permitted). User's Gewerbe registration is a separate fact from having a company-domain email; not yet verified. RESEARCH.md A3 |
| Keyword opportunity | PARTIALLY EVIDENCED | 5 of 22 tested search intents classified PROMISING (or PROMISING-on-visibility); majority (16/22) are WEAK/REJECT/saturated-by-veterans. RESEARCH.md → Phase B1 |
| Demand validation (3 of 5 narrowed intents) | PARTIALLY EVIDENCED | 3 of 5 Phase B1 intents show real, dated, non-generic customer evidence (production use / regulatory outcomes / multi-year retention) at app level; 2 of 5 (`user access review`, `audit log confluence`) demoted to NEEDS EVIDENCE after app-level scrutiny — low competition alone was not treated as proof of demand. RESEARCH.md → Phase C |
| Repeated pain | UNKNOWN | |
| Switching signal | UNKNOWN — some switching language surfaced incidentally in Phase C reviews (e.g. Multiplier vs. IdP alternatives) but not yet systematically researched | |
| Clear wedge | UNKNOWN | |
| Solo feasibility | UNKNOWN | |
| Support burden | UNKNOWN | |
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

**Reason:** Phase A (marketplace screening) and Phase B0 (cold-start validation) are complete — Atlassian Marketplace is selected (see Section 0). Phase B1 (search landscape) is complete — 5 candidate search intents selected (see Section 0.5). Phase C (demand validation) is complete — 3 of those 5 intents (`gdpr compliance confluence`, `confluence page views analytics`, `hubspot integration jira`) show real app-level demand evidence and carry forward to Phase D; the other 2 were demoted to NEEDS EVIDENCE after app-level scrutiny (see Section 0.6). No product has been chosen. No BUILD decision may be made until pain/switching evidence (Phase D) and a concrete wedge (Phase E) are established for one specific candidate product on Atlassian Marketplace.
