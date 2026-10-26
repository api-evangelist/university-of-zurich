# University of Zurich (university-of-zurich)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The University of Zurich (UZH) is Switzerland's largest university, founded in 1833, and is ranked #61 in the QS World University Rankings 2025. This repository catalogs UZH's public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile. UZH has no centralized public developer portal; its machine-readable surface centers on open scholarship (the ZORA research repository), open-source code (the `uzh` GitHub organization), and federated identity (SWITCH edu-ID).

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-zurich-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Public Research University, Switzerland, Europe, League of European Research Universities, Open Access, Research Repository, OAI-PMH, Identity Federation, GraphQL, Research Computing

## APIs

Every surface below carries an operator: `institution` means UZH runs the thing, `tenant` means UZH's data and users on someone else's platform. UZH authors no API contract of its own — each institution-operated endpoint below speaks a contract written by DSpace, GitLab or the OAI-PMH community.

- **ZORA Repository OAI-PMH** (`institution`) — OAI-PMH 2.0 metadata harvesting for the Zurich Open Repository and Archive. Live base URL `https://www.zora.uzh.ch/server/oai/request`; disseminates mods, oai_dc, oai_datacite, marc, akaber. Docs: https://www.zora.uzh.ch/
- **ZORA DSpace REST API** (`institution`) — DSpace 8.0 REST API (HAL+JSON) at `https://www.zora.uzh.ch/server/api`; communities and collections read open, items 401. Docs: https://www.zora.uzh.ch/
- **KlickerUZH GraphQL API** (`institution`) — The UZH Department of Banking and Finance's open-source audience-response platform, at `https://api.klicker.uzh.ch/graphql`. Live and validating; introspection disabled in production. Docs: https://www.klicker.uzh.ch/development/
- **UZH GitLab REST API** (`institution`) — Self-hosted GitLab at `https://gitlab.uzh.ch/api/v4`; anonymous read of public project metadata. Docs: https://gitlab.uzh.ch/
- **University of Zurich Identity Provider (SWITCH edu-ID)** (`tenant`) — The entity `https://aai-idp.uzh.ch/idp/shibboleth` is UZH's namespace, but its SAML SSO endpoints run on SWITCH's hosted edu-ID platform at `uzh.login.eduid.ch`. Machine-readable in the SWITCHaai federation aggregate: https://metadata.aai.switch.ch/metadata.switchaai.xml

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-zurich-plans-pricing.yml](plans/university-of-zurich-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-zurich-rate-limits.yml](rate-limits/university-of-zurich-rate-limits.yml)
- FinOps: [finops/university-of-zurich-finops.yml](finops/university-of-zurich-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.uzh.ch/en.html
- Privacy: https://www.uzh.ch/en/privacy.html
- Legal notice: https://www.uzh.ch/en/impressum.html
- Blog: https://www.news.uzh.ch/en.html
- Support: https://www.zi.uzh.ch/en/support.html
- Research repository: https://www.zora.uzh.ch/
- Identity federation: https://metadata.aai.switch.ch/metadata.switchaai.xml
- Course catalogue: https://courses.uzh.ch/
- Research computing: https://www.zi.uzh.ch/en/teaching-and-research/science-it/computing/sciencecluster.html
- AI policy: https://www.uzh.ch/en/explore/basics/ai/recommendations.html
- Conformance: [conformance/university-of-zurich-conformance.yml](conformance/university-of-zurich-conformance.yml)
- GitHub: https://github.com/uzh
- LinkedIn: https://www.linkedin.com/school/uzh
- Twitter/X: https://x.com/UZH_en
- Authentication: https://www.zi.uzh.ch/en/support/identity-access/eduid-faq.html

## Notes

Re-profiled 2026-08-30 under the university pipeline's operator axis.

**What was removed.** This repository previously held three OpenAPI documents — `discovery-api`, `oauth2-api` and `openid-connect-api` — plus collections, examples, JSON Schema, JSON Structure, rules, vocabulary, JSON-LD, agentic-access, authentication and capability artifacts derived from them. All of it described `https://login.eduid.ch`, and said so itself: `info.title` began "SWITCH edu-ID", `info.contact.name` was "SWITCH edu-ID", and `servers[]` was `https://login.eduid.ch`. That is SWITCH's shared national identity issuer, used by every Swiss institution — the EPFL profile in this catalog points at the same host. Twenty-six files were removed so UZH is not credited for SWITCH's engineering. The relationship itself was kept and re-labelled `x-operator: tenant`.

**What was repaired.** The June 2026 profile recorded the ZORA OAI-PMH base URL as `https://www.zora.uzh.ch/oai/request` and noted it could not be confirmed. It returns 404. The live DSpace 8.0 base URL is `https://www.zora.uzh.ch/server/oai/request`, confirmed by an Identify response naming `repositoryName ZORA` and `adminEmail martin.braendle@uzh.ch`.

**What was found.** Two institution-operated surfaces the June profile missed: the KlickerUZH GraphQL API and the self-hosted GitLab v4 REST API. Domain-standard conformance was probed against the Kin Score `education` regime and evidenced for `oai-pmh`, `datacite`, `orcid`, `shibboleth` and `saml`; `scim`, `lti`, `oneroster`, `ed-fi`, `caliper` and `qti` were not found.

**What is absent.** No developer portal, no OpenAPI, no API keys, no published rate limits, no status page, no `llms.txt` (404), no `.well-known/security.txt` (404). `api.uzh.ch`, `data.uzh.ch`, `opendata.uzh.ch` and `developer.uzh.ch` do not resolve. The course catalogue, the OLAT learning platform and swisscovery library discovery are web/SSO surfaces with no documented public API. `www.zora.uzh.ch` serves an Anubis bot challenge on some paths. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
