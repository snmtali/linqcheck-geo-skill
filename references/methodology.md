# Evidence methodology / Kanıt metodolojisi

Evidence class is independent of check status.

| Class | Meaning | Example |
|---|---|---|
| MEASURED / Ölçüldü | Direct reproducible technical test with method and result | GET returned HTTP 200 at recorded time |
| OBSERVED / Kaynakta görüldü | Direct content or markup observation in retrieved material | JSON-LD contains an Offer price |
| INFERRED / Çıkarım | Interpretation or hypothesis grounded in explicit evidence | Missing attributes may make comparisons harder |
| NOT VERIFIED / Doğrulanamadı | Insufficient evidence or unavailable capability | Raw HTML unavailable |

PASS means the stated check meets its criterion; FAIL means evidence establishes nonconformance; UNKNOWN means insufficient evidence; N/A means irrelevant to page type with reason. An inference alone must not establish a technical failure. Separate observed facts from inferred effects. Record exact URL, timestamp, retrieval mode and short evidence excerpt or measurement. Avoid retaining personal data. For conflicts, record both sources and context; never guess the correct value. A single fetch does not establish persistent availability.

Priority: P1 confirmed material access or commerce-data issue; P2 confirmed content/structure issue or important unknown requiring verification; P3 optional enhancement. Adjust with explicit reasoning. No overall GEO score; report coverage and counts only.

References for semantics (consult current official documentation when necessary):
- https://schema.org/Product
- https://schema.org/Offer
- https://www.rfc-editor.org/rfc/rfc9309
- https://developers.google.com/search/docs/appearance/structured-data/product
- https://developers.google.com/search/docs/crawling-indexing/robots/intro
- https://platform.openai.com/docs/bots
- https://agentskills.io/specification

Crawler rules and engine policies evolve. A robots rule is not proof of indexing, actual crawling or recommendation. llms.txt is optional and must not be scored as a required ranking signal.
