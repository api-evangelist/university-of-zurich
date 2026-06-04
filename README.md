# University of Zurich (university-of-zurich)

The University of Zurich (UZH) is Switzerland's largest university, founded in 1833, and is ranked #61 in the QS World University Rankings 2025. This repository catalogs UZH's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile. UZH has no centralized public developer portal; its machine-readable surface centers on open scholarship (the ZORA research repository), open-source code (the `uzh` GitHub organization), and federated identity (SWITCH edu-ID).

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-zurich-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Switzerland, Open Access, Research Repository, Open Data, Identity

## APIs

- **ZORA Repository OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the Zurich Open Repository and Archive of UZH research output. Docs: https://www.zora.uzh.ch/
- **ZORA DSpace REST API** — Standard DSpace REST API (HAL+JSON) exposed after ZORA's October 2025 migration to DSpace. Docs: https://www.zora.uzh.ch/
- **SWITCH edu-ID / UZH Identity (SAML & OpenID Connect)** — Central federated identity for UZH services via SWITCHaai (Shibboleth/SAML) and OpenID Connect / OAuth 2.0. Docs: https://www.zi.uzh.ch/en/support/identity-access/eduid-faq.html

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-zurich-plans-pricing.yml](plans/university-of-zurich-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-zurich-rate-limits.yml](rate-limits/university-of-zurich-rate-limits.yml)
- FinOps: [finops/university-of-zurich-finops.yml](finops/university-of-zurich-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.uzh.ch/en.html
- GitHub: https://github.com/uzh
- LinkedIn: https://www.linkedin.com/school/uzh
- Twitter/X: https://x.com/UZH_en
- Authentication: https://www.zi.uzh.ch/en/support/identity-access/eduid-faq.html

## Notes

Verification caveats: The GitHub org `uzh` (65 public repos) was confirmed live via the GitHub API. The official website and edu-ID linking service resolve (HTTP 200). ZORA's existence and OAI-PMH support are confirmed via the EPrints registry, a CORE OAI sample record, and the UZH University Library blog announcing the October 2025 migration from EPrints to DSpace; the legacy EPrints OAI endpoint (`/cgi/oai2`) now returns HTTP 404. The new DSpace OAI (`/oai/request`) and REST (`/server/api`) endpoints are cataloged as the current paths but could not be confirmed live from the cataloging environment (the `www.zora.uzh.ch` host timed out). No endpoints were fabricated. Student-facing systems (Course Catalogue, OLAT LMS, student services) are SSO/web-gated and are not cataloged as open APIs.

## Maintainers

- Kin Lane — kin@apievangelist.com
