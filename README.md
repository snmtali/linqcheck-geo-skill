# LinqCheck GEO Skill

**Evidence-based GEO and AI commerce readiness audits for public e-commerce pages.**

[ Türkçe README ](README.tr.md) · [Methodology](references/methodology.md) · [Checklist](references/checklist.md) · [Example](examples/sample-audit.md) · [Tests](TESTS.md)

This source tree is **0.1.3 — experimental Public Beta**. The v0.1.3 download links become available when the maintainer publishes the release; until then use the previous v0.1.2 release. Maintained by TalyNext.

## What it does

- Audits public product pages and adapts checks for other commerce page types.
- Separates measurements, observations, inferences and unverified claims.
- Examines product identity, variants, prices, stock, structured data, discovery and category-specific information where evidence permits.
- Produces prioritized findings with evidence and retest criteria, in English or Turkish.

No overall GEO score, ranking promises, automatic site edits or purchases. The skill is a set of agent instructions, not a crawler or standalone application. Results depend on the host model, available tools and source access.

## Install and use
[![Download GEO Skill](https://img.shields.io/badge/Download-GEO%20Skill%20v0.1.3-00897B?style=for-the-badge)](https://github.com/snmtali/linqcheck-geo-skill/releases/download/v0.1.3/linqcheck-geo-skill-v0.1.3-community.zip)

**Free for personal and internal business use.**

[View release notes](https://github.com/snmtali/linqcheck-geo-skill/releases/tag/v0.1.3)


Download or clone this repository into a folder named `linqcheck-geo-skill`. Install that folder using your compatible Agent Skills client's workflow. For Claude Code, use `.claude/skills/linqcheck-geo-skill/` inside a project or `~/.claude/skills/linqcheck-geo-skill/` for personal use. Other clients may accept a ZIP of the skill folder; consult their installation instructions. Web access is supplied by the host, not this skill.

Example prompt:

> Use LinqCheck GEO Skill to audit https://example.com/product for GEO and AI commerce readiness. Include evidence, coverage, limitations and prioritized actions. Read-only.

Skills.sh installer (review source and installer permissions first):

```sh
npx skills add snmtali/linqcheck-geo-skill --skill linqcheck-geo-skill
```

This command follows the repository source, not a checksum-pinned release asset.

## Network access / External services

Live audits use host-provided tools to retrieve the explicitly requested public URL and necessary supporting resources on the same HTTPS origin (robots.txt, sitemap, relevant product, seller and policy pages). Only HTTPS with effective port 443 is supported. Each redirect hop must be safely validated before retrieval; other hostnames and subdomains require separate explicit approval and applicable host/distribution policy permission. HTTP, downgrades, non-default ports, userinfo and ambiguous URLs are not supported. If the host tool cannot enforce these checks, retrieval is skipped. Static bibliography links are not automatically fetched. Offline analysis makes no network requests. No automatic transfer to TalyNext/LinqCheck, telemetry or mandatory API call is required. Destination websites may receive ordinary network request information. See [Privacy](PRIVACY.md).

## Example use cases

- “Audit my public product URL read-only; compare price, availability and variant evidence.”
- “In a permitted offline environment, assess the supplied synthetic HTML evidence without network access.”
- “Produce a Turkish audit with all 21 checks and prioritized fixes; keep unverified checks UNKNOWN.”

## Validation status

Historical candidate results, limitations and unresolved W012 are documented in [TESTS.md](TESTS.md) and [SECURITY.md](SECURITY.md). Targeted rc.2 reports reviewed: 12 offline rule checks, a blocked retail attempt, conditional live SaaS and offline synthetic product tests. Actual network enforcement, final-version activation and independent security verification remain unverified. Directory policy 1.F/3.F remains unresolved; no catalog approval claimed.

## Commercial disclosure

TalyNext also develops [LinqCheck](https://linqcheck.com), an optional commercial product. This source-available skill does not require an account, payment or mandatory LinqCheck service call. Host tools have their own data-handling policies. The skill contains no telemetry code.

## Contributing and license

Report reproducible issues with sanitized evidence, tool capabilities and skill version; omit personal data and credentials. See [LICENSE](LICENSE) (LinqCheck Community License — Version 1.0). Personal, educational, research and internal business use are permitted free of charge; business-related third-party audits and consulting (including free promotional audits), external commercial integrations, resale and public redistribution require separate written permission, subject to the license, GitHub Terms of Service and applicable law. Commercial enquiries: [LinqCheck](https://linqcheck.com). This is not an OSI-approved open-source project.

## Installation integrity

Review the official repository and release before installing. Compare the downloaded v0.1.3 ZIP hash with its accompanying SHA-256 release asset before installation.

Windows PowerShell: `Get-FileHash -Algorithm SHA256 <downloaded-zip>`

macOS: `shasum -a 256 <downloaded-zip>`

Linux: `sha256sum <downloaded-zip>`

Replace the placeholder with the actual file path (quoted if needed). A matching checksum verifies integrity against that reference, not publisher identity or safety. See [SECURITY.md](SECURITY.md).
