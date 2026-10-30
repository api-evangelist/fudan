# Fudan University

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

Fudan University is a public research university in Shanghai, China, and a member of the national C9 League and Double First-Class programme. Its programmable footprint is small and almost entirely internal, but — unusually for this cohort — none of it is a vendor's contract wearing the university's name: every surface catalogued here runs on a host under fudan.edu.cn and is operated by Fudan itself. The real find is identity federation. Fudan operates a Shibboleth SAML 2.0 identity provider, registered with the CARSI federation and published to eduGAIN since February 2020, and it serves its own SAML metadata live at idpfudan.fudan.edu.cn. Alongside it, id.fudan.edu.cn publishes a working OpenID Connect discovery document and JWKS with no authentication required. Both are genuinely machine-readable and neither is documented anywhere Fudan publishes. Beyond identity, the Social Science Data Platform migrated off Dataverse to a custom application at rdr.fudan.edu.cn/datahome; its JSON backend answers, but it is undocumented, session-bound, and returns application-level refusals with HTTP 200. There is no developer portal, no public API key programme, no OAI-PMH, no open data portal, no robots.txt and no llms.txt on the main site, and the official GitHub organisation has zero public repositories — the university's public code lives instead in departmental lab organisations.

**Areas:** University · Higher Education · Education · China · Shanghai · C9 League · Identity Federation · Research Data · SSO

## Fudan University on APIs.io

Everything profiled for Fudan University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fudan/](https://apis.io/providers/fudan/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Fudan University Shibboleth Identity Provider (CARSI / eduGAIN)](https://apis.io/apis/fudan/identity-saml/) — Fudan's SAML 2.0 identity provider, entityID https://idpfudan.fudan.edu.cn/idp/shibboleth, asserting scope fudan.edu.cn. It is registered with CARSI,…
- [Fudan University Social Science Data Platform (复旦大学社会科学数据平台)](https://apis.io/apis/fudan/research-data-platform/) — Fudan's institutional research data repository, operated by the Research Center for Social Sciences. It moved off Dataverse: dvn.fudan.edu.cn now only…
- [Fudan University Authorization API](https://apis.io/apis/fudan/fudan-authorization-api/) — End-user authentication and token issuance.
- [Fudan University Discovery API](https://apis.io/apis/fudan/fudan-discovery-api/) — Machine-readable metadata about the provider.
- [Fudan University Identity API](https://apis.io/apis/fudan/fudan-identity-api/) — Claims about the authenticated end user.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (1)

The data models the API reads and writes.

- [Fudan University OpenID Connect discovery document](https://apis.io/schemas/fudan/fudan-openid-configuration/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Fudan Context](https://apis.io/jsonld/fudan/fudan-context/)

#### Examples (2)

Example requests and responses.

- [Fudan Idp Jwks](https://apis.io/examples/fudan/fudan-idp-jwks/)
- [Fudan Openid Configuration](https://apis.io/examples/fudan/fudan-openid-configuration/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Fudan Authentication](https://apis.io/security/fudan/fudan-authentication/)
- [Fudan Domain Security](https://apis.io/security/fudan/fudan-domain-security/)
- [Fudan Vulnerability Disclosure](https://apis.io/security/fudan/fudan-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Fudan Scopes](https://apis.io/scopes/fudan/fudan-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Fudan Plans Pricing](https://apis.io/plans/fudan/fudan-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Fudan Rate Limits](https://apis.io/rate-limits/fudan/fudan-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Fudan Finops](https://apis.io/finops/fudan/fudan-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.fudan.edu.cn)
- [Support](https://xxb.fudan.edu.cn/)
- [Blog](https://news.fudan.edu.cn/)
- [GitHub](https://github.com/FudanUniversity)

## API Evangelist rating

**Kin Score 19.8** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 57.1 |
| Contract quality | 25.6 |
| Contract governance | 3.8 |
| Operational transparency | 7.9 |
| Developer ergonomics | 19.0 |
| Access clarity | 5.3 |

**Agent readiness 18.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 32.4** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fudan/](https://apis.io/providers/fudan/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Fudan University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fudan/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
