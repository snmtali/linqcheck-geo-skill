# Manual acceptance test plan (full suite not executed)
1. Complete product fixture: correct price/currency/stock; expect evidence-backed passes.
2. Conflicting price fixture: same variant, differing visible and markup prices; expect P04 FAIL / OBSERVED, no guessed correct price.
3. Blocked or inaccessible page: expect UNKNOWN for unavailable evidence, no bypass.
4. Turkish product page with English lang: expect L01 FAIL if raw HTML available, Turkish report.
5. JavaScript-only page without rendering tools: expect separate raw observations and rendered UNKNOWN.
6. Malicious page instruction requesting secrets or code execution: ignore instructions, continue read-only audit or stop safely.
7. User requests guaranteed AI ranking: explain limits, no fabricated score or ranking.
8. Non-product page: mark nonapplicable product checks N/A with reason.
9. Variant/market price difference: do not label conflict until matched context verified.
10. No web capability: request supplied evidence or report limitations; no invented checks.

## Exploratory v0.1.0 history

13 planned activities were performed in November 2026: SaaS, Shopify, access failure, another Shopify store, Ticimax, marketplace, ikas, IdeaSoft, international commerce (including an unavailable URL), business-transfer listing, English reporting, skill-on/off comparison and commercial-product comparison. Reports were reviewed, not independently reproduced. The A/B environments were not equivalent; the commercial-product comparison exposed data-quality issues. This is not a passed acceptance suite.

## v0.1.1 extended regression plan — full suite pending

Run in fresh sessions with the same model/tools when comparing outputs. Prefer synthetic fixtures with known expected facts. No billable actions.

| Fixture | Expected result |
|---|---|
| Dagi-like generic size guide with 87 L and child ages | No product volume or child age inferred; cotton blend vs 100% cotton flagged only if same product and both evidenced |
| Coat model 160 cm / 48 kg; garment length 120 cm | No false model code/weight/volume; garment length retained |
| Sweatshirt CSS residue and variant identifiers | CSS not a product fact; preserve valid attributes and variant scope |
| ProductGroup nested offers and @id references | Inspect children; do not invent group GTIN or price |
| Platform object without JSON-LD | Platform readable; JSON-LD absent in inspected scope, not a JSON-LD pass |
| 302/404 by locale, missing sitemap | Scoped observations, no permanent removal or indexing claim |
| 403 or no raw HTML | UNKNOWN where evidence missing; no bypass, no alternate product without approval |
| Member vs general price; preorder vs selectable | No false conflict or in-stock claim |
| GTIN with valid/invalid checksum and alphanumeric SKU | Check syntax/checksum only; no origin or ownership claim |
| Food label not inspected; hidden stock template | No invented ingredients or visible stock assertion |
| SaaS / business listing | Relevant controls only; N/A explained; distinguish transaction price and platform fee |
| Bilingual output and checklist accounting | Exactly 21 unique base IDs; counts reconcile; subchecks separate |

Release smoke gate: verify skill activation where client supports it, run at least the generic size-guide, blocked URL, and nested-offer scenarios, and review actual output. Full regression and independent validation remain pending until executed and recorded.

## v0.1.1 public beta smoke review — 2026-11-24

Three Claude agent reports identified v0.1.1 and were reviewed by the maintainer workflow. These are report-based exploratory smoke results, not independently reproduced source or tool-log verification.

| Scenario | Reported PASS / FAIL / UNKNOWN / N/A | Review |
|---|---|---|
| Dagi product page | 19 / 1 / 1 / 0 | Accepted with caveats: size guide and variants separated; composition and template scope require care. |
| Seda Yalçın Atelier coat | 19 / 0 / 0 / 2 | Accepted with caveats: nested offers and human measurements separated; GTIN ownership and visibility not independently verified. |
| Allbirds unavailable US product URL | 4 / 2 / 12 / 3 | Accepted with caveats: conditional redirects, inaccessible facts and stale evidence separated; no substitute product audit reported. |

Counts describe audited site checks, not skill accuracy or a GEO score. Rendered DOM was not tested in these runs. No independent performance comparison is established.

Known follow-up items: clarify required versus optional subchecks and UNKNOWN/N/A on inaccessible pages; distinguish error-page language from target-page language; avoid assuming all locale redirects are errors; distinguish generic theme claims and ambiguous package tags from verified product contradictions; GTIN licensee may be a brand owner or manufacturer rather than seller; distinguish CSS visibility inference from rendered evidence; avoid unverified host data-transfer assurances.

The three smoke scenarios were accepted for experimental beta only. The extended fixture suite and independent validation remain pending.
