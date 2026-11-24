# Illustrative report — synthetic data, not a live audit
Scope: https://example.com/product (fictional fixture); supplied raw HTML only.
Fixture: visible price TRY 499; JSON-LD Offer price 599, priceCurrency TRY; same variant assumed by fixture. HTTP headers not supplied.

| ID | Status | Evidence | Finding | Priority | Action / retest |
|---|---|---|---|---|---|
| P04 | FAIL | OBSERVED | Visible 499 TRY vs markup 599 TRY | P1 | Verify authoritative price; align both representations; compare again |
| A01 | UNKNOWN | NOT VERIFIED | No HTTP response supplied | P2 | Retrieve public URL and record status |

Coverage for these two illustrative checks: 0 pass, 1 fail, 1 unknown. This is not a full audit. Possible comparison impact is INFERRED, not measured. No claims about actual AI visibility.
