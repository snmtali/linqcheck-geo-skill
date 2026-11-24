# Checklist v0.1.1
Apply checks individually. Read guardrails.md for scope, aggregation and evidence rules. If the required source or tool is unavailable, return UNKNOWN / NOT VERIFIED. For absence claims, define the inspected scope. Do not treat optional fields as mandatory universally.

| ID | Check / criterion | Evidence required |
|---|---|---|
| A01 | Public page responds successfully; record redirects and status | Actual HTTP response |
| A02 | Applicable robots.txt rules permit intended crawler and path, where desired by owner | robots.txt and current official crawler documentation; distinguish search and training bots |
| A03 | Index directives consistent with intended public discovery | Raw meta robots and HTTP X-Robots-Tag where available |
| A04 | Canonical points to intended equivalent URL | Raw/rendered canonical and target context |
| A05 | Product URL listed in relevant sitemap if sitemap discovery is intended | Relevant sitemap fetched and inspected; partial sample cannot prove omission |
| A06 | Core product content accessible in raw and/or rendered page; report separately | Actual raw HTML and rendered snapshot; no simulated rendering |
| S01 | Product markup present and parseable where appropriate | Actual structured data; inspect JSON-LD, Microdata and RDFa separately from platform data |
| S02 | Offer describes applicable price and currency when publicly offered | Markup plus visible same-variant offer |
| S03 | Availability consistent across visible page and structured offer | Same variant and market snapshot |
| S04 | Breadcrumb markup matches navigation when present | Visible navigation and markup; optional enhancement |
| P01 | Product identity clear (name, brand when applicable) | Visible product content and markup |
| P02 | Identifiers (GTIN, SKU, MPN) valid and consistent when applicable and supplied | Actual identifiers; validate GTIN checksum if present; do not invent identifiers |
| P03 | Variant identity and offers distinguishable | Actual variant data; distinguish selectable, in-stock and preorder |
| P04 | Price and currency consistent across inspected representations | Same variant, locale and timestamp |
| C01 | Description provides meaningful product-specific information | Visible description |
| C02 | Category-relevant attributes available for comparison | Observed attributes; state relevant category and missing evidence |
| C03 | Product image references and alt text inspected | Actual HTML/rendered evidence; distinguish missing alt from decorative image |
| T01 | Seller identity and contact route discoverable | Public seller/contact pages |
| T02 | Delivery and returns information discoverable when applicable | Public policy pages; no legal compliance certification |
| L01 | Document language matches actual content | HTML lang and visible text |
| L02 | Alternate-language hreflang and market currencies consistent if applicable | Actual annotations and target pages; report sample coverage |

Readiness conclusions are hypotheses unless tested directly. Do not invent current AI engine recommendations, live search rankings or merchant eligibility. No changes, purchases or external submissions.
