# LinqCheck GEO Skill

**Evidence-based GEO and AI commerce readiness audits for public e-commerce pages.**

[ Türkçe README ](README.tr.md) · [Methodology](references/methodology.md) · [Checklist](references/checklist.md) · [Example](examples/sample-audit.md) · [Tests](TESTS.md)

Version **0.1.1 — experimental public beta**. Maintained by TalyNext.

## What it does

- Audits public product pages and adapts checks for other commerce page types.
- Separates measurements, observations, inferences and unverified claims.
- Examines product identity, variants, prices, stock, structured data, discovery and category-specific information where evidence permits.
- Produces prioritized findings with evidence and retest criteria, in English or Turkish.

No overall GEO score, ranking promises, automatic site edits or purchases. The skill is a set of agent instructions, not a crawler or standalone application. Results depend on the host model, available tools and source access.

## Install and use
[![Download GEO Skill](https://img.shields.io/badge/Download-GEO%20Skill%20v0.1.1-00897B?style=for-the-badge)](https://github.com/snmtali/linqcheck-geo-skill/releases/download/v0.1.1/linqcheck-geo-skill-v0.1.1-community.zip)

**Free for personal and internal business use.**

[View release notes](https://github.com/snmtali/linqcheck-geo-skill/releases/tag/v0.1.1)


Download or clone this repository into a folder named `linqcheck-geo-skill`. Install that folder using your compatible Agent Skills client's workflow. For Claude Code, use `.claude/skills/linqcheck-geo-skill/` inside a project or `~/.claude/skills/linqcheck-geo-skill/` for personal use. Other clients may accept a ZIP of the skill folder; consult their installation instructions. Web access is supplied by the host, not this skill.

Example prompt:

> Use LinqCheck GEO Skill to audit https://example.com/product for GEO and AI commerce readiness. Include evidence, coverage, limitations and prioritized actions. Read-only.

## Validation status

The previous version underwent 13 exploratory test activities, including Turkish and English reports, several commerce platforms, inaccessible URLs, a limited skill-on/off comparison and commercial-product comparison. Not all acceptance criteria passed. Three v0.1.1 agent smoke scenarios (Dagi, Seda Yalçın Atelier, Allbirds) were reviewed on 24 November 2026 and accepted for experimental beta with caveats. Full regression and independent reproduction remain pending; no claim of independently verified accuracy or superiority is made. See [TESTS.md](TESTS.md).

## Commercial disclosure

TalyNext also develops [LinqCheck](https://linqcheck.com), an optional commercial product. This source-available skill does not require an account, payment or mandatory LinqCheck service call. Host tools have their own data-handling policies. The skill contains no telemetry code.

## Contributing and license

Report reproducible issues with sanitized evidence, tool capabilities and skill version; omit personal data and credentials. See [LICENSE](LICENSE) (LinqCheck Community License — Version 1.0). Personal, educational, research and internal business use are permitted free of charge; business-related third-party audits and consulting (including free promotional audits), external commercial integrations, resale and public redistribution require separate written permission, subject to the license, GitHub Terms of Service and applicable law. Commercial enquiries: [LinqCheck](https://linqcheck.com). This is not an OSI-approved open-source project.
