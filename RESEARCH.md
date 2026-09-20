# Research — Niche Scout

**Research date:** 2026-09-18  
**Status:** PHASE A COMPLETE (marketplace screening) — Phase B (deep keyword research) not started.  
**Rule:** external claims require URL + verification date.

## A. Marketplace screening

### A1. Wix

**Verdict: NEEDS EVIDENCE (weak PASS on structure, no confirmed new-entrant traction)**

**Search/discovery.** Real customer-facing search and category browsing exists at wix.com/app-market (verified 2026-09-18). No official Wix document was found that discloses the ranking algorithm/signals (unlike Atlassian, Shopify, WordPress, which all publish at least partial ranking factors). This is a genuine gap: `RANKING SIGNALS — UNKNOWN — NEEDS EVIDENCE`.

**Commercial fit — PASS.** Confirmed directly from official docs (fetched 2026-09-18):
- Wix processes all payments; developer sets price, Wix billing/checkout handles the rest. Source: https://dev.wix.com/docs/build-apps/launch-your-app/pricing-and-billing/about-monetizing-your-app
- Revenue share: 100% of revenue in year 1, 80% after, calculated after a 2.5% transaction fee + tax. Payout on a net-30 EOM basis. Same source.
- All apps that collect money for any purpose (incl. donations) **must** use the Wix Billing System — no external checkout allowed. Source: https://dev.wix.com/docs/build-apps/launch-your-app/app-distribution/app-market-guidelines (fetched 2026-09-18).
- This means billing is fully platform-managed — no external payment dependency required.

**Platform/compliance risk.** App Market Guidelines (same URL, fetched in full 2026-09-18) require: a live demo account for review, HTTPS/SSL, OWASP-level security (salted password hashes, CSRF/XSS protection), GDPR compliance, PCI-DSS/PA-DSS compliance if handling payment data. **No KYC/KYB or company-entity requirement was found** in the guidelines — this is lighter than Atlassian's process. No published approval-time SLA was found (`APPROVAL TIMELINE — UNKNOWN — NEEDS EVIDENCE`).

**New entrant evidence — UNKNOWN — NEEDS EVIDENCE.** Multiple searches (2026-09-18) did not surface any named example of a Wix app launched in the last ~12 months with public reviews/ratings/traction. Secondary sources describe the market as "crowded" and stress marketing effort is needed, but this is marketing-blog commentary, not verifiable adoption evidence. **This claim needs direct verification against the live App Market (sort-by-newest) in Phase B if Wix is revisited.**

**Organic-entry proof — PARTIAL / UNVERIFIED.** Catalog size is small relative to competitors: secondary sources (magecomp.com, sqmagazine.co.uk, wix.com/app-market marketing page — not an official count endpoint, checked 2026-09-18) state **500–800 apps total**, versus Shopify's ~18,000+ and WordPress's ~73,000+. Fewer apps per category is a plausible reason for easier visibility, but **no evidence was found that this actually converts into new-app organic traction** — the causal claim "Wix легший через малу кількість apps" is **not confirmed**, only the raw app-count fact is confirmed. Label: `UNKNOWN — NEEDS EVIDENCE` on the causal claim.

Official sources used:
- https://dev.wix.com/docs/build-apps/launch-your-app/pricing-and-billing/about-monetizing-your-app (checked 2026-09-18)
- https://dev.wix.com/docs/build-apps/launch-your-app/app-distribution/app-market-guidelines (checked 2026-09-18, fetched in full)
- https://www.wix.com/app-market (checked 2026-09-18, marketing page, catalog size claim only)

### A2. Shopify

**Verdict: PASS candidate (strongest solo-feasibility evidence; organic discovery is real but slow, not free)**

