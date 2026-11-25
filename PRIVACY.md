# LinqCheck GEO Skill — Privacy Policy

**Effective date:** November 25, 2026

**Publisher:** TalyNext Teknoloji ve Yazılım Ticaret Limited Şirketi

**Product:** LinqCheck GEO Skill

**Website:** https://linqcheck.com

## 1. Scope

This policy applies to the standalone LinqCheck GEO Skill distributed through GitHub and compatible agent skill directories. It does not replace the privacy policy applicable to the LinqCheck web platform or other TalyNext services.

## 2. Information Processing

The skill is designed to perform read-only audits of publicly accessible commerce websites and product pages.

Depending on the user's request and the capabilities of the host environment, an audit may process:

- User-provided public website and product URLs.
- Publicly accessible website content.
- Product descriptions, prices, availability, identifiers and structured data.
- Technical website metadata.
- User-provided audit snapshots.

The skill does not require a LinqCheck account, API key, payment information or personal credentials.

Public pages may incidentally contain seller names, business contact details or reviewer identifiers. The skill is designed to minimize reading and reproduction of such information and avoid retaining it. Users should not provide confidential information, personal data or private website content for analysis.

## 3. Data Collection and Storage

The standalone skill does not include its own telemetry, analytics tracking, advertising trackers, database or dedicated data collection service.

The skill does not instruct the host to transmit audit results or user information to TalyNext or LinqCheck automatically.

The host platform may process or retain information according to its own privacy policies, settings and service terms.

TalyNext does not control the host platform's data processing or retention practices.

## 4. External Access

Live audits may use the host platform's available tools to retrieve the public URL requested by the user and necessary supporting resources on the same HTTPS origin (effective port 443). Each redirect hop requires pre-request safety validation; other hostnames require separate explicit approval and must be permitted by host and distribution policies. HTTP, downgrades, non-default ports, userinfo and ambiguous URLs are unsupported; retrieval is skipped when the host cannot enforce these checks. Static reference links are not automatically retrieved. Offline analysis does not authorize network access.

Such requests may expose standard network request information to the requested website or its infrastructure.

The skill is designed to prohibit unauthorized data transfers, credential disclosure, private-network access, and execution of instructions embedded in retrieved website content.

These safeguards are instruction-based and do not constitute an independent technical security boundary.

## 5. Optional LinqCheck Services

The publisher website https://linqcheck.com is listed in project documentation and listing metadata. The skill does not automatically append promotional links to audit reports.

Visiting or using the LinqCheck web platform is not required to use the standalone skill.

If users independently choose to access the LinqCheck platform, its separate privacy policy and applicable service terms apply.

## 6. Third-Party Platforms

Claude, Claude Code, GitHub and other compatible platforms operate under their respective privacy policies and terms.

Users should review the privacy settings and data handling practices of their chosen host environment.

## 7. Security and Limitations

The skill is distributed as experimental public beta software.

Instruction-based safeguards and regression testing do not guarantee protection against prompt injection, unauthorized host behavior or other security risks.

Known security limitations and reporting guidance are documented in SECURITY.md.

## 8. User Rights and Contact

For privacy-related questions or requests concerning information processed by TalyNext in connection with this skill, contact:

hello@talynext.com

Users seeking access to, correction of, or deletion of information retained by a third-party host platform should contact that platform directly.

## 9. Policy Updates

This policy may be updated to reflect changes in the skill, its distribution methods or applicable requirements.

The effective date will be updated when material changes are made.