**Search/discovery.** Real customer-facing search + categories at apps.shopify.com. Shopify has published partial official ranking info: since Feb 27 2023, search folds in **post-search merchant engagement data** (what merchants click/install after searching), reducing the weight of pure keyword-stuffing. Source (secondary, summarizing an official Shopify changelog/blog — https://www.shopify.com/partners/blog/search-improvements, checked 2026-09-18; full algorithm is proprietary and not fully documented). **Built for Shopify** badge gives a documented **ranking/placement boost** but requires an *existing* track record of installs/reviews/ratings to qualify — source: https://shopify.dev/docs/apps/launch/built-for-shopify (fetched in full 2026-09-18). So the boost is not available to a brand-new app.

**Commercial fit — PASS, well documented.** Confirmed from official docs (fetched 2026-09-18, https://shopify.dev/docs/apps/launch/billing and https://shopify.dev/docs/apps/launch/distribution/revenue-share):
- Shopify processes billing; charges are added directly to the merchant's Shopify invoice. All paid apps published in the App Store **must** use a Shopify-provided billing solution (Shopify App Pricing or the Billing API) — no external payment gateway needed.
- Revenue share: developers keep **100% of gross app revenue up to $1,000,000 USD lifetime**, then 85% above that (Shopify keeps 15%). One-time $19 USD Partner registration fee. 2.9% processing fee + tax applies to billing.
- This is the most generous revenue-share term found among all candidates for a developer under $1M lifetime revenue.

**New entrant evidence — PASS (volume), MIXED (traction).**
- App catalog grew from **~12,320 apps (Jan 2025)** to **~18,368 apps (May 2026)** per aggregator sources (meetanshi.com, appjubilee.io — secondary, checked 2026-09-18, not an official Shopify count) — i.e., thousands of new listings within the study window, confirming new entrants exist at scale.
- Direct friction evidence for *organic ranking* specifically (secondary/community sources, checked 2026-09-18): a developer documented their new compliance app ranking **below position 96** on relevant search terms after two weeks despite a solid listing and zero installs (https://dev.to/lawebe/shopify-app-store-ranking-what-day-14-of-a-new-compliance-app-launch-actually-looks-like-li4); community analysis states new apps typically need **10+ reviews within the first 30 days** to gain traction (https://community.shopify.dev/t/reading-page-one-of-50-app-store-searches-the-ranking-pattern-title-carries-it-not-reviews/37411). These are developer/community-voice sources, not Shopify official statements, and should be read as customer/practitioner evidence, not policy.
- Counter-evidence that organic-only growth *does* eventually work without paid ads: multiple bootstrapped solo/small-team founders on Indie Hackers (checked 2026-09-18) report reaching real MRR primarily through organic App Store traffic and word-of-mouth, explicitly stating paid ads "never saw traction" for them (https://www.indiehackers.com/post/i-bootstrapped-a-shopify-app-to-78k-cad-mrr-in-3-years-ask-me-anything-5fbbc2b886, https://www.indiehackers.com/post/tech/getting-out-of-the-freelancing-game-by-building-a-100k-mrr-shopify-app-portfolio-qdReVAgLjz6EpW4OrJSI). This is community/self-reported evidence (not independently verifiable installs), but it is a repeated pattern across independent posts, which is the standard this project asks for.

**Verifying the claim "Shopify органічно недоступний новому app":** **NOT CONFIRMED as an absolute.** Evidence shows a real cold-start period (new apps rank poorly with zero reviews, no boost mechanism exists for brand-new apps), but it is not evidence of zero organic path — it is evidence of a *slow, review-dependent* organic path that does not require *paid* acquisition, though it does require sourcing initial reviewers somehow (existing network, communities) which is a genuine planning constraint, not a hard veto.

**Platform/compliance risk.** As of April 1, 2025, all new public apps must use the GraphQL Admin API exclusively (REST Admin API being sunset for new apps) — a real, dated technical/maintenance requirement (secondary source summarizing Shopify dev requirements, checked 2026-09-18; should be confirmed against https://shopify.dev/changelog directly before build). Review process: official docs describe a multi-stage automated + manual review; secondary sources report **5–14 business days** typical, with some outlier cases of 3+ weeks (checked 2026-09-18, not independently confirmed against an official SLA page).

**Solo feasibility — PASS, best-evidenced of all candidates.** No KYC/company-entity requirement found. Large number of publicly documented solo/small-team founders running Shopify apps profitably (Indie Hackers AMAs cited above, plus https://www.indiehackers.com/post/bootstrapped-a-shopify-app-to-500-paying-clients-with-an-mvp-ama-7dbaf8084e, checked 2026-09-18).

Official sources used:
- https://shopify.dev/docs/apps/launch/billing (fetched in full 2026-09-18)
- https://shopify.dev/docs/apps/launch/distribution/revenue-share (fetched in full 2026-09-18)
- https://shopify.dev/docs/apps/launch/built-for-shopify (fetched in full 2026-09-18)
- https://shopify.dev/docs/apps/launch/marketing (checked 2026-09-18, not fully fetched)

Secondary/community sources (customer/practitioner voice, not policy):
- https://dev.to/lawebe/shopify-app-store-ranking-what-day-14-of-a-new-compliance-app-launch-actually-looks-like-li4 (checked 2026-09-18)
- https://community.shopify.dev/t/reading-page-one-of-50-app-store-searches-the-ranking-pattern-title-carries-it-not-reviews/37411 (checked 2026-09-18)
- https://www.indiehackers.com/post/i-bootstrapped-a-shopify-app-to-78k-cad-mrr-in-3-years-ask-me-anything-5fbbc2b886 (checked 2026-09-18)
- https://www.indiehackers.com/post/we-got-our-shopify-app-approved-in-72-days-now-were-stuck-at-distribution-and-people-keep-offering-us-paid-reviews-df8505401d (checked 2026-09-18)

### A3. Atlassian

**Verdict: PASS candidate — strongest organic-newcomer mechanism found; compliance overhead is real, and one specific sub-requirement (company-domain email) remains an open CHECK PENDING regardless of Gewerbe status**

**Search/discovery — PASS, best documented.** Official page (fetched in full 2026-09-18: https://developer.atlassian.com/platform/marketplace/marketplace-search-results-and-rankings/) names three explicit ranking factors: (1) keyword relevance in name/tagline/description, (2) semantic matching (vector-based, understands intent not just exact words), (3) engagement score (reviews, ratings, installs, support responsiveness). Backend migrated from Algolia to OpenSearch during H1 2026 (same page).
- **New-entrant-specific mechanism found:** Atlassian's community/ecosystem articles describe a **badge system — "Spotlight" (top apps), "Rising Star" (newer apps gaining traction), "Bestseller"** — specifically designed to give visibility to apps that are new but gaining momentum, not just to established leaders. Source: https://community.atlassian.com/forums/App-Central-articles/Same-Top-Searches-a-Different-Marketplace-What-s-Changed-for-App/ba-p/3247062 (Atlassian Community "App Central" article, checked 2026-09-18 — semi-official, written by Atlassian ecosystem staff, not third-party). **This is the only explicit, named organic-newcomer-visibility mechanism found across all four platforms studied.**

**Commercial fit — PASS, fully platform-managed for "Paid via Atlassian" apps.** Official page (fetched in full 2026-09-18: https://developer.atlassian.com/platform/marketplace/pricing-payment-and-billing/):
- Atlassian processes payment and handles recurring billing end-to-end for "Paid via Atlassian" apps (monthly/annual). No external payment processor required.
- Revenue share: Forge apps 84% to developer (effective April 1, 2026); new Forge apps get 95%/100% promotional share in year 1 up to $1M lifetime Forge revenue; Connect apps' developer share is being reduced from 85%→80%→75% through 2026 (i.e., Atlassian's cut is rising for the older Connect architecture — a real, dated policy change worth tracking) — source: https://www.atlassian.com/blog/development/updates-to-marketplace-revenue-share-2026 (checked 2026-09-18, official Atlassian blog).
- Payout threshold $500, paid 30–60 days after sale.

**Platform/compliance risk — real but largely one-time, not recurring, for this specific user.** Official approval guidelines (fetched in full 2026-09-18: https://developer.atlassian.com/platform/marketplace/app-approval-guidelines/):
- Approval takes 10–15 business days.
- KYC/KYB verification via a third-party vendor is mandatory for all partners.
- **Paid-via-Atlassian apps require a company email domain — personal domains (Gmail, etc.) are explicitly not permitted.**
- A partner security questionnaire (security practices, infrastructure, vulnerability management) is required, plus a per-app security review for new apps.

**Important reframing of "Atlassian занадто складний для solo" — corrected 2026-09-19, do not overstate:** the claim is **not fully confirmed nor fully refuted**. Two distinct sub-requirements must not be conflated:
- **KYC/KYB (business-entity verification):** having a registered German business (Gewerbe, per `CONTEXT.md`) plausibly helps satisfy a "this is a real company" check, but this has **not been directly verified** against Atlassian's actual KYC/KYB vendor-onboarding process — `CHECK PENDING`.
- **Company-domain email for "Paid via Atlassian" apps:** Atlassian's guidelines explicitly require a company email domain and explicitly reject personal/generic domains (Gmail, Yahoo, etc.). Owning a Gewerbe does **not** automatically mean a company-domain email exists or is in use — these are separate facts. This is a distinct, unverified `CHECK PENDING`, not something Gewerbe resolves by itself.
- What remains independently **CONFIRMED as real overhead**, regardless of entity/email status, is the **security questionnaire and per-app security review** — recurring-per-app friction not found on Wix or WordPress, and heavier than Shopify's automated+manual review.
- **Verdict on the claim: NEEDS EVIDENCE overall** — the entity/email sub-requirements are open CHECK PENDING items (not resolved, not proven blocking), while the security-review overhead sub-claim is CONFIRMED as real and above Wix/WordPress/Shopify level.

**New entrant evidence — RESOLVED 2026-09-19 (see B0 below): CONFIRMED with an important caveat.** Marketplace has grown to **7,210 apps (Oct 2025)** to **8,000+ apps (2025)** with **1,800+ active vendors**, per secondary aggregator sources (appmarketplace.com, aventis-advisors.com — checked 2026-09-18, not an official Atlassian count page).

### B0. Cold-start validation follow-up (2026-09-19)

This directly closes the gap flagged above. Method: (1) read the live Rising Star collection page in full, (2) opened individual app and vendor pages for the apps found there, (3) ran 8 real customer-style marketplace search queries and recorded whether Rising Star apps actually appear in the organic results (not just the curated collection page). All data pulled live from marketplace.atlassian.com on 2026-09-19; figures (ratings, review counts, install counts) are live and will drift over time — re-check before relying on exact numbers.

**Source:** https://marketplace.atlassian.com/collections/rising-star (checked 2026-09-19, live page, "Showing 30 apps").

**Step 1 — 18 Rising Star apps sampled from the live collection (exceeds the requested 10–15):**

| App | Vendor | Rating | Reviews | Installs |
|---|---|---|---|---|
| SprintPoker – Planning Poker & Async Estimation | Agile Pulse | 5/5 | 22 | 669 |
| SnapMetrics – Real Time Analytics | Snapbytes | 5/5 | 13 | 189 |
| SprintRetro Pro | Agile Pulse | 5/5 | 15 | 602 |
| Dashboard Templates, Charts, Graphs & Reports for Jira | Clovity | 5/5 | 6 | 234 |
| Time Tracking, Resource Planning & PM | Clovity | 5/5 | 7 | 214 |
| TimeEase | OptimalSDLC | 5/5 | 6 | 280 |
| Task Reports for Jira | Meetical | 4.9/5 | 9 | 688 |
| Content Formatting Macros | Clovity | 5/5 | 6 | 203 |
| WIP Aging Reports & Run Charts | Broken Build | 5/5 | 6 | 697 |
| Throughput Charts | Broken Build | 5/5 | 5 | 731 |
| Agile Velocity & Sprint Status Gadgets | RVS Softek | 4.8/5 | 5 | 762 |
| Apportunity: Mermaid Diagrams Macro | Apportunity | 3.8/5 | 4 | 475 |
| Monte Carlo Simulations & Capacity Planning | Broken Build | 5/5 | 4 | 747 |
| SnapAssign – Smart Assignments for Jira | Snapbytes | 5/5 | 11 | 61 |
| Created vs Resolved charts | Broken Build | 5/5 | 3 | 702 |
| Script Master for Jira | Apportunity | 4.8/5 | 6 | 281 |
| Issue History for Jira | votazz | 5/5 | 1 | 635 |
| Issue (Work Item) Templates for Jira | Achlys Solutions | 5/5 | 4 | 192 |

All install counts are low relative to established marketplace apps (hundreds vs. thousands/tens of thousands) — consistent with these being genuinely young listings by marketplace standards.

**Critical finding — every Rising Star app checked belongs to a multi-app vendor, not a solo first-time debut:**
- **Agile Pulse** (vendor page, checked 2026-09-19): 8 apps in the marketplace. SprintPoker's own listing states it is "created as the premium successor to Planning Poker Agility... trusted by 3,000+ organizations" — Agile Pulse's own free app with 3.3k installs / 76 reviews. The Rising Star app is a paid upsell cross-promoted to an existing user base, not a cold-start product.
- **Snapbytes** (vendor page, checked 2026-09-19): describes itself as "one of the first Atlassian Marketplace Partners," 4 apps, offices in Istanbul and Cambridge — an established company, not a newcomer.
- **votazz** (vendor page, checked 2026-09-19): 17+ apps; lists Apple, NVIDIA, Sony, Daimler, Philips, EA, VMware, DBS Bank as customers of its portfolio. Its Rising Star app's documentation is hosted under "rvsoftwares.atlassian.net," linking it to RVS Softek (also has a separate Rising Star app in this sample) — a large, experienced dev shop operating under multiple brand names.
- **Broken Build** (vendor page, checked 2026-09-19): explicitly an "Atlassian Gold Marketplace Partner trusted by 2,000+ customers," 15+ apps, SOC 2 Type 2, own Trust Center — 4 of its apps carry the Rising Star badge, alongside older apps in the same portfolio with 1,000–2,200+ installs.
- **Achlys Solutions**, **Apportunity**, **Clovity**: all multi-app portfolios (7, 3, and 3+ apps respectively); Clovity self-describes as an "Atlassian Platinum Solution Partner" doing enterprise digital-transformation consulting.
- **No example was found, across all 18 sampled apps, of a Rising Star badge going to a single-app vendor with no other marketplace presence, no existing trust-center/security-questionnaire infrastructure, and no existing customer base to cross-promote to.**

**Step 2 — 8 real customer search queries, checking whether Rising Star apps surface in organic search (not just the curated collection page):**

| Query | Total matches | Rising Star app(s) found | Position on page 1 |
|---|---|---|---|
| "planning poker" | 1,000+ | SprintPoker (Agile Pulse) | #3, above two Appfire apps with 45–110 reviews but below Appfire's top app (134 reviews, 3.6k installs) |
| "time tracking" | 1,000+ | **None found** in the ~17 visible results | — most competitive query tested; dominated by apps with 1,000–27,000 installs |
| "sprint retrospective" | 672 | SprintRetro Pro (Agile Pulse); SprintPoker (Agile Pulse); Agile Velocity Gadgets (RVS Softek) | SprintRetro Pro at **#2** |
| "issue templates" | 1,000+ | Issue (Work Item) Templates for Jira (Achlys Solutions) | ~#15 of visible results, below several apps with 1,000–4,600 installs |
| "smart assignment" | 915 | SnapAssign (Snapbytes) | **#1** |
| "mermaid diagrams" | 307 | Apportunity: Mermaid Diagrams Macro | ~#8, below a Bestseller app with 6.4k installs |
| "jira backup" | 1,000+ | ProBackup (ProBackup) | ~#4 |
| "real time analytics" | 1,000+ | SnapMetrics (Snapbytes) | **#1** |

Source for all 8 queries: https://marketplace.atlassian.com/search?query=... (live searches, checked 2026-09-19).

**Interpretation — separating organic discovery evidence from mere existence of the Rising Star program:**

1. **Organic discovery is real, not just an editorial artifact.** Rising Star apps appeared in genuine keyword search results (not only on the curated `/collections/rising-star` page) in **7 of 8 queries**, including **two #1 placements** and one **#2 placement**, ahead of apps with far more reviews/installs. This confirms the search algorithm (RESEARCH.md A3: keyword relevance + semantic match + engagement score) does surface newer/smaller apps in practice, not merely in Atlassian's own promotional collection — a materially stronger organic-discovery signal than was available before this check.
2. **Discovery strength is category-dependent.** In the single most saturated, generic category tested ("time tracking" — dozens of apps with 1,000–27,000 installs), no Rising Star app broke into the visible top results. Niche/specific queries ("smart assignment," "real time analytics," "sprint retrospective") showed far better placement than broad/generic ones. This matches the general pattern expected for a long-tail wedge strategy (CONTEXT.md's own guidance to target specific customer intent, not broad categories).
3. **Two separate claims, stated explicitly and not merged:**
   - **Organic discovery via Marketplace search: EVIDENCED.** The mechanism above (point 1) is a directly observed, repeatable property of live search results.
   - **First-time unknown vendor success: UNKNOWN.** Every single Rising Star example found is a new app from a vendor that already has other live apps, existing trust-center/security-questionnaire infrastructure, and in at least one case (Agile Pulse) an existing free product with thousands of installs to cross-promote into the paid one. No evidence was found — positive or negative — for how a genuinely first-time, single-app, unknown vendor performs, because no such example appeared in this sample. Mark `NEEDS EVIDENCE`, not `CONFIRMED IMPOSSIBLE` and not `CONFIRMED POSSIBLE`: CONTEXT.md's own rule against treating an absence as proof applies in both directions.
   - **On the trust-building infrastructure (security questionnaire, published docs, demo account, EULA):** this was **observed among all 18 sampled Rising Star vendors** — it is a correlation, not a demonstrated causal requirement. Whether it is necessary for reaching similar placement, or merely typical of established multi-app vendors for unrelated reasons, is **unknown**. Do not describe it as "table stakes" or a requirement without further evidence.

Official/primary sources used for B0 (all checked 2026-09-19, live marketplace pages, not secondary commentary):
- https://marketplace.atlassian.com/collections/rising-star
- https://marketplace.atlassian.com/apps/1143291390/sprintpoker-planning-poker-async-estimation
- https://marketplace.atlassian.com/apps/1235482/snapassign-smart-assignments-for-jira
- https://marketplace.atlassian.com/apps/1231436/issue-history-for-jira
- https://marketplace.atlassian.com/apps/1233958/script-master-for-jira
- https://marketplace.atlassian.com/vendors/1225397/agile-pulse
- https://marketplace.atlassian.com/vendors/1227191/snapbytes
- https://marketplace.atlassian.com/vendors/1219338/votazz
- https://marketplace.atlassian.com/vendors/1210856/broken-build
- https://marketplace.atlassian.com/vendors/1226033/achlys-solutions
- https://marketplace.atlassian.com/search?query=planning+poker
- https://marketplace.atlassian.com/search?query=time+tracking
- https://marketplace.atlassian.com/search?query=sprint+retrospective
- https://marketplace.atlassian.com/search?query=issue+templates
- https://marketplace.atlassian.com/search?query=smart+assignment
- https://marketplace.atlassian.com/search?query=mermaid+diagrams
- https://marketplace.atlassian.com/search?query=jira+backup
- https://marketplace.atlassian.com/search?query=real+time+analytics

Prior official sources (A3, 2026-09-18):
- https://developer.atlassian.com/platform/marketplace/marketplace-search-results-and-rankings/ (fetched in full 2026-09-18)
- https://developer.atlassian.com/platform/marketplace/pricing-payment-and-billing/ (fetched in full 2026-09-18)
- https://developer.atlassian.com/platform/marketplace/app-approval-guidelines/ (fetched in full 2026-09-18)
- https://www.atlassian.com/blog/development/updates-to-marketplace-revenue-share-2026 (checked 2026-09-18)
- https://community.atlassian.com/forums/App-Central-articles/Same-Top-Searches-a-Different-Marketplace-What-s-Changed-for-App/ba-p/3247062 (checked 2026-09-18)

### A4. WordPress

**Verdict: REJECT for the wordpress.org discovery surface — confirmed structural billing mismatch. WordPress.com Marketplace is a separate surface with billing but unverified reach/new-entrant evidence.**

**This is two different marketplaces, and conflating them is the main risk of a shallow read:**

**(1) wordpress.org plugin directory — the big, organically-discoverable one.**
- Search/discovery — PASS structurally. Official handbook + community sources (checked 2026-09-18) describe a two-phase ElasticSearch-based system: a relevance score (keyword coverage in readme/metadata) and a quality score (active installs, support-thread responsiveness, rating, freshness, compatibility).
- Catalog: ~60,300–73,588 plugins depending on snapshot date (secondary aggregator sources, checked 2026-09-18, not an official WordPress.org count endpoint). New submissions: **6,086 new plugins added in 2025**, **12,713 plugins reviewed in 2025 (69.5% approval rate, up from 63.4% in 2024)** — this figure IS official, from the WordPress.org Plugin Review team's own blog: https://make.wordpress.org/plugins/2026/01/07/a-year-in-the-plugins-team-2025/ and https://make.wordpress.org/plugins/2025/05/21/the-wordpress-ecosystem-is-growing-new-plugin-submissions-have-doubled-in-2025/ (both checked 2026-09-18). This confirms new entrants exist at real volume.
- **Commercial fit — CONFIRMED FAIL.** Official Plugin Directory guidelines (checked 2026-09-18: https://developer.wordpress.org/plugins/wordpress-org/, https://developer.wordpress.org/plugins/wordpress-org/detailed-plugin-guidelines/, https://github.com/WordPress/wporg-plugin-guidelines) state the plugin hosted on wordpress.org **must be fully functional on its own and cannot contain locked, disabled, or paywalled code.** A paid "Pro" tier must be sold as a **separate product outside wordpress.org** (own site, Stripe, Gumroad, Lemon Squeezy, etc.). **This means wordpress.org — the surface with real organic search/discovery — has no marketplace-managed or platform-native billing at all.** This directly fails CONTEXT.md's Marketplace Gate requirement ("платформа підтримує marketplace-managed або platform-native billing для релевантної моделі").
- Organic-entry for *brand-new* plugins specifically: secondary/practitioner sources (checked 2026-09-18) state the search algorithm favors plugins with existing installs/ratings, and new plugins can "languish on page 10." No confirmed example of a brand-new (≤12 months old), previously-unknown plugin achieving strong organic traction was found in this pass — one commonly-cited growth example ("Accessibility Checker," doubling installs from 4,000 to 10,000 in 7 months) is a **5-year-old plugin**, not a new entrant, so it does not count as new-entrant evidence.

**(2) WordPress.com Marketplace — has billing, different (and much narrower) reach.**
- Official docs (fetched in full 2026-09-18: https://developer.wordpress.com/docs/wordpress-com-marketplace/wordpress-com-store-saas-billing-flow/) confirm a real SaaS billing flow: customer discovers a listing on the WordPress.com Store, vendor creates a billing intent via API, WordPress.com hosts checkout, webhook confirms purchase. **WordPress.com is the merchant of record and processes payment** — this is genuinely platform-managed billing.
- However, this surface only reaches **WordPress.com-hosted site owners**, a small fraction of the ~810M+ total WordPress installs (most of which are self-hosted and use wordpress.org). No new-entrant traction evidence (reviews, ratings, listing dates) was found for this specific marketplace in this research pass — `NEEDS EVIDENCE`.

**Verifying the claim "WordPress не відповідає commercial model":** **CONFIRMED for wordpress.org** (the surface with actual organic search/discovery) — this is not an assumption, it is a direct reading of the official plugin-directory guidelines. **NOT CONFIRMED for WordPress.com Marketplace**, which does fit the billing requirement but has unverified discovery reach — flagged `NEEDS EVIDENCE` rather than assumed to fail.

Official sources used:
- https://developer.wordpress.org/plugins/wordpress-org/ (checked 2026-09-18)
- https://developer.wordpress.org/plugins/wordpress-org/detailed-plugin-guidelines/ (checked 2026-09-18)
- https://github.com/WordPress/wporg-plugin-guidelines (checked 2026-09-18)
- https://make.wordpress.org/plugins/2026/01/07/a-year-in-the-plugins-team-2025/ (checked 2026-09-18)
- https://make.wordpress.org/plugins/2025/05/21/the-wordpress-ecosystem-is-growing-new-plugin-submissions-have-doubled-in-2025/ (checked 2026-09-18)
- https://developer.wordpress.com/docs/wordpress-com-marketplace/wordpress-com-store-saas-billing-flow/ (fetched in full 2026-09-18)

### A5. Meta (added per current screening request — not in original candidate list)

**Verdict: REJECT — no marketplace surface fits the discovery→install→pay model for a general solo-built app.**

Three Meta surfaces were checked to see if any resembles Wix/Shopify/Atlassian/WordPress:

1. **Meta Business Partner Directory** (https://www.facebook.com/business/partner-directory, checked 2026-09-18) — this is a **directory of certified agencies/service companies** (Marketing Partners, Messaging Technology Partners, Advertising Technology Partners), not a customer-facing app catalog with search → install → in-marketplace payment. It is a B2B lead-gen listing, structurally closer to a consultants directory than an app store. **No customer-facing install/billing flow exists here.**
2. **Meta Business Suite "available apps"** — a curated set of Meta's own and select named integrations that admins connect via account credentials, not an open, developer-submittable marketplace with public search/reviews/ratings. Could not confirm (page content not retrievable in this session, checked 2026-09-18) any mechanism for an independent solo developer to list a new app here for public discovery.
3. **Meta Horizon Store** (Quest/VR app store) — this IS a real marketplace with customer-facing search, reviews, ratings, and platform-managed billing (Meta Horizon OS Developer docs, https://developers.meta.com/horizon/, checked 2026-09-18; https://en.wikipedia.org/wiki/Meta_Horizon_Store, checked 2026-09-18). However:
   - It is scoped to **VR/AR hardware apps and games**, not general web/business SaaS — a structural product-category mismatch with "micro-SaaS app in a website/business-tool marketplace."
   - Discovery is documented as a pain point even for existing developers: a 2024 developer-community piece describes the suggestion system surfacing low-quality high-budget content over "little gems made by indies," with sales reportedly dropping after the store opened up (https://skarredghost.com/2024/11/11/meta-quest-store-developers-problems/, checked 2026-09-18 — developer/customer-voice source, not official policy).
   - A solo-dev success example exists in a narrow case (a file-manager app filling a content gap — https://developers.meta.com/horizon/discover/success-stories/an-explorer/, checked 2026-09-18) but this is one anecdote in a fundamentally different product category (utility app for a niche hardware audience), not a transferable pattern for web-based B2B SaaS.

**Conclusion:** unlike Wix/Shopify/Atlassian/WordPress, Meta does not have a marketplace where a solo developer can list a general SaaS/productivity app for organic search discovery, install, and in-marketplace payment by an unfamiliar customer. Meta Horizon Store meets the mechanical definition of a marketplace but fails the product-category and organic-discoverability fit. **REJECT.**

## B. Marketplace Gate evidence

| Marketplace | Search/discovery | Platform billing | New entrants (volume) | New entrants (named traction) | Organic-entry proof | Solo/compliance | Verdict |
|---|---|---|---|---|---|---|---|
| Wix | PASS (exists), ranking signals UNKNOWN | PASS (confirmed, mandatory Wix Billing System) | UNKNOWN | UNKNOWN — NEEDS EVIDENCE | UNKNOWN — NEEDS EVIDENCE (smaller catalog is fact, "easier" is not proven) | Light — no KYC found | NEEDS EVIDENCE |
| Shopify | PASS, partial official ranking factors | PASS (confirmed, mandatory Shopify billing, best revenue share: 100% to $1M lifetime) | PASS (~12.3k→18.4k apps in ~16 months) | PARTIAL — community/Indie Hackers evidence of organic-only growth exists, but real cold-start friction is also documented | PARTIAL — organic path exists but is slow/review-dependent, not free | Moderate — no KYC, but strict/growing technical requirements (mandatory GraphQL migration) | PASS candidate |
| Atlassian | PASS, most explicit official ranking factors + only found newcomer-visibility badge system (Rising Star) | PASS (confirmed, fully platform-managed for Paid-via-Atlassian) | PASS (7,200–8,000+ apps, 1,800+ vendors) | CONFIRMED with caveat (2026-09-19 B0 check): Rising Star apps verifiably rank on real search queries (2x #1, 1x #2 across 8 queries), but every example found is a new *product* from an already-multi-app vendor, not a first-time solo debut — NEEDS EVIDENCE specifically for the true-first-timer case | PASS — confirmed via live search testing, strongest of the four, though category-dependent (weak on saturated generic terms like "time tracking") | KYC/company-email required — but user already has Gewerbe, so this is largely already satisfied; security review overhead is real and above other candidates; sampled Rising Star apps all had trust-center/security-questionnaire infrastructure already in place from prior products | PASS candidate |
| WordPress (wordpress.org) | PASS (documented two-phase algorithm) | **FAIL — confirmed no paid/gated code allowed; billing must be external** | PASS (6,086 new plugins in 2025, official figure) | UNKNOWN — NEEDS EVIDENCE (no brand-new-entrant traction example found; growth example found was 5 years old) | WEAK — documented tendency to favor established plugins | Light — no KYC, ~5 business day review | REJECT (commercial fit fails Marketplace Gate) |
| WordPress.com Marketplace | UNKNOWN (different, smaller surface; not researched in depth) | PASS (confirmed platform-managed SaaS billing) | UNKNOWN — NEEDS EVIDENCE | UNKNOWN — NEEDS EVIDENCE | UNKNOWN — NEEDS EVIDENCE | UNKNOWN | NEEDS EVIDENCE (out of scope unless wordpress.org path is fully closed) |
| Meta (all surfaces checked) | Partner Directory: no install/search catalog. Horizon Store: PASS but wrong product category | Partner Directory: N/A. Horizon Store: PASS but wrong category | N/A for a general SaaS use case | N/A | FAIL for general SaaS (no matching surface); Horizon Store has documented discovery complaints | N/A | REJECT (no marketplace fits the model) |

## C. Deep research rules

Once one marketplace passes screening, research only that marketplace in depth.

### Required keyword sample

Use 10–20 concrete user-intent queries.

For every query record:

| Field | Value |
|---|---|
| Exact query | |
| Date | |
| Marketplace | |
| Result 1 | |
| Result 2 | |
| Result 3 | |
| Review signals | |
| Install signals | |
| New entrant visible? | |
| Pain/wedge hypothesis | |
| Notes | |

### New entrant test

Find multiple apps added/appearing within approximately the previous 12 months.

Record only public evidence:

- listing date / age if available;
- review count;
- rating;
- visible installs;
- ranking position;
- other public traction signal;
- evidence URL.

### Pain test

Collect at least 10–20 genuine customer statements across several competing apps.

Classify each:

- bug/reliability;
- missing feature;
- workflow friction;
- compatibility;
- price;
- support;
- migration;
- performance;
- other.

Mark switching language separately.

### Switching evidence

Strong signals include:

- alternative-to language;
- switching/migration language;
- explicit intent to replace;
- recent entrant receiving praise for solving the same pain;
- repeated requests for a missing capability.

### Phase B1 — Search Landscape (executed 2026-09-19)

**Methodology note:** The 22 queries below were generated from the real Atlassian Marketplace category taxonomy (project-management, software-development, admin-tools, data-analytics, content-communication, sales-customer-relations, design-diagramming — confirmed live categories) and from natural customer-language phrasing, **not** by starting from B0's known Rising Star examples. No query was chosen because a Rising Star app was already known to live there. All 22 were executed live against `https://marketplace.atlassian.com/search?query=<query>&hosting=cloud` on 2026-09-19. Badge/rating/install data is transcribed directly from the live page; nothing is inferred or estimated.

| # | Exact query | Marketplace | Top 5 results (App — Vendor — Rating — Reviews — Installs — Badges) | Search intent | Notes |
|---|---|---|---|---|---|
| 1 | `user access review` | Jira Cloud | 1. Access Reviewer360 — miniOrange — no rating — 12 installs — SILVER, RUNS ON ATLASSIAN<br>2. Project Access Review for Jira Cloud — Akeles Consulting — 5/5 (1) — 46 — SILVER, RUNS ON ATLASSIAN<br>3. UpRaise for Employee Success — Amoeboids — 4.1/5 (42) — 642 — GOLD, CLOUD FORTIFIED<br>4. Approvals for Confluence — AppFox — 4.4/5 (21) — 986 — GOLD, CLOUD FORTIFIED<br>5. Access Agent for Jira Snapshots for Confluence — RadBee — no rating — 311 — SILVER, CLOUD FORTIFIED | Admin/compliance: periodic access audits for SOC2/security review | No Rising Star/Spotlight/Bestseller badge anywhere in results. #1 and #2 are tiny (12, 46 installs) yet rank at the very top for an exact-match compliance query. Several more near-zero apps appear just below top 5 (User Access Review for Jira by Ballon Apps — 0 reviews shown; Access Review for Jira by Flow Time Apps — 1 install; Access Evidence by ArdSaor — 1 install). Result #3 (UpRaise, an OKR/feedback app) is a poor intent match, showing the ranking isn't purely keyword-exact. |
| 2 | `bulk user management` | Jira Cloud | 1. User Management for Jira (bulk & timed inactive users) — TechTime — 4.8/5 (25) — 865 — SILVER, CLOUD FORTIFIED<br>2. User Management for Confluence (same family) — TechTime — 4.3/5 (5) — 452 — SILVER, CLOUD FORTIFIED<br>3. BulkOps Pro — ELFAPP Technologies — 3.1/5 (4) — 232 — RUNS ON ATLASSIAN<br>4. BulkOps Free — ELFAPP Technologies — 2.6/5 (35) — 1.6k — RUNS ON ATLASSIAN<br>5. Deep Clone for Jira — codefortynine — SPOTLIGHT — 4.5/5 (134) — 11.9k — PLATINUM, CLOUD FORTIFIED | Admin: reduce license cost / manage inactive users at scale | Top 4 results are all SILVER-partner or unbadged small/mid vendors (TechTime, ELFAPP) — no PLATINUM veteran dominates until #5, and #5 is a loosely-related clone tool, not a direct competitor. Real, if modest, install counts. |
| 3 | `audit log confluence` | Confluence Cloud | 1. User Activity Audit Log for Confluence — Twinit — no rating — 30 — SILVER<br>2. Audit Log for Confluence (Pages, Blogs & Attachments) — Aptify Tech — no rating — 7 — RUNS ON ATLASSIAN<br>3. Link Tools – Bulk Editor, Graphs, Audit, Structure — STAGIL — 3.9/5 (20) — 538 — SILVER<br>4. LogViewer for Confluence — Accxia — no rating — 29 — RUNS ON ATLASSIAN<br>5. Event Journal for Confluence Cloud — Softgrown — no rating — 4 — none | Admin/compliance: who changed/viewed what content | Every genuine audit-log app in the top 5 has single-digit-to-30 installs and zero visible ratings — this is a real but extremely thin-adoption niche. No veteran or badge anywhere. Could mean "wide open" or could mean "nobody wants this yet" — cannot distinguish from search data alone. |
| 4 | `gdpr compliance confluence` | Confluence Cloud | 1. Data Protection Toolkit: GDPR, PII & DLP — Actonic — 4.1/5 (8) — 176 — SILVER, CLOUD FORTIFIED<br>2. Compliance for Confluence (DLP, Classification & Detection) — AppFox — 4.1/5 (11) — 502 — GOLD, CLOUD FORTIFIED<br>3. SoftComply Validation for Confluence — SoftComply — 5/5 (2) — 57 — GOLD, CLOUD FORTIFIED<br>4. STAGIL Workflows and Fields — STAGIL — no rating — 50 — SILVER<br>5. Compliance Glossary for Confluence — DailyMind — no rating — 3 — none | Compliance: GDPR/PII discovery and redaction | Small/mid GOLD-and-SILVER vendors throughout; no PLATINUM incumbent, no Bestseller/Spotlight/Rising Star badge. Install counts modest but nonzero (57–502), consistent with a real but narrow paid compliance niche. |
| 5 | `custom dashboard jira` | Jira Cloud | 1. Custom Charts for Jira — Tempo Software — BESTSELLER — 4.5/5 (139) — 8.1k — PLATINUM, CLOUD FORTIFIED<br>2. Rich Filters for Jira Dashboards — Appfire — SPOTLIGHT — 4.8/5 (185) — 9.5k — PLATINUM, CLOUD FORTIFIED<br>3. Easy Reports — Bloompeak — 4.8/5 (91) — 2.9k — GOLD, RUNS ON ATLASSIAN<br>4. Easy Reports Free — Bloompeak — 4.8/5 (91) — 11.7k — GOLD, RUNS ON ATLASSIAN<br>5. eazyBI for Jira — eazyBI — BESTSELLER — 4.7/5 (227) — 11k — PLATINUM, CLOUD FORTIFIED | Reporting: build custom dashboards/charts | Saturated by PLATINUM/GOLD veterans with thousands of installs and Bestseller/Spotlight badges throughout. No small/new entrant visible in top 5. |
| 6 | `jql query builder` | Jira Cloud | 1. KARMA Page Builder for Confluence — Aura Apps — 4.9/5 (164) — 3.5k — PLATINUM, CLOUD FORTIFIED (off-topic: Confluence formatting, not JQL)<br>2. GO! JQL: Essential JQL Functions — Almbase — 4.5/5 (10) — 202 — no badge<br>3. JQL Search Extensions for Jira — Appfire — 4.1/5 (51) — 3.9k — PLATINUM, CLOUD FORTIFIED<br>4. Enhanced Search for Jira (JQL & Subqueries) — Adaptavist Group — 4.1/5 (8) — 911 — PLATINUM, CLOUD FORTIFIED<br>5. JQL Tricks for Jira — J-Tricks — 3.9/5 (28) — 1.1k — GOLD, CLOUD FORTIFIED | Power-user: extend/simplify JQL search | Only 698 total matches (smaller pool than most other queries, "over 1,000" elsewhere). One small unbadged vendor (Almbase, 202 installs) sits at #2 among PLATINUM competitors — a real but modest opening. |
| 7 | `export jira issues to excel` | Jira Cloud | 1. Better Excel Exporter for Jira — Midori Global Consulting — SPOTLIGHT — 4.9/5 (254) — 4.4k — PLATINUM, CLOUD FORTIFIED<br>2. Xporter — Xblend — 4.6/5 (293) — 3.8k — PLATINUM, CLOUD FORTIFIED<br>3. Exporter for Jira — Deiser — 3.7/5 (59) — 1.4k — GOLD, CLOUD FORTIFIED<br>4. BigTemplate — Appfire — 3.8/5 (66) — 3.7k — PLATINUM, CLOUD FORTIFIED<br>5. Better PDF Exporter for Jira — Midori Global Consulting — SPOTLIGHT — 4.8/5 (467) — 4.4k — PLATINUM, CLOUD FORTIFIED | Reporting: export issues for offline/stakeholder reporting | Fully veteran/PLATINUM-dominated with Spotlight badges throughout; no small entrant visible. |
| 8 | `confluence page views analytics` | Confluence Cloud | 1. Google Analytics for Confluence — Capable — 3.9/5 (11) — 396 — CLOUD FORTIFIED (no partner tier shown)<br>2. view26 Page View Analytics for Confluence Cloud — view26 GmbH — 4.7/5 (4) — 306 — SILVER, CLOUD FORTIFIED<br>3. Better Content Archiving and Analytics — Midori Global Consulting — 4.8/5 (155) — 1.2k — PLATINUM, CLOUD FORTIFIED<br>4. Viewtracker – Analytics for Confluence — Elevatic — 4.6/5 (62) — 2.4k — PLATINUM, CLOUD FORTIFIED<br>5. Google Analytics in Confluence — David Simpson Apps — 4.7/5 (29) — 319 — no badge | Analytics: which pages get read, by whom | Small/no-partner-tier vendors (view26 with only 4 reviews, David Simpson Apps, Capable) sit interleaved with PLATINUM incumbents rather than being pushed off the page — a genuine mixed result, not veteran-only. |
| 9 | `confluence approval workflow` | Confluence Cloud | 1. Workflows for Confluence — AppFox — 4.7/5 (25) — 954 — GOLD, CLOUD FORTIFIED<br>2. AURA Workflow & Approval for Confluence — Aura Apps — 5/5 (33) — 275 — PLATINUM, CLOUD FORTIFIED<br>3. Page Approval for Confluence — Appfire — 3.4/5 (73) — 1.7k — PLATINUM, CLOUD FORTIFIED<br>4. Capable Approval for Confluence — Capable — 5/5 (1) — 55 — CLOUD FORTIFIED (no partner tier shown)<br>5. Forms for Confluence — Kolekti/Adaptavist Group — 4/5 (58) — 1.4k — PLATINUM, CLOUD FORTIFIED | Document control: page sign-off/review workflow | Mostly GOLD/PLATINUM incumbents; one genuinely tiny new entrant (Capable Approval, 1 review, 55 installs) visible at #4. |
| 10 | `email notifications jira` | Jira Cloud | 1. Notification Assistant for Jira – Email — Modus Create — 4.4/5 (57) — 1.2k — GOLD (no CLOUD FORTIFIED shown)<br>2. Raley Email Notifications for Jira & JSM — RaleyApps — 3.8/5 (33) — 382 — SILVER, CLOUD FORTIFIED<br>3. Email This Issue — META-INF KFT — BESTSELLER — 4.4/5 (181) — 5.7k — PLATINUM, CLOUD FORTIFIED<br>4. Simple Reminder – Email Notifications — Simple — 4.9/5 (11) — 113 — no badge<br>5. Inbox for Jira (smart notifications) — Rixter AB — 4.4/5 (21) — 517 — SILVER, RUNS ON ATLASSIAN | Ops: keep stakeholders informed via email | One Bestseller veteran at #3, but #1, #2, #4, #5 are all small/mid vendors with modest installs (113–1.2k) — not a veteran monopoly. |
| 11 | `slack integration jira` | Jira Cloud | 1. Slack Integration+ for Jira — Appfire — 4.6/5 (77) — 2.7k — PLATINUM, CLOUD FORTIFIED<br>2. Slack Integration for Jira — Troopr Labs — 4.9/5 (17) — 162 — no badge<br>3. Slack Connector for Jira — WISOFT — 3.4/5 (57) — 1.2k — SILVER<br>4. Slack Connector for Jira Cloud — J Soft — 4/5 (6) — 131 — no badge<br>5. Power BI Connector for Jira — Tempo Software — BESTSELLER (off-topic) | Integration: Jira updates surfaced in Slack | A PLATINUM veteran leads, but 3 of the next 4 slots are small/unbadged vendors (Troopr Labs, J Soft) with double-digit review counts and installs in the low hundreds — real coexistence, not exclusion. |
| 12 | `table of contents confluence` | Confluence Cloud | 1. Easy Heading Macro (Floating Table of Contents) — Shinetech Software — 4.1/5 (19) — 1.5k — SILVER<br>2. Table Filter, Charts & Spreadsheets — Stiltsoft — BESTSELLER (off-topic)<br>3. KARMA Page Builder — Aura Apps — PLATINUM, CLOUD FORTIFIED (off-topic)<br>4. Scroll Content Manager — K15t — PLATINUM, CLOUD FORTIFIED (off-topic)<br>5. Advanced Tables for Confluence — Appfire — PLATINUM, CLOUD FORTIFIED (off-topic) | Content formatting: in-page navigation aid | "Floating Table of Contents for Confluence" by Grovr (no rating, 42 installs, no badge) — the smallest true competitor — appears further down the list (~position 11), not in top 5. Only two genuine TOC-specific apps exist at all (Easy Heading Macro and Grovr's app); review counts across the whole niche are thin (max 19 reviews). Top 5 is otherwise dominated by large off-topic formatting suites, meaning discoverability for this exact intent is poor even though the niche itself has almost no dedicated competition. |
| 13 | `hubspot integration jira` | Jira Cloud | 1. HubSpot CRM Integration for Jira — Appsvio — 4.2/5 (9) — 379 — SILVER<br>2. HubSpot CRM Connector for Jira — Presago — 5/5 (4) — 225 — SILVER<br>3. HubSpot Integration for Jira (HubSpot Connector) FORGE — Getint integrations — 4.1/5 (4) — 144 — GOLD, CLOUD FORTIFIED<br>4. HubSpot Connector for Jira — Korvex Systems — no rating — 457 — no badge<br>5. Slack Integration+ for Jira — Appfire — PLATINUM, CLOUD FORTIFIED (off-topic) | Integration: sync CRM records ↔ Jira issues | All four genuine HubSpot-Jira apps are small/unbadged-or-SILVER vendors with no PLATINUM incumbent and no Bestseller/Spotlight badge anywhere in the category. Installs (144–457) show real, if modest, adoption. |
| 14 | `customer feedback widget jira` | Jira Cloud | 1. Smart Forms for Jira — SaaSJet — 4.7/5 (48) — 1k — PLATINUM, CLOUD FORTIFIED<br>2. Jira Misc Custom Fields — Appfire — PLATINUM, RUNS ON ATLASSIAN (off-topic)<br>3. Custom Charts for Jira — Tempo — BESTSELLER (off-topic)<br>4. UpRaise for Employee Success — Amoeboids — GOLD, CLOUD FORTIFIED (off-topic)<br>5. Awesome Custom Fields — Seibert — RUNS ON ATLASSIAN (off-topic) | Product: collect end-customer feedback on features | Query matched poorly — 4 of top 5 are generic custom-field/reporting apps, not feedback tools. Genuine feedback apps are buried further down and thin: Myra (META-INF KFT, PLATINUM, 1 review/17 installs), Customer Satisfaction (CSAT) Survey (Candylio, 43 reviews/561 installs), Pendo Feedback for Jira (152 installs, no rating). |
| 15 | `salesforce integration confluence` | Confluence Cloud | 1. Connector for Salesforce & Confluence Cloud — Appfire — 3.6/5 (15) — 344 — PLATINUM, CLOUD FORTIFIED<br>2. Salesforce for Confluence — UpSmith — 5/5 (4) — 121 — no badge<br>3. SharePoint Connector for Confluence — Elevatic — PLATINUM, CLOUD FORTIFIED (off-topic)<br>4. Google Drive Connector in Confluence — ikuTeam — GOLD, CLOUD FORTIFIED (off-topic)<br>5. Mermaid Integration for Confluence — Toshihiro Sato — SILVER (off-topic) | Integration: surface Salesforce data in Confluence pages | Only two genuine Salesforce-Confluence apps exist at all; the smaller one (UpSmith, no partner badge, 121 installs) ranks above most off-topic connectors. Extremely narrow — total addressable competition is 2 apps. |
| 16 | `org chart confluence` | Confluence Cloud | 1. Table Filter, Charts & Spreadsheets — Stiltsoft — BESTSELLER (off-topic)<br>2. SequenceDiagram.org for Confluence — NoSpareTime AB (off-topic)<br>3. Excel-like Tables for Confluence — Ricksoft — PLATINUM, CLOUD FORTIFIED (off-topic)<br>4. Mermaid Charts & Diagrams for Confluence — weweave — BESTSELLER (off-topic)<br>5. Easy Gantt Charts for Confluence — Narva Software — GOLD, RUNS ON ATLASSIAN (off-topic) | Content: visualize team/reporting hierarchy | The one genuine org-chart app, "Org Charts, Organizational Charts for Confluence" (BOJA Technology, SILVER, 5/5 rating shown with no review count visible, RUNS ON ATLASSIAN), appears at roughly position #8 — not in the top 5. Query-intent match at the top of results is very poor (all diagramming/table tools, not org charts specifically). |
| 17 | `roadmap timeline jira` | Jira Cloud | 1. Calendar for Jira — Teamlead — 3.3/5 (104) — 1k — SILVER<br>2. Portfolio Roadmaps, Kanban & Timeline Structure — DevSamurai — 4.3/5 (30) — 1.5k — GOLD, CLOUD FORTIFIED<br>3. Swanly — Appfire — 4.1/5 (61) — 1.5k — PLATINUM, CLOUD FORTIFIED<br>4. Time Squad — Apwide — 4.1/5 (11) — 221 — SILVER, CLOUD FORTIFIED<br>5. Activity Timeline — Reliex — BESTSELLER — 4.7/5 (121) — 3.7k — PLATINUM, CLOUD FORTIFIED | Planning: cross-project roadmap visualization | Established/veteran category; only one small entrant (Time Squad, 221 installs) visible, and even it has a GOLD/SILVER-tier established vendor profile, not a true newcomer. |
| 18 | `flowchart jira` | Jira Cloud | 1. ScriptRunner for Jira — Adaptavist Group — SPOTLIGHT — 4.6/5 (826) — 35k — PLATINUM, CLOUD FORTIFIED (off-topic)<br>2. Bar Charts for Jira — TNG Technology Consulting — 3.2/5 (36) — 572 — SILVER, RUNS ON ATLASSIAN<br>3. Jira Workflow Toolbox — Decadis AG — SPOTLIGHT — 4.9/5 (540) — 4.8k — PLATINUM, CLOUD FORTIFIED (off-topic)<br>4. Xray – Test Management for Jira — Xblend — BESTSELLER (off-topic)<br>5. Lucidchart Diagrams Connector for Jira — Lucid — 3.8/5 (47) — 7.9k (off-topic, large veteran) | Diagramming: draw flowcharts linked to Jira issues | Total domination by large veterans/Spotlight/Bestseller apps, none of which are actually flowchart tools — the query itself surfaces mostly unrelated large automation/testing apps. |
| 19 | `gantt chart jira` | Jira Cloud | 1. Gantt-Chart for Jira — Werkstack GmbH — 3.4/5 (129) — 501 — SILVER<br>2. BigGantt – Gantt Chart for Jira — Appfire — 3.5/5 (273) — 5.7k — PLATINUM, CLOUD FORTIFIED<br>3. Gantt Charts for Structure PPM — Tempo Software — 4.2/5 (61) — 6.4k — PLATINUM, CLOUD FORTIFIED<br>4. WBS Gantt-Chart for Jira — Ricksoft — 3.5/5 (160) — 5.5k — PLATINUM, CLOUD FORTIFIED<br>5. Project Management, Resource Planning & Gantt Chart — DevSamurai — 4.3/5 (175) — 3.2k — GOLD, CLOUD FORTIFIED | Planning: Gantt-style scheduling | Fully saturated by PLATINUM/GOLD veterans with thousands of installs each; no small entrant in top 5. |
| 20 | `okr tracking jira` | Jira Cloud | 1. OKR in Jira — Oboard Inc. — 4.8/5 (110) — 2.9k — GOLD<br>2. OKR for Jira — Appfire — 4.5/5 (43) — 1.1k — PLATINUM, CLOUD FORTIFIED<br>3. Timesheet Tracking for Jira — Cappsule — BESTSELLER (off-topic)<br>4. Timesheets by Tempo — Tempo Software — SPOTLIGHT (off-topic)<br>5. Clockwork Pro for Jira — HeroCoders — PLATINUM (off-topic) | Goal-setting: track OKRs inside Jira | Notable: "Bazz-OKR: AI-Powered OKR Automation for Jira" (Bazz OKR, a genuinely new single-app vendor) carries a **RISING STAR** badge and appears at roughly position #9 with 5/5 (4 reviews) and 47 installs — a live, non-cherry-picked sighting of a Rising Star badge on what appears to be a true first-time vendor. This is a distinct, positive data point for the still-open "first-time unknown vendor success" question tracked in DECISION.md, though a single sighting is not enough to resolve it. |
| 21 | `code review jira` | Jira Cloud | 1. Sprint Review for Jira — Applifare Technologies — 5/5 (21) — 80 — RUNS ON ATLASSIAN<br>2. Sprint Reviewer Pro — Forge5 — 5/5 (29) — 92 — RUNS ON ATLASSIAN<br>3. AI Apps Builder for Jira — SaaSJet Studios — 5/5 (18) — 223 — no badge<br>4. UpRaise for Employee Success — Amoeboids — GOLD, CLOUD FORTIFIED (off-topic)<br>5. Collaborator – Code Review Integration for Jira Cloud — SmartBear — no rating — 35 — PLATINUM | Engineering: review pull requests/commits from Jira | Query-intent match is poor: "code review" surfaces sprint-review and AI-builder apps, not source-code review tools. The one genuine code-review app (SmartBear's Collaborator) is thin (35 installs) despite a PLATINUM parent. Cannot tell if this reflects weak real demand or simply a mismatched search term. |
| 22 | `test case management jira` | Jira Cloud | 1. Xray – Test Management for Jira — Xblend — BESTSELLER — 4.3/5 (553) — 25.4k — PLATINUM, CLOUD FORTIFIED<br>2. Zephyr – Test Management and Automation — SmartBear — SPOTLIGHT — 4.1/5 (492) — 15.3k — PLATINUM, CLOUD FORTIFIED<br>3. AIO Tests — Navarambh Software — BESTSELLER — 4.9/5 (114) — 3.5k — GOLD, CLOUD FORTIFIED<br>4. Zephyr Essential — SmartBear — 3.9/5 (900) — 10.1k — PLATINUM<br>5. Requirements & Test Management for Jira — Deviniti — 4.4/5 (66) — 2k — PLATINUM, CLOUD FORTIFIED | QA: manage test cases/plans tied to Jira issues | Extremely saturated — every top-5 app has thousands to tens of thousands of installs and a placement badge. No opening visible. |

### Phase B1 — Intent classification (PROMISING / WEAK / REJECT)

Classified against the four B1 criteria: (1) real marketplace demand, (2) paid apps present, (3) not exclusively veterans, (4) smaller/newer apps at least sometimes visible, plus (5) a potentially narrow customer problem. No numerical score used, per instruction.

| # | Query | Classification | Reasoning |
|---|---|---|---|
| 1 | user access review | **PROMISING** | Tiny/new apps (12–46 installs) dominate top 2 slots for an exact-match compliance query; several more near-zero apps visible just below. No veteran or badge presence at all in this niche. |
| 2 | bulk user management | WEAK | Small/mid vendors dominate, but the leading vendor (TechTime, 865+452 installs across two listings) is already fairly established, not a fresh entrant; niche is real but less "wide open" than #1. |
| 3 | audit log confluence | **PROMISING**, but demand strength itself is NEEDS EVIDENCE | Every competing app has single-digit-to-30 installs and no ratings — real absence of incumbents, but this could equally mean nobody wants the product yet. Search-visibility criterion is met; underlying demand is not verified beyond it. |
| 4 | gdpr compliance confluence | **PROMISING** | Small/mid GOLD-and-SILVER vendors throughout, no PLATINUM incumbent, modest but nonzero installs (57–502) consistent with a real narrow paid compliance niche. |
| 5 | custom dashboard jira | REJECT | Saturated by PLATINUM/GOLD veterans with Bestseller/Spotlight badges and thousands of installs; no opening. |
| 6 | jql query builder | WEAK | One small unbadged vendor visible at #2, but rest of top 5 is PLATINUM-dominated; category itself (JQL power-user tooling) is arguably not "narrow" enough. |
| 7 | export jira issues to excel | REJECT | Fully veteran/PLATINUM-dominated with Spotlight badges; classic saturated utility category. |
| 8 | confluence page views analytics | **PROMISING** | Small/no-partner-tier vendors genuinely interleaved with (not excluded by) PLATINUM incumbents; real mixed result, not veteran monopoly. |
| 9 | confluence approval workflow | WEAK | Mostly GOLD/PLATINUM incumbents; only one genuinely tiny entrant (1 review) visible, and the category (document workflow) is broad, not narrow. |
| 10 | email notifications jira | WEAK | Mixed result with one Bestseller veteran and several small vendors, but "email notifications" is a broad utility category, not a narrow customer problem. |
| 11 | slack integration jira | WEAK | Real coexistence of small vendors (Troopr Labs, J Soft) alongside a PLATINUM leader, but this is a broad integration category already well served. |
| 12 | table of contents confluence | WEAK | Near-zero competition specifically for TOC (only 2 real apps, max 19 reviews), but top-of-results discoverability for the exact query is poor (dominated by unrelated large formatting suites) and overall demand signal is very thin. |
| 13 | hubspot integration jira | **PROMISING** | All four genuine competing apps are small/SILVER-or-unbadged vendors, no PLATINUM incumbent, no placement badges anywhere in category, real modest installs (144–457) — narrow, real, and open. |
| 14 | customer feedback widget jira | REJECT | Query-intent match is poor (top 5 mostly off-topic); genuine feedback apps are buried and thin (17–561 installs); weak evidence of demand specifically for "feedback widget." |
| 15 | salesforce integration confluence | WEAK | Only two apps exist for this exact intent (extremely narrow), but total demand signal (15 and 4 reviews respectively) is very thin. |
| 16 | org chart confluence | WEAK | Only one genuine org-chart app exists and it does not rank in the top 5 for its own category name — poor discoverability even in an uncontested niche. |
| 17 | roadmap timeline jira | REJECT | Veteran/PLATINUM-dominated planning category; only entrant present is already GOLD/SILVER-tier established, not new. |
| 18 | flowchart jira | REJECT | Total domination by large veterans (ScriptRunner, Jira Workflow Toolbox, Xray) that are not even on-topic; no real flowchart-specific competition visible. |
| 19 | gantt chart jira | REJECT | Fully saturated by PLATINUM/GOLD veterans with thousands of installs each. |
| 20 | okr tracking jira | WEAK, with one notable data point | Top 5 mixed with off-topic Bestseller/Spotlight apps; but a live, non-cherry-picked **RISING STAR** sighting (Bazz-OKR, single-app vendor, 4 reviews/47 installs) appeared at ~position 9 — see cross-reference to B0 in DECISION.md. |
| 21 | code review jira | NEEDS EVIDENCE | Query-intent match itself is uncertain (surfaces sprint-review tools, not code review); cannot separate "weak demand" from "wrong search term" without further research, which is out of scope for B1. |
| 22 | test case management jira | REJECT | Extremely saturated (10k–25k+ installs on every top-5 app). |

**Summary:** Of 22 queries, 4 are classified PROMISING outright (user access review, GDPR compliance/Confluence, Confluence page-view analytics, HubSpot–Jira integration), 1 is PROMISING on the search-visibility criterion but flagged NEEDS EVIDENCE on underlying demand strength (audit log/Confluence), 9 are WEAK, 7 are REJECT, and 1 is NEEDS EVIDENCE due to ambiguous query-intent match (code review). This is fewer clean PROMISING results than the 5–10 range the task description anticipated — reported honestly rather than stretched to fill the range. A cross-cutting observation: four of the five PROMISING/near-PROMISING intents (user access review, audit log, GDPR compliance, and to a lesser extent bulk user management) sit in the same admin/compliance theme — this may indicate a genuinely underserved theme on Atlassian Marketplace rather than four independent niches, which is itself worth carrying into Phase C rather than treating as redundant.

### Phase C — Demand Validation (executed 2026-09-19)

**Методологія:** для кожного з 5 intent, відібраних у Phase B1, перевірено не тільки search-результати, а окремі app listing pages (`tab=overview` та `tab=reviews`) для 3-5 репрезентативних конкурентів на intent (найменші, середні та — де є — найбільш усталені гравці). Зафіксовано: pricing model (`Payment model` з Version information на overview tab — Atlassian не рендерить точні цінові рівні статично, тому конкретні $-цифри позначені NEEDS EVIDENCE нижче), дату останнього релізу (update activity), дату та зміст відгуків (не тільки рейтинг), формулювання явного switching/production-use language у відгуках. Усі дані — з живих сторінок Atlassian Marketplace, дата перевірки 2026-09-19.

**Явне правило, застосоване тут:** низька конкуренція сама по собі НЕ трактується як доказ хорошої ніші (`NEEDS EVIDENCE`, поки немає доказу реального попиту — installs, reviews, свідчення оплати).

---

**1. `user access review`**

| App | Vendor | Installs | Reviews | Last release | Payment model | Notes |
|---|---|---|---|---|---|---|
| Access Reviewer360 | miniOrange | 12 | 0 | v5.1.0, Sep 3 2026 | Paid via Atlassian | Активно оновлюється, але 0 reviews — неможливо підтвердити реальне використання. |
| Project Access Review for Jira Cloud | Akeles Consulting | 46 | 1 (5/5) | v2.6.0, Aug 3 2026 | Free | Один відгук (Jul 2025): описує конкретну функцію позитивно, але немає switching/production language. |
| AuditAdmin for Jira | MOY Apps | 10 | 2 (5/5) | v8.1.0, Jun 12 2026 | Paid via Atlassian | 2 короткі позитивні відгуки (Jan 2025), один описує реальний use case ("tracking admin rights across projects... great tool for transparency"). |
| Multiplier – Access Management & IGA for Okta and Entra | Multiplier | 177 | 19 (5/5) | v18.25.0, Sep 10 2026 | Paid via Atlassian | Найсильніший доказ у цій групі: відгуки з 2025-2026 описують **реальне багаторічне production-використання** ("used for a few years"), пряме switching-свідчення ("saved us a significant amount of money we were considering investing in alternative solutions"), активний вендор відповідає на фічі-реквести. **Але це ширший IGA/access-management продукт, а не вузький "access review" point-solution** — попит підтверджений для суміжної, ширшої категорії, не для точного intent. |

**Verdict: NEEDS EVIDENCE.** Paid-моделі є, конкуренція є, smaller entrants присутні — але реальний, підтверджений (production-use, switching) попит зафіксовано лише для Multiplier, який є ширшим IGA-продуктом, а не вузьким access-review інструментом, що відповідає буквальному query. Для вузьких point-solution апп (12–46 installs) доказів оплаченого/тривалого використання немає — лише 0-2 короткі відгуки. Не можна змішувати ці два докази в один "PASS" для вузького intent.

---

**2. `gdpr compliance confluence`**

| App | Vendor | Installs | Reviews | Last release | Payment model | Notes |
|---|---|---|---|---|---|---|
| Data Protection Toolkit: GDPR, PII & DLP | Actonic Products GmbH | 176 | 8 (3.8/5 based on 6 visible) | v5.1.0, Sep 7 2026 | Paid via Atlassian | Змішані відгуки: 2 технічні скарги (2025, 2020) про баги/повільність, АЛЕ також відгук (2020) із прямим доказом оплаченого-і-працюючого продукту: "we got an official approval from our data protection department, which certify our atlassian tools are now fully compliant." Вендор публічно відповідає на скарги й повідомляє про фікси. |
| Compliance for Confluence (DLP, Classification & Detection) | AppFox | 502 | 11 (3.8/5 based on 8 visible) | v18.140.0, Sep 16 2026 | Paid via Atlassian | Детальний, активний цикл фідбек→фіча: користувач (2022) просить bulk-classification, вендор відповідає і за kілька версій дійсно додає цю функцію (підтверджено в тому ж review thread). Найновіший відгук (Feb 2026) — явно позитивний, описує "made it much easier... simple to set up." Vendor claims "Trusted by Fannie Mae, Infineon, BT, Visa" — це **vendor marketing claim, не перевірене незалежно**, позначено як таке. |
| SoftComply Validation for Confluence (MedTech) | SoftComply | 57 | 2 (5/5) | v9.98.0, Sep 9 2026 | Paid via Atlassian | Обидва відгуки (2023) — розгорнуті, з конкретним регуляторним контекстом (робота з AAMI, eQMS-валідація медичних приладів) — це сильний, специфічний доказ реального платного B2B-використання у вузькій вертикалі. |

**Verdict: PASS.** Real customer demand — так (детальні, різночасові відгуки з конкретними production/regulatory use cases, а не generic похвала); existing paid products — так (усі 3, Paid via Atlassian); install/review activity — помірна, але не нульова, і зростає з часом; real competition — так, 3 генуїнно різні під-ніші (загальний GDPR/PII, DLP/classification, MedTech validation) без PLATINUM-ветерана; potential for smaller entrant — так (усі SILVER/GOLD, без placement-бейджів).

---

**3. `confluence page views analytics`**

| App | Vendor | Installs | Reviews | Last release | Payment model | Notes |
|---|---|---|---|---|---|---|
| view26 Page View Analytics | view26 GmbH | 306 | 4 (4.7/5) | v2.0.0, Aug 22 2025 | Paid via Atlassian | Один відгук (Aug 2022) — прямий доказ багаторічного платного використання: "installed in our org for the past two years... great compliment to the Space Level analytics... As a Premium Confluence subscriber... I highly recommend." |
| Google Analytics for Confluence | Capable | 396 | 11 (3.9/5) | v5.1.0, Sep 11 2026 | Paid via Atlassian | Кілька генуїнних позитивних відгуків 2021-2022 з конкретними use cases ("helps a lot in understanding how to improve public spaces/pages"). |
| Viewtracker – Analytics for Confluence | Elevatic | 2,374 | 62 (4.8/5 based on 20 visible) | v8.0.0, Aug 26 2026 (нова AI Agent feature) | Paid via Atlassian | Найзріліший приклад у всій вибірці: клієнт (Sep 2024) — "Have been using Viewtracker since 2012... one of the few must-have Cloud apps for us." Вендор системно й персонально відповідає на кожен відгук. Активний, недавній feature-реліз (Rovo AI agent, Aug 2026). Vendor claims "10,000+ companies" / "Trusted by Honeywell, Apple, Zeiss, HubSpot" — vendor marketing claim, не перевірено незалежно. |

**Verdict: PASS.** Найсильніший доказ довгострокового, реального, платного попиту в усій вибірці (13-річна історія використання одним клієнтом, безперервний розвиток фічей). Real competition — так, і що важливо: маленькі вендори (view26, 306 installs) реально співіснують з великим ветераном (Viewtracker, 2,374), а не витіснені з нього — це вже було зафіксовано в Phase B1 і підтверджено тут на рівні окремих аккаунтів. Ризик: категорія доведено велика й монетизована, але й ветеран (Viewtracker) дуже сильний і активно інвестує в AI-фічі — вужчий wedge буде складніше сформулювати, ніж у GDPR-компліансі.

---

**4. `hubspot integration jira`**

| App | Vendor | Installs | Reviews | Last release | Payment model | Notes |
|---|---|---|---|---|---|---|
| HubSpot CRM Integration for Jira | Appsvio | 379 | 9 (4.2/5) | v8.9.0, Aug 17 2026 | Paid via Atlassian | Розгорнутий відгук (Nov 2023) описує **реальну production-міграцію** ("in the midst of migrating from Freshdesk to Jira Service Management (JSM) coupled with HubSpot... has since been an integral component in our toolkit"). Вендор персонально відповідає на кожен відгук, включно з негативними. |
| HubSpot CRM Connector for Jira | Presago | 225 | 4 (5/5) | v7.3.0, Jul 15 2026 | Paid via Atlassian | Короткі, але позитивні відгуки (2022-2023). Vendor claim "40k+ companies worldwide" стосується всього портфоліо Presago apps, не саме цього app — позначено як vendor marketing claim. |
| HubSpot Connector for Jira | Korvex Systems | 457 (найбільше з трьох) | 0 | v2.11.0, May 26 2026 | Paid via Atlassian | **Показовий disconnect**: найбільша кількість installs серед трьох, але 0 reviews. Не можна визначити, чи це реальні активні користувачі, чи trial-installs без конверсії — NEEDS EVIDENCE саме для цього app. |

**Verdict: PASS**, з застереженням. Real customer demand підтверджено для 2 з 3 семпльованих апп (детальний production-use відгук в Appsvio); existing paid products — так; install activity помірна (144-457 за Phase B1 даними); real competition — так, 3+ генуїнно різних вендори без PLATINUM-гравця; smaller entrant — так. Застереження: найбільший за installs гравець (Korvex, 457) не має жодного review — це саме по собі не дискваліфікує intent (інші 2 конкуренти показують реальний попит), але має бути позначено, а не проігноровано.

---

**5. `audit log confluence` — посилена перевірка (за прямою вимогою через слабкі install-сигнали з Phase B1)**

| App | Vendor | Installs | Reviews | First/last release | Payment model | Notes |
|---|---|---|---|---|---|---|
| User Activity Audit Log for Confluence | Twinit | 30 | 0 | v2.7.0, Jul 30 2026 | Paid via Atlassian | Регулярно оновлюється, але 0 reviews після кількох версій. |
| Audit Log for Confluence (Pages, Blogs & Attachments) | Aptify Tech | 7 | 0 | v4.6.0, Sep 14 2026 | Paid via Atlassian | Дуже активні релізи (нова функція щойно, Sep 14 2026), але 0 reviews, 7 installs. |
| Auditable: Document Control, Approvals & Audit Evidence | Rethought | 1 | 0 | **v3.3.0 — але "First release" датовано Aug 28 2026** (тобто продукт існує ~3 тижні на момент перевірки) | Paid via Atlassian | Щойно випущений продукт, по суті pre-traction. |
| Access Lens – Permissions Audit for Confluence | Prometheus | 1 | 0 | **"First public release" Jul 7 2026** (~2.5 місяці на момент перевірки) | Paid via Atlassian | Так само pre-traction. |
| (для контрасту) Link Tools – Bulk Editor, Graphs, Audit, Structure | STAGIL by catworkx | 538 | 20 (3.7/5 based on 13 visible) | v2.0.0, Feb 3 2026 | Paid via Atlassian | Реальні, змістовні відгуки з 2024-2025 ("Incredibly useful for cross reference in a dynamic eQMS environment"), але це **не audit-log app** — audit є побічною функцією universal link-management інструменту, отже не є прямим конкурентом на цей intent. |

**Verdict: NEEDS EVIDENCE, з дуже виразним схилянням до "недостатньо доказів попиту" — не PASS.** Явно застосовано правило "мало конкурентів ≠ хороша ніша": усі 4 генуїнні audit-log-специфічні apps мають 0 reviews і 1-30 installs. Два з чотирьох — це фактично щойно запущені продукти (перший реліз 2.5 і 3 тижні тому відповідно на момент перевірки), що незалежно один від одного намагаються закрити ту саму проблему — це слабкий позитивний сигнал ("кілька різних розробників одночасно роблять ставку на цю ідею"), але жоден з чотирьох не має **жодного** підтвердженого платного/тривалого користувача. Payment model скрізь "Paid via Atlassian", але це говорить лише про наявність білінгової моделі, не про факт здійсненої покупки. Критерій "достатня install/user activity" і критерій "докази, що клієнти реально користуються/платять" — обидва не виконані. Це не автоматичний REJECT (могло бути занадто рано), але за інструкцією проекту явно НЕ переходить як PASS.

---

**Підсумок Phase C:**

| # | Intent | Verdict |
|---|---|---|
| 1 | user access review | NEEDS EVIDENCE (доказ попиту є лише для ширшого IGA-продукту, не для вузького point-solution) |
| 2 | gdpr compliance confluence | **PASS** |
| 3 | confluence page views analytics | **PASS** |
| 4 | hubspot integration jira | **PASS** (із застереженням щодо одного конкурента без reviews) |
| 5 | audit log confluence | NEEDS EVIDENCE (посилена перевірка підтвердила: 0 reviews на всіх 4 genuine competitors; ризик "нікому не треба", а не "вільна ніша") |

3 з 5 intent переходять до Phase D (Pain + Switching): **gdpr compliance confluence, confluence page views analytics, hubspot integration jira**. Це в межах ліміту "максимум 3", встановленого завданням. Жоден продукт ще не обрано.

### Phase D — Pain + Switching Evidence (executed 2026-09-19)

**Методологія:** для кожного з 3 intent зібрано genuine customer statements з reviews tabs кількох конкурентів (ті самі + додаткові апп, не досліджені в Phase C, для ширшого охоплення). Джерело — тільки реальний текст відгуків з датою; відгуки без тексту (тільки зірки) не рахуються як "statement" і не включені в таблиці. Один відгук (Daniela Ackermann на Getint app) виключено з доказової бази — вендор публічно засумнівався в його автентичності (немає запису звернень до підтримки, немає відповідного LinkedIn-профілю) — трактується як unverified, не як факт. Додатково виконано 3 targeted web-пошуки (Reddit/G2) на explicit switching-мову для кожного intent — результати не дали жодного релевантного on-topic влучення (тільки шум/незв'язані теми); це зафіксовано як відсутність додаткових доказів, не як позитивний чи негативний сигнал.

---

**1. `gdpr compliance confluence`**

| # | Quote | App | Date | Category | Frequency | Severity | Workaround | Switching language | Product vs support |
|---|---|---|---|---|---|---|---|---|---|
| 1 | "App doesn't load in the cloud, literally just sits there. App is not responding. Wait or cancel?" | Data Protection Toolkit (Actonic) | Aug 22, 2025 | Reliability | Persistent (за словами автора) | HIGH — app непридатний | Немає | Немає | Product issue |
| 2 | "This app is causing many issues in the Confluence Cloud, and we have been waiting for a new release for a long time. ...impact on PDF export time, which takes over 100 seconds instead of 10 seconds. After the PDF export, a new page is generated with an error stating that the app is still loading" | Data Protection Toolkit (Actonic) | Jan 21, 2025 | Performance + Reliability | Щоразу при PDF export (систематично) | HIGH — 10x сповільнення + помилка | Немає | Немає (лише фрустрація "waiting... for a long time") | Product issue (вендор пізніше підтвердив фікс) |
| 3 | "This is a great tool, we got an official approval from our data protection department, which certify that our atlassian tools are now fully compliant." | Data Protection Toolkit (Actonic) | Jun 23, 2020 | Compliance (позитивний outcome) | — | — | — | — | Підтверджує реальний job-to-be-done (пройти внутрішній compliance-аудит) |
| 4 | "Really solid app... made it much easier for us to manage data governance across our Confluence spaces. Simple to set up and works seamlessly." | Compliance for Confluence (AppFox) | Feb 24, 2026 | Reporting/Visibility | — | — | — | — | Позитив, підтверджує value prop |
| 5 | "There seems to be no way to set a default classification for all pages, and no way to bulk-set classifications, and no inheritance of classifications. This makes this very painful to go through and manually apply a classification for thousands of individual pages." | Compliance for Confluence (AppFox) | Feb 7, 2022 | Missing feature / Workflow friction | Повторювано (кожна нова/існуюча сторінка) | HIGH — ручна праця на "тисячах сторінок" | Немає на момент відгуку | Немає явного "switch", але сильне незадоволення | Product issue — вендор пізніше (той самий review thread, "Update") підтвердив: bulk classification і default classification таки додані |
| 6 | "The setup does take some time, but nothing an experienced Atlassian administrator can't handle." | SoftComply Validation | Sep 19, 2023 | Workflow friction (мінорна) | Одноразово (setup) | LOW | Досвідчений адмін вирішує сам | Немає | Product characteristic, не критичний issue |
| 7 | "Using automated validation means we don't need to spend resource time on manually testing and keeping our Jira and Confluence tools in a validated state." | SoftComply Validation | Apr 27, 2023 | Workflow friction (позитивний outcome) | — | — | — | — | Підтверджує: автоматизація ручної compliance-праці — реальна цінність, за яку платять |

**Джерела (URL, дата перевірки 2026-09-19):**
- https://marketplace.atlassian.com/apps/1219041/data-protection-toolkit-gdpr-pii-dlp-for-confluence?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1218474/compliance-for-confluence-dlp-classification-detection?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1229288/softcomply-validation-for-confluence-medtech-compliance?hosting=cloud&tab=reviews

**Повторювані проблеми:** (a) reliability/performance-баги, що ламають плановий, регулярний процес (PDF export) — 2 незалежні згадки в одному й тому ж app (Data Protection Toolkit); (b) відсутність bulk/default-операцій для класифікації великої кількості сторінок (1 детальний відгук, але підтверджений довгим vendor-response циклом, що натякає на ширшу проблему, ніж один клієнт).

**Switching evidence:** Явної "switched from" / "alternative to" / "migrate" мови в жодному з 7 statements НЕ знайдено. Найсильніший непрямий сигнал — фрустрація і "waiting for a new release for a long time" (statement #2), що є попередником switching, але не самим switching. Web-пошук (Reddit/G2) на explicit switching-мову для цього intent — нуль релевантних результатів.

**WEDGE TEST — "bulk/default PII-класифікація для великих legacy-просторів" (з statement #5):**
1. Вирішується однією вузькою функцією? — Так, потенційно: bulk-scan-and-classify з CQL-подібним скоупінгом.
2. Потрібна важка інтеграція? — Ні, тільки Confluence REST/Forge API.
3. Потрібна ручна робота? — Мінімальна з боку розробника; ризик ручної роботи з боку клієнта (масові bulk-дії на контенті вимагають обережного UX із підтвердженням/rollback).
4. Потрібна зовнішня інфраструктура? — Ні, судячи з наявних даних.
5. Чи Forge-first? — Так, ймовірно.
6. Великий support burden? — Помірний ризик (масові зміни контенту — джерело скарг при помилковій класифікації).

**SUPPORT TRAP:** MEDIUM — bulk-операції на клієнтському контенті мають реальний ризик "зіпсували мої дані/розмітку", що вимагає retry/audit-trail функціоналу, а це вже не тривіальний self-serve UX.

**Verdict: NEEDS EVIDENCE.** Реальний, конкретний pain є (bulk-класифікація; reliability на PDF export), але (a) жодного explicit switching-сигналу не знайдено, (b) кожна конкретна проблема підтверджена лише 1 детальним джерелом (не "повторюваністю" у строгому сенсі — кілька незалежних клієнтів з тим самим specific complaint). Це не REJECT (проблема реальна й вирішувана), але й не PASS за критерієм "вузький, повторюваний, потенційно switchable pain."

---

**2. `confluence page views analytics`**

| # | Quote | App | Date | Category | Frequency | Severity | Workaround | Switching language | Product vs support |
|---|---|---|---|---|---|---|---|---|---|
| 1 | "...has been installed in our org for the past two years... As a Premium Confluence subscriber, Page View Analytics for Confluence Cloud is a great compliment to the Space Level analytics that we have access to..." | view26 | Aug 1, 2022 | Reporting/Visibility | — | — | — | **Switching-from-native**: явно каже, що вбудована (Premium) аналітика Confluence недостатня сама по собі | Підтверджує core value prop |
| 2 | "A very useful app to track traffic and users for your Confluence. Helps a lot in understanding how to improve public spaces/pages." | Google Analytics for Confluence (Capable) | Nov 15, 2022 | Reporting/Visibility | — | — | — | Немає | Позитив |
| 3 | "show a connecting error in every pdf. we try to deactivate but they arent a butbton for that. so we cant send this week all our weekly reports. very bad!" | Google Analytics in Confluence (David Simpson Apps) | Sep 6, 2024 | Reliability | Щоразу при PDF export (систематично) | HIGH — заблокувало щотижневу звітність | Спроба деактивації не вдалась (немає кнопки) | Немає явного "switch", але сильне незадоволення ("very bad!") | Product issue |
| 4 | "We were using Confluence at work for a client facing application and needed to pull some analytics for management. The 'out of the box' solution wasn't giving us the exact results we wanted, so we reached out to David for assistance." | Google Analytics in Confluence (David Simpson Apps) | Apr 9, 2024 | Reporting/Visibility | — | — | — | **Switching-from-native**: явно каже, що вбудоване рішення Confluence не влаштувало | Product issue (gap), закрито custom-допомогою вендора |
| 5 | "Works perfectly and helps us analyze our users main interests. Support is super fast." | Viewtracker (Elevatic) | Mar 4, 2025 | Reporting/Visibility | — | — | — | Немає | Позитив |
| 6 | "Have been using Viewtracker since 2012... Migrating our view data from Server to Cloud worked like a charm... team constantly adds new reports and capabilities." | Viewtracker (Elevatic) | Sep 17, 2024 | Migration (позитивний outcome) | — | — | — | Немає | 13-річне утримання клієнта; підтверджує успішну Server→Cloud міграцію без проблем |
| 7 | "...automates content lifecycle tasks like archiving outdated pages and sending review reminders, which saves us a lot of manual effort." | Better Content Archiving and Analytics (Midori) | Mar 17, 2026 | Workflow friction (позитивний outcome) | — | — | — | Немає | Підтверджує: автоматизація ручного content governance — цінність, за яку платять |
| 8 | "keeping outdated content under control is no trivial task... For me, this tool belongs as a standard plugin in every larger Confluence instance." | Better Content Archiving and Analytics (Midori) | Dec 11, 2025 | Reporting/Visibility + Workflow friction | Структурна (постійна проблема) | — | — | Немає | Підтверджує структурний, повторюваний job-to-be-done |

**Джерела (URL, дата перевірки 2026-09-19):**
- https://marketplace.atlassian.com/apps/1218023/view26-page-view-analytics-for-confluence-cloud?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1216514/google-analytics-for-confluence-page-view-tracker-reports?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1216936/google-analytics-in-confluence?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/28637/viewtracker-analytics-for-confluence?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/123/better-content-archiving-and-analytics-for-confluence?hosting=cloud&tab=reviews

**Повторювані проблеми:** (a) вбудована Confluence-аналітика ("Space Level"/"out of the box") недостатня — підтверджено 2 незалежними клієнтами різних app (view26, David Simpson Apps), з різницею ~18 місяців; це і є причина, чому весь цей платний niche взагалі існує — але це вже підтверджений (Phase C) загальний попит, а не новий, невирішений під-pain; (b) PDF-export reliability баг — та сама специфічна проблема категорії "export", що й у GDPR-інтенті (statement #3 тут vs. statement #2 в gdpr-таблиці), в двох повністю незалежних apps і vendors.

**Switching evidence:** Немає жодного explicit "switched from [конкурент]" quote. Є два **switching-from-native** сигнали (statements #1, #4) — клієнти явно перейшли від вбудованого Confluence-рішення до платного app, а не з одного платного конкурента на інший. Це реальний, але слабший тип switching-доказу, ніж той, що вимагає CONTEXT.md (Section 7 "Pain Gate": "alternative to X" / "switched from X"). Web-пошук (Reddit/G2) — нуль релевантних результатів.

**WEDGE TEST — "надійний, простий export/reporting, без reliability-багів, що ламають плановану звітність":**
1. Вирішується однією вузькою функцією? — Частково: сам "надійний export" — це якість виконання, не унікальна фіча; важко зробити з цього самостійний продукт (не можна "полагодити" export чужого конкурента ззовні).
2. Потрібна важка інтеграція? — Ні.
3. Потрібна ручна робота? — Ні.
4. Потрібна зовнішня інфраструктура? — Ні.
5. Чи Forge-first? — Так.
6. Великий support burden? — Помірний (аналітичні apps типово генерують "чому цифри не збігаються" тікети — це логічний висновок, не підтверджений прямим доказом у цій вибірці).

**SUPPORT TRAP:** MEDIUM (за аналогією з категорією — не підтверджено прямим доказом саме тут).

**Verdict: NEEDS EVIDENCE.** Є switching-from-native доказ (сильніший за просто негативний review, за правилом CONTEXT.md §7), але це вже відомий (з Phase C) загальний попит, а не новий under-served під-pain. Немає жодного competitor-to-competitor switching-сигналу. Ринок уже добре обслуговується зрілим лідером (Viewtracker, безперервний розвиток), що звужує простір для wedge.

---

**3. `hubspot integration jira`**

| # | Quote | App | Date | Category | Frequency | Severity | Workaround | Switching language | Product vs support |
|---|---|---|---|---|---|---|---|---|---|
| 1 | "Best HS integration yet. Had a small issue with searching for a match when using custom field, reported to dev team and a few days later they had implemented improved search matching functionality." | HubSpot CRM Integration (Appsvio) | Dec 15, 2025 | Missing feature / Workflow friction | Одноразово, швидко вирішено | LOW (вирішено за кілька днів) | Немає (вирішено vendor'ом) | **Порівняльна мова**: "Best... yet" імплікує досвід з іншими HubSpot-Jira інтеграціями | Product issue, швидко закрито |
| 2 | "In the midst of migrating from Freshdesk to Jira Service Management (JSM) coupled with HubSpot, finding an app that could integrate these platforms effectively was paramount... It promises to provide read-only data visibility on Jira tickets, and it does exactly that." | HubSpot CRM Integration (Appsvio) | Nov 16, 2023 | Migration / Integration-API | — | — | — | Контекст реальної production-міграції (Freshdesk→JSM), явний процес вибору серед варіантів | Підтверджує реальний, дорогий production use case |
| 3 | "Never worked right. Company info from Hubspot would not load, which really was the primary reason for installing it." | HubSpot CRM Integration (Appsvio) | Apr 3, 2023 | Reliability | Постійно (за словами автора) | HIGH — головна причина встановлення не спрацювала | Немає | Немає явного, але сильне незадоволення | Product issue, не support incident |
| 4 | "I tested a lot of integration tools to find the right one for us. Ultimately, this tool didn't support multi-select fields (of which we have many)... It didn't support date fields, but we found a workaround that made it work for us by converting the dates to a string and transferring the string." | HubSpot Integration for Jira FORGE (Getint) | Oct 23, 2024 | Missing feature (integration/API) | Структурна (типи полів завжди відсутні) | MEDIUM — обійдено через workaround | Так: конвертація дат у рядок | **Найсильніший знайдений сигнал**: explicit comparison-shopping "tested a lot of integration tools to find the right one for us" | Product gap, залишились попри нього через простоту налаштування |
| 5 | "Helps synchronize products and eliminate manual copying info from one system to another." | HubSpot Integration for Jira FORGE (Getint) | Apr 16, 2024 | Workflow friction (позитивний outcome) | — | — | — | Немає | Підтверджує core job-to-be-done (усунення ручного copy-paste) |
| 6 | "Keine Möglichkeit zum konfigurieren. Es kommt eine 500 im Netzwerktab und im Manage Apps klappt es nicht auf, andere Plugins laufen Reibungslos." (укр.: "Немає можливості налаштувати. З'являється 500 помилка в мережевій вкладці, і в Manage Apps воно не відкривається, інші плагіни працюють без проблем.") | HubSpot CRM for Jira (resolution) | Apr 22, 2025 | Reliability / Installation | Постійно (за словами автора) | HIGH — блокує будь-яке використання | Немає | Немає | Product issue (вендор каже, що жоден інший клієнт про це не повідомляв — можливо, environment-specific, але для цього клієнта це реальний product failure, не просто "як користуватись" питання) |
| 7 | "This has been one of the easiest integrations I've worked with... covers everything we need without unnecessary complexity." | HubSpot CRM for Jira (resolution) | Apr 15, 2026 | Reporting/Visibility (позитив) | — | — | — | **Порівняльна мова**: "easiest... I've worked with" імплікує досвід з іншими | Позитив |

*Виключено з доказової бази:* відгук "Daniela Ackermann" на Getint app (Feb 19, 2025) — вендор публічно засумнівався в його автентичності (немає записів звернень до підтримки, немає відповідного LinkedIn-профілю). Не використано як факт.

**Джерела (URL, дата перевірки 2026-09-19):**
- https://marketplace.atlassian.com/apps/1226482/hubspot-crm-integration-for-jira?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1227969/hubspot-crm-connector-for-jira?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1231637/hubspot-integration-for-jira-hubspot-connector-forge?hosting=cloud&tab=reviews
- https://marketplace.atlassian.com/apps/1228240/hubspot-crm-for-jira-report-issue-link-collaboration?hosting=cloud&tab=reviews

**Повторювані проблеми:** (a) неповна підтримка типів полів (multi-select, date) в sync/integration апп — 1 детальний приклад (Getint), типова, але не підтверджена на кількох незалежних апп цього ж intent; (b) reliability/installation-баги, що повністю блокують використання — 2 незалежні приклади (Appsvio "never worked right"; resolution's "500 error, won't open").

**Switching evidence:** Це єдиний з 3 intent із явною **порівняльною/comparison-shopping мовою**: "tested a lot of integration tools to find the right one for us" (Getint, statement #4), плюс два слабші імпліцитні порівняльні сигнали ("Best HS integration yet"; "easiest... I've worked with"). Це підтверджує, що клієнти в цій категорії реально оцінюють кілька варіантів перед вибором — важливий, хоч і не найсильніший за шкалою CONTEXT.md §7 (немає прямого "switched from X to Y"), сигнал switchability. Web-пошук (Reddit/G2) — нуль релевантних результатів.

**WEDGE TEST — "надійна HubSpot↔Jira синхронізація з повною підтримкою типів полів (multi-select, date) без workaround":**
1. Вирішується однією вузькою функцією? — Так: коректна field-type mapping — вузька, конкретна інженерна задача.
2. Потрібна важка інтеграція? — Так, за визначенням (HubSpot API + Jira API) — це integration-категорія за своєю природою, отже "важка інтеграція" тут не опціональна, а сама суть продукту.
3. Потрібна ручна робота? — Ні, з боку розробника після побудови; можливе періодичне обслуговування при змінах HubSpot/Jira API.
4. Потрібна зовнішня інфраструктура? — Залежить від реалізації (webhook-приймач, якщо не Forge-native).
5. Чи Forge-first? — Можливо частково (Getint вже має FORGE-версію), але глибока field-mapping синхронізація типово важча в межах Forge-обмежень (NEEDS EVIDENCE — не перевірено окремо).
6. Великий support burden? — Ризик середній-високий: інтеграційні апп типово генерують customer-specific конфігураційні питання (яке поле на яке мапити), що суперечить Solo Gate/Support Gate вимогам проекту.

**SUPPORT TRAP:** HIGH — інтеграційні (integration/API) апп за своєю природою схильні до customer-specific конфігурації, багів на рівні API третьої сторони (HubSpot) поза контролем розробника, і зламів при змінах зовнішнього API — це системний ризик, а не разовий, і прямо суперечить Solo Gate (CONTEXT.md §10: "складні customer-specific integrations" — явний veto-тригер).

**Verdict: NEEDS EVIDENCE**, з найсильнішим із трьох switching-сигналом (explicit comparison-shopping), але з HIGH support-trap ризиком, що ставить під сумнів solo-feasibility цього wedge ще до Phase E.

---

**Загальний підсумок Phase D:**

| # | Intent | Verdict | Найсильніший знайдений сигнал |
|---|---|---|---|
| 1 | gdpr compliance confluence | NEEDS EVIDENCE | Детальний, багаторічно підтверджений feature-gap (bulk classification), але без switching-мови |
| 2 | confluence page views analytics | NEEDS EVIDENCE | Switching-from-native (2 незалежні клієнти), але не competitor-to-competitor |
| 3 | hubspot integration jira | NEEDS EVIDENCE | Найсильніша порівняльна/comparison-shopping мова з трьох, але HIGH support-trap для очевидного wedge |

**Важливо:** жоден з трьох intent не дав явного, підручникового "switched from X to Y" quote. Це чесний результат, а не невдача процесу — за інструкцією проекту (CONTEXT.md §7: "complaint != willingness to switch") відсутність цього сигналу не дозволяє класифікувати жоден intent як PASS на цьому етапі. Numeric score не використано; "більше негативних reviews" НЕ трактовано як "краща можливість" (розділ hubspot integration jira має найбільше позитивних відгуків, а не найбільше скарг, і саме там знайдено найсильніший switching-сигнал — це навмисно суперечить наївній евристиці "шукай скарги").

**2 pain/wedge hypotheses, обрані для подальшого дослідження (максимум 2, за інструкцією):**

**Hypothesis 1 — GDPR/Confluence: вузький bulk/default PII-classification інструмент для великих legacy-просторів**

`Problem` → Адміни великих/старих Confluence-інстансів не можуть масово/за замовчуванням класифікувати сторінки за чутливістю даних; ручна класифікація "тисяч окремих сторінок" описана як "very painful."

`Evidence` → 1 детальний, датований відгук (Compliance for Confluence, Feb 7 2022) + підтверджений vendor-response-цикл (той самий thread: функція запитана 2022, реалізована пізніше) — помірна, не масова доказова база.

`Switching signal` → Відсутній (жодного "switched"/"alternative" quote); є лише тривала фрустрація до моменту, поки функцію не додали.

`Minimal wedge` → Вузький Forge-app: сканування + bulk-класифікація PII/labels за CQL-подібним скоупінгом, без повного DLP-функціоналу конкурентів.

`Support risk` → MEDIUM (bulk-дії на клієнтському контенті вимагають UX з підтвердженням/rollback).

`Platform/API risk` → LOW-MEDIUM (Confluence REST/Forge API підтримують content search/labeling; конкретні ліміти не перевірені окремо — NEEDS EVIDENCE).

**Hypothesis 2 — HubSpot↔Jira: надійна синхронізація з повною підтримкою типів полів**

`Problem` → Існуючі HubSpot-Jira конектори не підтримують деякі типи полів (multi-select, date), змушуючи клієнтів або обходити проблему вручну (конвертація дат у рядок), або продовжувати "тестувати багато інтеграційних інструментів."

`Evidence` → 1 детальний відгук з explicit comparison-shopping мовою (Getint, Oct 23 2024) — найсильніший знайдений сигнал у всій Phase D, але одноджерельний.

`Switching signal` → Порівняльна/comparison-shopping мова ("tested a lot of integration tools to find the right one for us") — не повний "switched from X", але найближче до цього з усього зібраного корпусу.

`Minimal wedge` → Коректна, повна field-type mapping (multi-select, date, etc.) без workaround — вузько сформульована технічна перевага.

`Support risk` → HIGH — інтеграційні апп системно генерують customer-specific конфігураційні запити та залежать від змін API третьої сторони (HubSpot), що напряму конфліктує з Solo Gate (CONTEXT.md §10).

`Platform/API risk` → MEDIUM-HIGH — залежність від HubSpot API (зовнішній, поза контролем Atlassian-екосистеми) на додачу до Jira/Forge API; це подвійна залежність, а не одинарна.

**Explicitly not done:** жоден продукт не обрано; MVP не спроєктовано; numeric score не використано; жоден intent не позначено PASS на основі кількості негативних відгуків; слабкість конкурента не інтерпретована як доказ власного попиту.

### Методологічне уточнення (застосовується з 2026-09-19): класифікація switching evidence

За вказівкою користувача, відсутність literal "switched from X to Y" більше НЕ трактується як автоматичний провал доказової бази. Switching evidence далі розділяється на 4 типи:

- **A — direct replacement:** явна заміна одного рішення іншим (конкурент→конкурент, або інструмент→продукт).
- **B — comparison-shopping:** клієнт явно оцінював кілька варіантів перед вибором.
- **C — replacement intent:** клієнт висловлює намір/бажання замінити, але ще не діяв.
- **D — pain only:** скарга/фрустрація без будь-якого порівняння чи наміру заміни.

Ретроспективна класифікація ключових сигналів з Phase D:
- Anne Dietz (HubSpot/Getint, "tested a lot of integration tools to find the right one for us") → **B**.
- Craig Parsons ("Best HS integration yet"), Thilini Rathnayake ("easiest... I've worked with") → слабкий/імпліцитний **B**.
- Andy Gladstone (view26) та Natalie Dolce (Google Analytics in Confluence) — заміна вбудованого Confluence-рішення платним app → фактично **A** (direct replacement), але baseline — не конкурент, а "no tool"/native functionality, що є іншим типом ринкового сигналу, ніж класичний competitor-to-competitor switch.
- Rob Shannon, Mahyar Ghaffarpour, James Charles, Steffen Grabaum, Besar Bilalli, Amin Mirzaee → **D** (pain only, без порівняння).
- OpsHub's власна фіча "Excel-based user mapping — no more sync failures from user mismatches" (Phase E, нижче) → непрямий, vendor-inferred сигнал типу **C** (вендор явно побудував фічу проти відомої категорії проблем, що натякає на реальний, повторюваний customer pain, який спонукав до заміни/незадоволення) — не пряма customer quote, тому позначено окремо.

## E. Phase E — Wedge Kill Test (executed 2026-09-19)

**Мета:** не підтвердити красиву ідею, а спробувати ВБИТИ обидві гіпотези з Phase D. `confluence page views analytics` переведено у `HOLD` — дослідження не продовжується, поки не знайдено конкретний unmet job (див. DECISION.md).

---

### Кандидат 1: GDPR/Confluence — "bulk/default PII classification for legacy Confluence spaces"

**Досліджено 8 існуючих Marketplace apps** (усі Confluence Cloud, дата перевірки 2026-09-19):

| App | Vendor | Installs/Reviews | Exact workflow | Чого НЕ вирішує |
|---|---|---|---|---|
| [Compliance for Confluence](https://marketplace.atlassian.com/apps/1218474/compliance-for-confluence-dlp-classification-detection?hosting=cloud&tab=overview) | AppFox | 502 / 11 | **Bulk classification вже є**: "Save time with the new bulk classification feature! You can now easily classify multiple pages in one action and use Confluence Query Language (CQL) to narrow the scope." Плюс: default classification, enforce-classification-before-publish, access restriction за рівнем класифікації, audit log, AI-детекція. | AI-детекція описана як "AI-tools" вже присутня (не gap); не покриває consent/DSAR workflows. |
| [Data Protection Toolkit](https://marketplace.atlassian.com/apps/1219041/data-protection-toolkit-gdpr-pii-dlp-for-confluence?hosting=cloud&tab=overview) | Actonic | 176 / 8 | Сканування за шаблонами, **"Schedule checks so nothing slips through"** (уже bulk+scheduled), redact/replace/comment/notify, consent forms, DSAR/right-to-be-forgotten. | Reliability-баги на PDF export (Phase D); UI/UX складність. |
| [PII Protection and DLP for Confluence](https://marketplace.atlassian.com/apps/1230602/pii-protection-and-dlp-for-confluence?hosting=cloud&tab=overview) | Polymetis Apps | 50 / 1 (5/5) | Сканування простору за 70+ типами PII, **автоматизовані дії через Confluence/Jira Automation**, класифікація з кастомними рівнями, SOC 2 Type II, Forge-native (дані не залишають інстанс). | Молодий продукт (1 review) — реальна довгострокова demand-picture ще не підтверджена. |
| [Data - PII Scanner (DLP) for Confluence](https://marketplace.atlassian.com/apps/1233049/data-pii-scanner-dlp-for-confluence?hosting=cloud&tab=overview) | miniOrange | 22 / 0 | Real-time сканування (при create/update), 80+ типів даних, attachment-сканування (PDF/Word), custom regex, automated redaction, violation dashboard, Forge-native. Явно написано: **"Coming up: AI-based scanning, scheduled scans"** — тобто scheduled/bulk-сканування ЩЕ немає, тільки real-time. | Bulk/scheduled scan — поки що реальний gap саме в цьому одному app (але вже "Coming up", отже недовго). |
| [SoftComply Validation for Confluence](https://marketplace.atlassian.com/apps/1229288/softcomply-validation-for-confluence-medtech-compliance?hosting=cloud&tab=overview) | SoftComply | 57 / 2 | Періодичні (twice-monthly) автоматизовані validation-тести — інша ніша (MedTech eQMS validation, не PII-класифікація як така). | Не PII-класифікація за своєю суттю — інший job. |
| [Compliance Glossary for Confluence](https://marketplace.atlassian.com/apps/460119464/compliance-glossary-for-confluence?hosting=cloud&tab=overview) | DailyMind | 3 / 0 | Term-level approval workflow, **compliance scanner на кожен page save** (event-driven, не bulk), CSV audit evidence export. Інший job: контрольована термінологія/glossary, не PII. | Не PII/DLP за суттю. |
| STAGIL Workflows and Fields | STAGIL | 50 / 0 | Jira workflows/fields на Confluence-сторінках — **не PII/GDPR app взагалі**, off-topic, помилково потрапив у B1-вибірку за назвою "compliance". | Немає стосунку до PII-класифікації. |
| [DLP - Sensitive Data (PII, GDPR) Scanner for Confluence](https://marketplace.atlassian.com/apps/544091142/dlp-sensitive-data-pii-gdpr-scanner-for-confluence?hosting=cloud&tab=overview) | (unlisted vendor) | — | Regex-based сканування + page history, encrypt/redact/delete, migration-readiness tools, 9 релізів з Dec 2025 (активна розробка). **Version history показує тільки "Confluence Data Center" реліфи** — це, схоже, Data Center-only app, НЕ Cloud-конкурент. | Не прямий Cloud-конкурент (потребує окремої перевірки хостингу — NEEDS EVIDENCE). |

**Відповіді на контрольні питання:**

1. **Чи функція вже є у 5-10 existing apps?** Так, повністю або майже повністю — у мінімум 3 з 8 (AppFox — bulk+default+enforce; Actonic — scheduled bulk scan+redact; Polymetis — space-level scan+classify+automate). Ще 1 (miniOrange) явно анонсував це як "Coming up".
2. **Exact workflows, що вони підтримують:** CQL-scoped bulk classification (AppFox); scheduled recurring scans з auto-редакцією (Actonic); space-level scan → classify → trigger Automation (Polymetis); real-time per-save scanning (miniOrange, Compliance Glossary).
3. **Що вони НЕ вирішують:** жоден із самльованих apps не поєднує "PII-виявлення" з **одноразовим legacy-cleanup проєктом** (на відміну від recurring-моніторингу) — усі продаються як continuous-compliance підписки, не як разовий "приберіть стару wiki" сервіс/інструмент. Це не підтверджено прямим customer evidence (жоден клієнт цього явно не просив) — тому це NEEDS EVIDENCE спостереження, не підтверджена гіпотеза.
4. **Чи є вузький job, не покритий existing apps?** За зібраними доказами — ні, для буквально сформульованої гіпотези "bulk/default PII classification." Єдина залишкова, неперевірена ідея — "разовий legacy PII cleanup" як інша товарна форма (не підписка), але це спекуляція без клієнтського підтвердження.
5. **Чи можна вирішити однією вузькою feature set?** Гіпотетично так, але сама feature set (bulk scan+classify) вже не унікальна.
6. **Forge-first без external data egress?** Так, це вже стандарт категорії — AppFox, Polymetis, miniOrange усі явно заявляють Forge-native/no-data-leaves-instance. Не диференціатор.
7. **Security/privacy burden:** Високий за замовчуванням для всієї категорії (сканування чутливого контенту користувачів) — усі серйозні гравці інвестують у SOC 2/Bug Bounty/Trust Center; новий entrant без цього стартує в невигідній позиції довіри.
8. **Support burden:** MEDIUM-HIGH (не змінилось з Phase D) — bulk-дії на клієнтському контенті.

**EXISTING SOLUTIONS** → AppFox (bulk+enforce+access-control), Actonic (scheduled scan+redact+consent), Polymetis (automation-triggered scan+classify), miniOrange (real-time, scheduled "coming soon") — 4 прямих, активно розвинутих конкуренти покривають майже весь заявлений job.

**UNMET JOB** → Не знайдено в межах буквальної гіпотези. Єдина неперевірена, спекулятивна альтернатива — "разовий legacy-cleanup" як окремий товар (не підписка) — без жодного прямого клієнтського запиту на це.

**MINIMAL WEDGE** → Немає обґрунтованого мінімального wedge для заявленої гіпотези.

**WHY USER WOULD INSTALL** → Не встановлено доказами (job вже закритий конкурентами).

**WHY USER WOULD PAY** → Не встановлено доказами.

**SUPPORT TRAP** → MEDIUM-HIGH (характерно для всієї категорії, не специфічно для гіпотези).

**SECURITY/API TRAP** → Категорія вимагає читання/зміни всього корпоративного Confluence-контенту — це сам по собі high-trust bar; новий entrant без track record матиме високий поріг довіри клієнтів (compliance officers за визначенням обережні).

**BUILD COMPLEXITY** → Помірна технічно (Confluence REST/Forge API добре документовані для search/labeling), але конкурентний бар'єр (довіра, track record, сертифікації) високий.

**REJECT REASON** → **Feature вже існує, повністю або майже повністю, у щонайменше 3 активно підтримуваних конкурентів** (AppFox, Actonic, Polymetis), включно з bulk CQL-scoped операціями, scheduled-сканами, і automation-тригерами. Пряма інструкція проекту: "Особливо заборонено називати bulk classification 'wedge', якщо feature уже є у конкурентів" — застосовано буквально.

**Verdict: KILLED.**

---

### Кандидат 2: HubSpot ↔ Jira — "reliable field-type sync"

**Досліджено 7 existing integrations** (дата перевірки 2026-09-19):

| App | Vendor | Installs/Reviews | Sync scope | Field types | Auth | Sync conflict/retry |
|---|---|---|---|---|---|---|
| [HubSpot CRM Integration for Jira](https://marketplace.atlassian.com/apps/1226482/hubspot-crm-integration-for-jira?hosting=cloud&tab=overview) | Appsvio | 379 / 9 | Read-only: HubSpot-дані (deals/companies/contacts) на Jira-issue; two-way visibility (Jira-дані видно в HubSpot без Jira-доступу) | Custom fields, HubSpot Object Picker (single/multi-select) | OAuth (Atlassian-managed) | Не описано детально |
| [HubSpot CRM Connector for Jira](https://marketplace.atlassian.com/apps/1227969/hubspot-crm-connector-for-jira?hosting=cloud&tab=overview) | Presago | 225 / 4 | Sync contacts/companies/deals/tickets → Jira issues; custom filtered views | Не деталізовано | Не деталізовано | Не деталізовано |
| [HubSpot Integration for Jira FORGE](https://marketplace.atlassian.com/apps/1231637/hubspot-integration-for-jira-hubspot-connector-forge?hosting=cloud&tab=overview) | Getint | 144 / 4 | **Повний two-way sync**: коментарі, нотатки, статуси, вкладення, контакти, угоди, кастомні поля; гнучкий field mapping і напрямок синхронізації | Custom fields — **але відомий gap**: multi-select і date fields не підтримувались (Phase D, Anne Dietz, тип **B**); changelog Sep 2026 показує continuous fixes для date/query/attachment-полів **у всіх** інтеграціях Getint (Asana DUE field, ClickUp custom queries, Freshservice attachments) — це системна, не HubSpot-специфічна проблема архітектури мульти-платформного конектора, що активно закривається | OAuth/API token (Forge) | Не деталізовано; активний bug-fix cadence (щомісячні релізи) |
| [HubSpot Connector for Jira](https://marketplace.atlassian.com/apps/2205524648/hubspot-connector-for-jira?hosting=cloud&tab=overview) | Korvex Systems | 457 / 0 | **Display-only, one-way, або two-way — на вибір**, per-item конфігурація; status/comment/attachment sync toggles окремо | Field mappings (деталі невідомі) | Private app token | **Scheduled sync кожні 5 хвилин** + event-triggered push на Jira issue/comment/attachment events — конкретна, задокументована retry/sync-cadence модель |
| [HubSpot CRM for Jira](https://marketplace.atlassian.com/apps/1228240/hubspot-crm-for-jira-report-issue-link-collaboration?hosting=cloud&tab=overview) | resolution Reichert | 490 / 11 | **Embed + automation-trigger**, не full sync: показ Contacts/Companies/Deals у Jira-issue; тригер створення/лінкування HubSpot-об'єктів на основі Jira-даних; HubSpot лишається "single source of truth" | Не деталізовано | Не деталізовано | Перша версія app ("first version of this app") — вже 490 installs/11 reviews, гарна traction для v1 |
| [HubSpot Integration for Jira (Bidirectional Sync)](https://marketplace.atlassian.com/apps/1238418/hubspot-integration-for-jira-bidirectional-sync?hosting=cloud&tab=overview) | OpsHub, Inc. | — / 1 (5/5) | Enterprise-grade, **зовнішній** (не Forge-плагін, працює через secure API, cloud/on-prem/hybrid deployment), no/low-code field mapping, sync CRM+dev workflows за бізнес-логікою | Deals, Tickets, Contacts, Notes, Tasks + коментарі/вкладення/статуси | Secure API (зовнішній, не Atlassian OAuth) | **Явно задокументована eventual-consistency модель з error recovery**; окрема фіча — **"Excel-based user mapping — no more sync failures from user mismatches"** — прямий доказ (vendor-побудована фіча), що user/field mismatch — це визнана, повторювана категорія проблем у ніші (тип **C**, vendor-inferred) |
| HubSpot's власна нативна інтеграція (knowledge.hubspot.com) | HubSpot | — | Офіційна, безкоштовна HubSpot↔Jira інтеграція існує від самого HubSpot | — | — | Пряма конкуренція з платформи-власника даних — додатковий platform-risk |

**Відповіді на контрольні питання:**

1. **5-10 existing integrations:** 7 прямих + 1 нативна від HubSpot = 8 знайдено.
2. **Exact sync scope:** покрито все: full two-way (Getint), configurable two-way/one-way/display-only (Korvex), read-only display (Appsvio), embed+automation-trigger (resolution), enterprise external no-code (OpsHub), нативна безкоштовна (HubSpot).
3. **Supported field types:** переважно "custom fields" загалом; підтверджений конкретний gap (multi-select, date) лише в одному конкуренті (Getint), і цей gap — частина ширшого, системного (мульти-платформного) технічного боргу, що активно закривається щомісячними релізами.
4. **Mapping/configuration complexity:** варіюється від "5 minutes setup" (Getint marketing claim) до enterprise Excel-based mapping (OpsHub) — весь спектр складності вже представлений на ринку.
5. **Common customer complaints:** reliability/installation-баги (Appsvio, resolution — Phase D, тип **D**); відсутність деяких типів полів (Getint, тип **B**); user/field mismatch (непрямо, OpsHub feature, тип **C**).
6. **API dependencies:** усі залежать від HubSpot API (зовнішній, поза Atlassian-екосистемою) + Jira/Forge API — подвійна залежність для будь-якого нового entrant.
7. **Auth/permissions complexity:** OAuth (більшість), private app token (Korvex), secure API зовнішній (OpsHub) — стандартний спектр, не є диференціатором.
8. **Sync conflict/retry:** тільки 2 з 7 (Korvex, OpsHub) явно документують конкретну модель (5-хв cron / eventual consistency) — це справді слабко задокументована зона в категорії загалом, але не є "unmet job", а деталь реалізації.
9. **Support burden:** підтверджено високий за структурою категорії (customer-specific field mapping, залежність від зовнішнього API).
10. **Чи можна звузити до одного вузького workflow?** Спробовано: "тільки read-only показ CRM-контексту в Jira" — **вже є** (Appsvio, Korvex display-only mode). "Тільки embed + automation-trigger, без sync" — **вже є** (resolution, і це "перша версія", отже свіжий, підтверджений напрямок з хорошою traction). Кожна спроба звуження впирається в existing app, що вже займає саме цю вузьку нішу.

**EXISTING SOLUTIONS** → 7 прямих конкурентів + нативна HubSpot-інтеграція покривають повний спектр: full two-way, конфігурований two-way/one-way/display-only, read-only, embed+automation-trigger, enterprise no-code external.

**UNMET JOB** → Не знайдено вузького, не зайнятого workflow. Кожна спроба звузити scope (read-only, embed-only, display-only) вже реалізована щонайменше одним активним конкурентом.

**MINIMAL WEDGE** → Немає life обґрунтованого мінімального wedge, що одночасно (а) вузький, (б) не порушує вимогу "не повноцінна two-way integration", і (в) не вже зайнятий.

**WHY USER WOULD INSTALL** → Не встановлено доказами для нового, відмінного від існуючих, продукту.

**WHY USER WOULD PAY** → Не встановлено доказами.

**SUPPORT TRAP** → HIGH (підтверджено з Phase D) — не змінилось: integration-категорія структурно генерує customer-specific конфігурацію і залежить від чужого (HubSpot) API.

**SECURITY/API TRAP** → HIGH — подвійна зовнішня залежність (HubSpot API + Jira/Forge API); HubSpot може змінити API без узгодження з Atlassian-екосистемою; жоден з існуючих конкурентів не документує чіткий SLA щодо breaking changes.

**BUILD COMPLEXITY** → Висока: інтеграційна категорія за визначенням вимагає підтримки двох незалежних, зовнішньо-керованих API, і конкуренти вже покрили весь спектр архітектурних підходів (Forge-native, зовнішній сервіс, гібрид).

**REJECT REASON** → **Кожна вузька конфігурація вже зайнята активним конкурентом**, а сам конкретний evidence-based gap (field-type completeness) — це якість виконання наявного продукту (і вже активно виправляється постачальником), а не новий, незайнятий job. Пряма інструкція проекту ("не пропонуй повноцінну two-way integration") звужує можливий wedge до підмножини, яка вже цілком заповнена (read-only/display-only/embed-trigger).

**Verdict: KILLED.**

---

### Підсумок Phase E

| Гіпотеза | Verdict | Головна причина |
|---|---|---|
| GDPR/Confluence bulk PII classification | **KILLED** | Feature вже реалізована (bulk+scheduled+automated) щонайменше у 3 активних, добре задокументованих конкурентів |
| HubSpot↔Jira reliable field-type sync | **KILLED** | Кожна можлива вузька конфігурація (read-only/display-only/embed-trigger/full two-way/enterprise no-code) вже зайнята активним конкурентом; сам evidence-gap — якість виконання, що конкурент активно виправляє |

**Обидві гіпотези з Phase D не пережили kill test.** Це чесний, а не невдалий результат: методологія (AGENTS.md §5, Veto rules: "Wedge = veto") явно передбачає, що відсутність wedge зупиняє прогрес до BUILD, і не повинна компенсуватися рештою плюсів (реальний попит із Phase C, значна кількість позитивних відгуків тощо). Жоден з двох кандидатів не проектувався в MVP чи architecture — обидва зупинені на стадії гіпотези.

**Наслідок для подальшого research:** оскільки обидві активні гіпотези вбиті, а `confluence page views analytics` на `HOLD` без конкретного unmet job, проект наразі не має жодного живого wedge-кандидата на Atlassian Marketplace серед 3 intent, досліджених у Phase C/D. Наступний крок — не BUILD і не REJECT усього напрямку Atlassian, а повернення до ширшого пулу intent з Phase B1 (WEAK-класифіковані або ще не досліджені) для пошуку нового кандидата з підтвердженим unmet job, або поглиблене повторне дослідження HOLD-інтенту, коли з'явиться конкретний job. Це рішення явно НЕ приймається в цьому документі — очікує вказівки користувача.

### Phase F — Fresh Keyword Expansion (executed 2026-09-20)

**Мета:** знайти нові customer-intent queries на Atlassian Marketplace, що можуть вести до вузького solo micro-SaaS wedge, явно оминаючи 3 закриті теми: (а) GDPR bulk PII classification, (б) HubSpot↔Jira integration, (в) `confluence page views analytics` (HOLD). Перевірено 35 нових queries за патернами `automatically.../bulk.../validate.../enforce.../prevent.../notify.../clean.../compare.../export.../detect.../find...`.

**Обмеження методу (чесно задокументовано):**
- Atlassian Marketplace search завжди показує "Showing over 1,000 matches for your query" незалежно від фактичної релевантності — це поле не є дискримінуючим сигналом і в таблиці нижче опущено як марно однакове для всіх 35 запитів.
- Payment model (paid/free/freemium) не видно на сторінці результатів пошуку — тільки на сторінці конкретного застосунку (`tab=overview`, блок "Version information"). Перевірка цього поля для всіх ~175 застосунків (35 query × 5 апps) вимагала б у 5 разів більше запитів, ніж бюджет цієї фази дозволяє. Тому в таблиці нижче Pricing позначено як `NEEDS VERIFICATION`, окрім випадків, коли слово "Free" прямо в назві застосунку.

**Повна таблиця (35 queries, перший прохід):**

| # | Query | Top apps (installs, rating) | Small/new entrant visible? | Badges (RISING STAR/SPOTLIGHT/BESTSELLER) | External dependency | Initial verdict |
|---|---|---|---|---|---|---|
| 1 | automatically archive inactive projects jira | Projectrak (1.3k, 4.5); Deep Clone (11.9k, 4.5) | Ні (generic PPM/user-mgmt reuse) | Немає | Немає | WEAK |
| 2 | automatically archive stale confluence pages | Better Content Archiving (1.2k, 4.8); Automatic Archiving for Confluence Cloud (19, 5.0); Stale Page Finder (3, —) | Так (2 tiny apps) | Немає | Немає | WEAK — сильний incumbent (1.2k) вже займає нішу |
| 3 | automatically assign reviewer jira | SnapAssign (61, 5.0); Smart Assignments & Rotations (104, 4.4) | Так | Немає | Неоднозначно (Jira-native QA reviewer LOW vs. PR/code reviewer HIGH — потребує Bitbucket/GitHub) | NEEDS EVIDENCE |
| 4 | automatically close stale issues jira | Sprint Automation Auto Start/Close (90, 5.0) — лише для sprint, не для issue staleness взагалі | Так | Немає | Немає | NEEDS EVIDENCE |
| 5 | automatically label issues by content jira | Advanced Label Manager (1.4k, 4.0); Label Manager (747, 4.3) | Ні | Немає | Можливо (AI content-based labeling = LLM API) | WEAK |
| 6 | bulk close subtasks jira | Deep Clone (11.9k, 4.5); Bulk Clone Professional (699, 4.7) | Ні | Немає | Немає | REJECT — насичено |
| 7 | bulk delete old attachments confluence | GoEdit (834, 4.8); Cenote Lockpoint (788, 4.9) | Частково | Немає | Немає | WEAK |
| 8 | bulk move issues between projects jira | Deep Clone (11.9k); Elements Copy & Sync (2.4k, 4.7) | Ні | Немає | Немає | REJECT |
| 9 | bulk update custom field jira | Jira Misc Custom Fields/JMCF (3.3k, 4.8, Appfire) | Ні | Немає | Немає | REJECT — зрілий ринок |
| 10 | bulk user management | User Mgmt for Jira (865, 4.8); Manage Users for Jira Cloud (935, 3.4) | Частково | Немає | Немає | REJECT |
| 11 | clean broken links confluence | Link Management (575, 4.4); GitHub links (704, 3.8); Link Steward (NEW, 0 installs) | Так (Link Steward щойно запущений) | Немає (NEW label) | Немає | WEAK — середні incumbents вже займають |
| 12 | clean inactive users jira | miniOrange auto-deactivation (252, 5.0); Manage Users for Jira Cloud (935, 3.4) | Частково | Немає | Немає | WEAK |
| 13 | clean orphaned pages confluence | Немає прямого відповідника — топ apps: generic approval/formatting tools | — | Немає | — | REJECT — query не мапиться на реальний продукт |
| 14 | compare confluence page versions | Compare Any Two Pages — Visual Diff (1 install, RUNS ON ATLASSIAN, щойно запущений); Version Info (106, 5.0) | Так (майже pre-traction) | Немає | Немає | **PROMISING** |
| 15 | detect duplicate pages confluence | Немає прямого відповідника (Compliance for Confluence — інший job: DLP/sensitive data) | Ні | Немає | Можливо (text-similarity потребує ML) | NEEDS EVIDENCE |
| 16 | enforce definition of done jira | ReDo (11, 5.0); Definition of Done & Ready (2, —); Definition of Ready (4, 5.0); Definition of Done (63, 2.8 — низький рейтинг) | Так (4 незалежні спроби) | Немає | Немає | **PROMISING** |
| 17 | enforce naming convention jira | Немає dedicated app — топ: ScriptRunner (34.8k, generalist), Elements Connect (2.6k, generalist) | Ні | Немає | Немає | WEAK — вже вирішується generalist-платформами |
| 18 | enforce page template confluence | Scaffolding Forms & Templates (1.3k, 4.4, Appfire); Page Tree Creator Pro (818, 4.7) | Ні | Немає | Немає | REJECT |
| 19 | enforce required fields jira | JMCF (3.3k); Elements Connect (2.6k); easeRequirements (2k) | Ні | Немає | Немає | REJECT — зрілий ринок |
| 20 | export confluence space to word | Scroll Word Exporter (4.7k, 4.9, BESTSELLER); Scroll PDF Exporter (8.9k, BESTSELLER) | Ні | BESTSELLER×2 | Немає | REJECT |
| 21 | export jira issues to excel | Better Excel Exporter (4.4k, SPOTLIGHT); Xporter (3.8k) | Ні | SPOTLIGHT | Немає | REJECT |
| 22 | export jira sprint report to excel | Better Excel Exporter (4.4k, SPOTLIGHT); eazyBI (11k, BESTSELLER) | Ні | SPOTLIGHT+BESTSELLER | Немає | REJECT |
| 23 | find unassigned issues jira | Пошук повертає duplicate-detection apps — mismatch; ймовірно, задача вирішується нативним JQL-фільтром | — | — | — | WEAK — можливо, немає ринку через нативне рішення |
| 24 | find unused custom fields jira | **0 apps знайдено взагалі** (порожня видача) | Н/Д — жоден конкурент не існує | — | Немає | NEEDS EVIDENCE (див. застереження нижче) |
| 25 | notify manager before deadline jira | Reminder for Jira (1.2k, 4.5) | Частково | Немає | Немає | WEAK |
| 26 | notify slack on sla breach jira | Time to SLA (3.4k, SPOTLIGHT); SLA Time and Report (772, 4.5) | Ні | SPOTLIGHT | Так (Slack API) | REJECT |
| 27 | notify watchers on comment jira | Mentions Dashboard (65, 5.0); Smart Comments (159, 4.8) | Частково | Немає | Немає | WEAK |
| 28 | prevent accidental page deletion confluence | "Who Deleted My Page(s)?" (2, —) — audit-only, не prevention | Так (tiny) | Немає | Немає | NEEDS EVIDENCE |
| 29 | prevent duplicate issue creation jira | Find Duplicates (175, 4.9, 48 reviews) — сильний вузький incumbent | Частково | Немає | Немає | WEAK — ніша вже добре обслуговується одним лідером |
| 30 | prevent issue reopening jira | Reopening Counter (48, 3.5) — лише tracking, не gate; Reopen Receipt (щойно запущений) | Так | Немає | Немає | **PROMISING** (з застереженням) |
| 31 | prevent sprint start without estimation jira | SprintPoker (669, RISING STAR); Agile Poker (1.9k) | Ні | RISING STAR | Немає | WEAK — насичений ринок estimation-apps |
| 32 | validate acceptance criteria jira | Acceptance Criteria for Jira Free (1.1k, 4.0); кілька tiny AI-клонів (0-8 installs) | Так (багато, фрагментовано) | Немає | Можливо (AI-generation = LLM API) | WEAK |
| 33 | validate confluence page before publish | Comala Publishing (1.3k, 4.9, Appfire); AURA/KARMA suite | Ні | Немає | Немає | REJECT |
| 34 | validate issue before transition jira | Create on Transition (1.1k, 4.7, Appfire); Undo Transition (154, 4.5) | Частково | Немає | Немає | WEAK |
| 35 | validate story points before sprint start jira | Результати нерелевантні (Story Maps, SharePoint Connector) — низький сигнал query | — | — | — | REJECT |

**Спостереження щодо badges:** RISING STAR/SPOTLIGHT/BESTSELLER зустрічаються виключно у великих, вже встановлених гравців (Appfire, K15t, eazyBI, Agile Pulse) — жоден з badge не з'явився серед вузьких/малих кандидатів. Це підтверджує, що Marketplace-просування концентрується навколо incumbents, а не є сигналом про нові ніші.

### First-pass narrowing (35 → 8)

За критеріями "чіткий, специфічний job-to-be-done" + "не вирішується вже native-функцією платформи або generalist-інструментом" + "хоча б слабкий сигнал повторюваного попиту" відібрано 8 кандидатів:

| Query | Verdict (первинний) | Architecture Fit |
|---|---|---|
| enforce definition of done jira | PROMISING | LOW (Forge-native workflow validator) |
| prevent issue reopening jira | PROMISING (із застереженням) | LOW |
| compare confluence page versions | PROMISING (із застереженням) | LOW |
| find unused custom fields jira | NEEDS EVIDENCE | LOW |
| automatically assign reviewer jira | NEEDS EVIDENCE | НЕВИЗНАЧЕНО (LOW якщо Jira-native reviewer; HIGH якщо PR/code reviewer через Bitbucket/GitHub) |
| detect duplicate pages confluence | NEEDS EVIDENCE | MEDIUM (text-similarity, ймовірно потребує зовнішній ML API) |
| enforce naming convention jira | WEAK/NEEDS EVIDENCE | LOW номінально, але є generalist-substitute risk (ScriptRunner) |
| prevent accidental page deletion confluence | NEEDS EVIDENCE | LOW |

### Second-pass narrowing (8 → 3)

Для кожного з 8 перевірено: paid demand, real installs, active competitors, smaller/new entrant presence, clear customer intent, Architecture Fit, очікуваний support burden.

**enforce definition of done jira** → 4 незалежні спроби (ReDo, Definition of Done & Ready, Definition of Ready, Definition of Done) — це саме той патерн "кілька малих гравців атакують ту саму вузьку задачу, ніхто не робить це добре" (installs 2–63, один з великою кількістю встановлень має низький рейтинг 2.8/5). Definition of Done — стандартна, добре зрозуміла Scrum-термінологія → чіткий customer intent. Architecture Fit LOW. Support burden — MEDIUM (workflow gate, що блокує transition, вимагає продуманого UX для винятків). **Висновок: переходить у топ-3.**

**prevent issue reopening jira** → обидва існуючі конкуренти (Reopening Counter, Reopen Receipt) вирішують сусідню, але іншу задачу — вони **вимірюють/трекають** повторні відкриття, а не **блокують** їх. Це може означати або (а) справжню незайняту нішу для hard-gate рішення, або (б) що реальні клієнти свідомо не хочуть жорсткого блокування (сприймається як каральне/тертя) і тому обидва конкуренти обрали visibility-only підхід. Support burden HIGH (workflow-blocker завжди генерує термінові тікети при збої; політично чутливо — команди можуть опиратися "гейтуванню"). **Висновок: переходить далі, але з явним відкритим питанням для Pain/Switching фази — чи клієнти справді хочуть "prevent", чи тільки "track".**

**compare confluence page versions** → практично нульова конкуренція (1 install, pre-traction), але Confluence вже має нативне порівняння сусідніх версій — отже, реальний unmet job вужчий за формулювання запиту (порівняння несуміжних версій або крос-сторінкове порівняння). Architecture Fit LOW, support burden LOW (read-only). **Висновок: переходить у топ-3, з explicit застереженням про ризик перетину з нативною функцією платформи.**

**find unused custom fields jira** → НАЙСИЛЬНІШИЙ сигнал "порожньої ніші" (0 конкурентів), але саме тому НЕ переноситься автоматично в топ-3: нуль конкурентів так само добре пояснюється тим, що ніхто не готовий платити за це, як і тим, що це незайнята територія. Проектне правило прямо забороняє висновок "мало/нуль конкурентів = хороша ніша" без додаткових доказів. Custom field bloat — відома біль в Jira admin спільнотах (Atlassian Community, Reddit) поза межами Marketplace-даних, але це зовнішній доказ, не перевірений у цій фазі. **Висновок: НЕ входить у фінальні 3 без додаткового зовнішнього підтвердження попиту; залишається як окремо задокументована ідея для майбутнього раунду.**

**automatically assign reviewer jira** → відсікається через нерозв'язану двозначність job-to-be-done (Jira-native reviewer vs. PR/code reviewer з Bitbucket/GitHub) — Architecture Fit не може бути оцінений, доки не уточнено буквальний job.

**detect duplicate pages confluence** → відсікається через Architecture Fit MEDIUM (ймовірна потреба в text-similarity/ML) у поєднанні з повною відсутністю навіть слабкої спроби конкурента (гірша комбінація, ніж "0 конкурентів + LOW fit").

**enforce naming convention jira** → відсікається: це не порожня ніша, а ніша, вже вирішувана generalist-платформами (ScriptRunner, 34.8k installs) для тих, кому це дійсно важливо — ризик "рішення вже існує, просто не як окремий продукт".

**prevent accidental page deletion confluence** → відсікається: Confluence Cloud вже має нативний kошик/відновлення протягом 60 днів, що суттєво звужує реальний unmet job до вузької підмножини (напр., permission-based delete-blocking для окремих просторів), а не widescale "prevention".

### Фінальні 3 кандидати, що переходять у Pain/Switching дослідження

1. **enforce definition of done jira** (Jira workflow-gate, що блокує transition до виконання DoD-чеклиста)
2. **prevent issue reopening jira** (з відкритим питанням: "prevent" hard-gate vs. "track" visibility-only)
3. **compare confluence page versions** (з відкритим питанням: наскільки нативна функція Confluence вже покриває цю потребу)

Жоден кандидат не обраний як продукт, MVP чи архітектура не проектувались, числового скорингу не використано.

## F2. Phase G — Native Capability Kill Test (executed 2026-09-20)

**Мета:** не феча-порівняння заради документації, а спроба ЗНИЩИТИ кожного з 3 кандидатів Phase F, встановивши: чи потребує заявлений job стороннього Marketplace app взагалі, чи Jira/Confluence вже закриває його native (workflow conditions, validators, forms, required fields, automation, transition restrictions, native version history/compare).

---

### Кандидат 1: `enforce definition of done jira`

**NATIVE CAPABILITY** →
- **Field Required Validator** — блокує transition, якщо конкретне обране поле порожнє. Офіційний шлях: Project settings → Workflows → редагувати workflow → обрати transition → Add validator → Field Required Validator → обрати поле → error message → publish. ("users won't be able to complete the transition to the 'Closed' status if the required field is empty.") (https://support.atlassian.com/jira/kb/mandatory-field-validation-for-issue-closure-in-jira-cloud/, перевірено 2026-09-20)
- **Умови (Conditions)**: Permission Condition, User/Group/Role Condition, Value Field Condition (transition дозволено лише якщо поле = певне значення), Previous Status Condition. (https://support.atlassian.com/jira-cloud-administration/docs/configure-advanced-issue-workflows/, перевірено 2026-09-20)
- **Sub-Task Blocking Condition** — окрема нативна умова, що блокує закриття батьківського issue, поки є відкриті subtasks (тільки Company-managed проекти; недоступна в Team-managed). (https://support.atlassian.com/jira/kb/how-to-prevent-issues-from-being-closed-while-the-sub-tasks-are-still-open-in-jira/, перевірено 2026-09-20)
- Кілька Field Required Validators можна додати на один transition (по одному на поле) — стандартна поведінка редактора workflow дозволяє кілька validators на transition; офіційна документація не описує явно "stacking" кількох validators як єдину фічу, тому це помірно впевнений висновок з UI-поведінки, а не пряма цитата.

**NATIVE LIMITATION** →
- Немає нативного **checklist field type**: Jira Cloud взагалі не має вбудованого чекліста як типу поля. ("Jira doesn't come with a built-in checklist feature, so you will need to use a third-party app from the Atlassian Marketplace." — Atlassian Community, перевірено 2026-09-20)
- Field Required Validator перевіряє одне окреме поле; немає єдиного нативного механізму "N з M критеріїв виконано" (структурований DoD-чекліст із частковим прогресом, підпунктами, шаблонами per issue type).
- Post-functions виконуються ПІСЛЯ transition і не можуть блокувати його.

**Висновок:** це чітке підтвердження різниці, яку просив користувач — `basic transition gating` (одне-два обов'язкові поля через Field Required Validator) є нативним; `structured Definition-of-Done enforcement` (багатопунктовий чекліст з validator-гейтом, шаблонами, частковим прогресом) — НЕ є нативним і вимагає app.

**EXISTING MARKETPLACE SOLUTIONS** → залишковий gap (checklist + validator gating) вже щільно закритий, і не малими гравцями:
| App | Vendor | Installs/Reviews/Rating | Що саме робить |
|---|---|---|---|
| [Checklists for Jira (Pro)](https://marketplace.atlassian.com/apps/1213231/checklists-for-jira-pro-by-herocoders) | HeroCoders | **7,887 / 264 / 4.5** | Явно позиціонується для DoD: "Execute workflows with automated Jira checklists... to enforce DoD and acceptance criteria"; має власні checklist workflow validators, що блокують transition, поки чекліст не завершено. |
| [Enterprise Checklists for Jira](https://marketplace.atlassian.com/apps/2171539829/enterprise-checklists-for-jira) | Cognitiff | 1 review / 5.0 (installs не розкрито) | "native workflow validators" явно блокують transition ("Automatically block issue transitions... until every single checklist item is completed"); також audit trail з CSV export, JQL-ready progress fields. |
| [Definition of Done](https://marketplace.atlassian.com/apps/1215779/definition-of-done) | Chasing Agility | 63 / 4 / 2.8 | Буквально названий "Definition of Done"; workflow validator блокує transition до Done, поки критерії (checklist/bullet list) не виконані; пошук по JQL за статусом виконання. |

(усі три перевірені 2026-09-20 напряму на сторінках marketplace.atlassian.com)

Це суттєво доповнює/корегує Phase F: Phase F знайшов лише 4 малих, слабко виконаних apps (2–63 installs) за буквальним пошуком "definition of done" / "DoD" у назві, але не врахував ширшу категорію "Checklist for Jira", яка функціонально вирішує той самий job і має домінантного гравця з майже 8 тисячами встановлень.

**REAL UNMET JOB** → Не знайдено в межах буквального запиту. Job "checklist, що блокує transition, поки DoD не виконано" вже реалізований, добре відпрацьований і активно продається щонайменше 3 конкурентами, один з яких — домінантний incumbent (7,887 installs). Спекулятивна, неперевірена вузька альтернатива (напр., DoD-шаблони, прив'язані вузько до однієї regulated-галузі, або дуже спрощений single-purpose app без повного checklist-фреймворку) не підтверджена жодним клієнтським доказом — це НЕ рятує кандидата, лише фіксується як неперевірена ідея.

**MINIMAL POSSIBLE WEDGE** → Немає обґрунтованого мінімального wedge: будь-яка вузька версія "checklist + validator gate" вже є частиною функціоналу incumbent (HeroCoders) і кількох менших конкурентів.

**SUPPORT RISK** → MEDIUM (workflow-blocker вимагає продуманого UX для винятків/override, інакше генерує термінові тікети "чому я не можу закрити issue").

**PLATFORM RISK** → LOW (Field Required Validator + custom workflow validator module — стандартний, добре задокументований Forge/Connect механізм; https://developer.atlassian.com/cloud/jira/platform/modules/workflow-validator/, перевірено 2026-09-20).

**VERDICT: KILLED.**

---

### Кандидат 2: `prevent issue reopening jira`

**NATIVE CAPABILITY** → Native покриває майже весь заявлений job:
1. **Повне блокування** — просто не додавати transition з Closed назад у відкритий статус (структурна зміна workflow, без app).
2. **Обмеження для конкретних users/groups** — Permission Condition / User-Group-Role condition на transition (Company-managed); а також окрема нативна рула **"Restrict who can move a work item"** — доступна і в Team-managed проектах, дозволяє обрати assignee/reporter/конкретного користувача/role/group/permission. (https://support.atlassian.com/jira-service-management-cloud/docs/available-workflow-rules-in-team-managed-service-projects/, перевірено 2026-09-20)
3. **Time-limited reopen** — **Date Compare Validator** (Company-managed): напр. `Resolved > -14d`, дозволяє reopen лише протягом 15 днів після резолюції. (https://support.atlassian.com/jira/kb/limit-customer-issue-reopening-to-x-days-after-resolution/, перевірено 2026-09-20)
4. **Conditional reopen** — Value Field Condition (transition дозволено лише якщо задане поле має конкретне значення).
5. **Auditability** — issue history/activity log нативно показує всі виконані (успішні) transitions, включно з reopen, разом з автором і часом.
6. **JSM customer portal edge case** — офіційна документація прямо визнає обмеження: "Transitions executed from the Jira Service Management Portal ignore validators" — і прямо рекомендує нативну (безкоштовну) **automation rule** замість validator для цього випадку: перевірка `{{now.diff(issue.resolved).days}}` і додавання коментаря-відмови, якщо умова не виконана. Це теж нативний, безкоштовний механізм (Jira automation), не Marketplace app. (той самий source, перевірено 2026-09-20)

**NATIVE LIMITATION** →
- Team-managed проекти НЕ підтримують Date Compare Validator і Value Field Condition (складні transition validators/conditions) — доступна лише базова роль/користувач-рестрикція через "Restrict who can move a work item". Тобто *time-limited* і *conditional-by-field* reopen-обмеження в Team-managed проектах нативно недоступні (лише via automation rule, реактивно, а не як hard validator). (https://community.atlassian.com/forums/Jira-questions/I-have-a-team-managed-project-and-would-like-to-set-up/qaq-p/2180767, перевірено 2026-09-20)
- Немає нативного audit trail для **заблокованих спроб** reopen (Jira логує тільки успішні transitions, не спроби, яким умова відмовила).
- Немає нативного **звіту про кількість повторних reopen** на issue/проект: JQL підтримує оператор `WAS` (issue був у певному статусі хоча б раз), але не рахує, скільки разів. Це підтверджено прямо: "native Jira lacks a built-in report to count reopenings... You'll need a marketplace app." (https://community.atlassian.com/forums/App-Central-articles/How-to-Find-and-Analyse-Reopened-Issues-in-Jira/ba-p/2732595, перевірено 2026-09-20)

**EXISTING MARKETPLACE SOLUTIONS** → сам залишковий gap (підрахунок/звітність reopen) уже закритий двома різними шляхами:
| App | Vendor | Installs/Reviews/Rating | Що робить |
|---|---|---|---|
| [Reopening Counter for Jira](https://marketplace.atlassian.com/apps/1212789/reopening-counter-for-jira) | Rozdoum | 48 / 11 / 3.5 (Cloud доступний) | Dashboard gadget + issue-view лічильник кількості reopen на issue; візуалізація "проблемних" issues/команд. |
| [Timepiece – Time in Status for Jira](https://marketplace.atlassian.com/apps/1211756/timepiece-time-in-status-for-jira) | OBSS | **4,477 / 270 / 4.8** | Генералістський звітний застосунок; має "Status Count report", що явно виявляє "reopens and rework loops" через підрахунок відвідувань статусу — reopen-звітність тут лише один з 15+ типів звітів, не окремий продукт. |

(обидва перевірені 2026-09-20)

**REAL UNMET JOB** → Для рамки "prevent/block" (буквальний запит) — job вже вичерпно вирішений native (повне блокування, рестрикція за роллю/групою навіть у Team-managed, time-limit і умовний гейт у Company-managed, automation-based обхід для JSM порталу). Це прямий збіг з попередженням користувача: "Не називай `prevent reopen` wedge, якщо native workflow already handles the exact job." Залишковий, вужчий job — **зручна, готова reopen-аналітика/звітність** — це вже ІНША задача (не "prevent", а "measure"), і вона вже покрита і нішевим (Reopening Counter, 48 installs), і великим генералістським incumbent (Timepiece, 4,477 installs).

**MINIMAL POSSIBLE WEDGE** → Немає обґрунтованого мінімального wedge для заявленої "prevent reopening" гіпотези; вужча "reopen-only analytics" ніша технічно ще не насичена спеціалізованим гравцем з великою тракцією, але це вже інший job-to-be-done, не той, що досліджувався, і згадується тут лише для повноти, а не як спроба штучно врятувати кандидата.

**SUPPORT RISK** → HIGH (підтверджено з Phase F) — workflow-блокер, що спрацьовує невірно, генерує термінові, високовидимі тікети; це не змінюється тим, що механізм нативний чи сторонній.

**PLATFORM RISK** → LOW-MEDIUM — усі задіяні механізми (Conditions, Validators, "Restrict who can move a work item", Automation) — стандартні, добре задокументовані нативні Jira Cloud фічі; ризик радше в Team-managed/Company-managed feature-parity (описано вище), ніж у самій платформі.

**VERDICT: KILLED** (для буквальної "prevent/block reopening" гіпотези — native вже вирішує цей job; залишкова "reopen analytics" — інший, вже зайнятий job, не еквівалент початкової гіпотези).

---

### Кандидат 3: `compare confluence page versions`

**NATIVE CAPABILITY** →
- **Version History**: доступна через More actions → Version history на будь-якій сторінці.
- **Compare selected versions**: користувач відмічає чекбоксами будь-які **дві довільні версії** (не обов'язково суміжні, напр. версію 2 і версію 10) і натискає "Compare selected versions". (https://confluence.atlassian.com/doc/page-history-and-page-comparison-views-139379.html, перевірено 2026-09-20 — документація Data Center/Server-lineage, але описаний UI-патерн підтверджується і в Cloud-орієнтованих сторонніх джерелах, напр. community-форум "Compare versions of the same page")
- **View changes/diff-вигляд**: додане підсвічено зеленим, видалене — червоним, зміни форматування — синім; великі незмінені блоки тексту згортаються в "…" для читабельності.
- Навігація між сусідніми порівняннями прямо з екрана порівняння (напр., переглядаючи diff версій 30↔34, можна одним кліком перейти до 29↔30 або 34↔35).

**NATIVE LIMITATION** →
- Порівняння обмежене **однією і тією ж сторінкою** — не можна нативно порівняти дві РІЗНІ сторінки (крос-сторінкове порівняння). (https://community.atlassian.com/forums/Confluence-questions/Can-I-compare-different-pages-in-Confluence-Cloud/qaq-p/2081961, перевірено 2026-09-20)
- Great для точкового порівняння вручну обраних версій; немає нативного bulk/масового порівняння версій по багатьох сторінках одразу (згадується як відкрите community-питання: "Confluence bulk page version compare", перевірено 2026-09-20, без офіційного рішення).

**EXISTING MARKETPLACE SOLUTIONS** → жодна з знайдених apps не закриває навіть той вужчий (крос-сторінковий) job по-справжньому:
| App | Vendor | Installs/Reviews/Rating | Що робить |
|---|---|---|---|
| [Diff for Confluence](https://marketplace.atlassian.com/apps/1273931748/diff-for-confluence) | Aptify Tech | 6 / 1 / 5.0 | Порівнює Git-патчі або вручну вставлений текст/код — НЕ версії реальної Confluence-сторінки і НЕ дві різні сторінки автоматично. |
| [diff](https://marketplace.atlassian.com/apps/1233922/diff) | LN Software | 12 / 4 / 5.0 | Те саме — вручну вставлений текст/git-diff/patch-файли, не автоматичне порівняння live-сторінок. |

(обидва перевірені 2026-09-20)

**REAL UNMET JOB** → Буквальний запит `compare confluence page versions` (порівняння версій ОДНІЄЇ сторінки) **повністю закритий native functionality**, включно з довільними (не лише суміжними) версіями — це прямий збіг з правилом користувача: "Якщо literal customer job уже повністю закритий native functionality: KILLED. Без подальшого pain research." Ширший, окремий job — автоматичне крос-сторінкове порівняння (напр., порівняти сторінку з шаблоном, або дві споріднені сторінки в різних просторах) — нативно не підтримується і не вирішений жодним знайденим Marketplace app (обидва існуючі "diff"-apps вимагають ручного вставляння тексту, а не тягнуть live-контент сторінок). Це НЕ підтверджений wedge для буквального кандидата — лише зафіксований як інший, окремий job без будь-якого клієнтського доказу попиту (жодної скарги, review чи запиту, знайденого в цьому проході).

**MINIMAL POSSIBLE WEDGE** → Немає — буквальний job вже вирішено native; крос-сторінковий job — інша, неперевірена гіпотеза без жодного клієнтського доказу.

**SUPPORT RISK** → N/A (буквальний кандидат killed до стадії, де support risk мав би значення).

**PLATFORM RISK** → N/A.

**VERDICT: KILLED.**

---

### Підсумок Phase G

| Кандидат | Verdict | Головна причина |
|---|---|---|
| `enforce definition of done jira` | **KILLED** | Native має лише basic single-field gating (Field Required Validator), не structured checklist — але саме цей gap вже щільно закритий Marketplace-конкурентами, включно з домінантним incumbent (HeroCoders, 7,887 installs), явно позиціонованим під DoD-enforcement. |
| `prevent issue reopening jira` | **KILLED** | Native вичерпно вирішує "prevent/block": повне блокування, рестрикція за роллю/групою (навіть Team-managed), time-limit і умовний гейт (Company-managed), automation-based обхід для JSM-порталу. Залишкова "reopen-analytics" — інший job, вже зайнятий і нішевим (Reopening Counter), і великим генералістським (Timepiece, 4,477 installs) конкурентом. |
| `compare confluence page versions` | **KILLED** | Буквальний job (порівняння будь-яких двох версій ОДНІЄЇ сторінки, з diff-підсвічуванням) повністю нативний, включно з довільними (не лише суміжними) версіями. Крос-сторінкове порівняння — окремий, неперевірений job без клієнтського доказу попиту. |

**Усі 3 кандидати Phase F не пережили Native Capability Kill Test.** Жоден не був врятований штучним звуженням: у кожному випадку зафіксовано, що можлива вужча альтернатива (regulated-industry DoD templates; reopen-analytics; cross-page diff) є ОКРЕМИМ job-to-be-done без підтвердженого клієнтського попиту, а не прихованою версією дослідженого кандидата.

**Explicitly not done in this phase:** жодного MVP, жодної архітектури, жодного числового скорингу, жодного pain/switching дослідження для будь-якого з 3 кандидатів (за прямою інструкцією — Phase G зупиняється на native+marketplace kill test).

## D. Candidate record

Copy this block for each candidate query/wedge.

### Candidate: [NAME]

**Marketplace:**  
**Target query:**  
**Customer/job-to-be-done:**  

**Top existing solutions:**  

**Observed pain:**  

**Switching evidence:**  

**New entrant evidence:**  

**Potential wedge:**  

**Expected support burden:**  

**Native replacement risk:**  

**Policy/API risk:**  

**Dependency risk:**  

**Monetization:**  

**Evidence URLs:**

- 
- 
- 

**Confidence:** LOW / MEDIUM / HIGH

## E. Research conclusion

Do not produce a score unless all veto gates pass.

Final research outcome must feed `DECISION.md`.
