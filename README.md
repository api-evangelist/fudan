# Fudan University (fudan)

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

Fudan University is a public research university in Shanghai, China, and a member of the C9 League.
This repository catalogs Fudan's public developer and API footprint as an
[APIs.json](https://apisjson.org) profile. It was re-profiled on 2026-08-30 under the API Evangelist
university pipeline, which settles **who operates** each surface before anything is saved.

Fudan is a clean institution case. No vendor-operated surface and no vendor tenant was found: the
Figshare, Elsevier Pure, Canvas, WorldCat and Ex Libris tenant hostnames a university of this size
would normally carry all fail to resolve or return an empty or error response. Every surface
catalogued here runs on a host under `fudan.edu.cn` and is operated by Fudan itself.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=fudan-api-evangelist&utm_content=repo

## Type

- University / Public Research University / Index / Consumer / 3rd-Party

## Tags

- University
- Higher Education
- Education
- China
- Shanghai
- C9 League
- Identity Federation
- Research Data
- Single Sign-On

## Surfaces

All three are `x-operator: institution`.

- **Fudan University Unified Identity — OpenID Connect** (`id.fudan.edu.cn`). A live OpenID Connect
  discovery document and JWKS, both served without authentication. Issuer
  `https://id.fudan.edu.cn/idp`. The OpenAPI in this repository is **derived from Fudan's own
  discovery document**, not published by Fudan.
- **Fudan University Shibboleth Identity Provider** (`idpfudan.fudan.edu.cn`). SAML 2.0 metadata
  served by Fudan itself, entityID `https://idpfudan.fudan.edu.cn/idp/shibboleth`, scope
  `fudan.edu.cn`, registered with the CARSI federation and published to eduGAIN since 2020-02-12.
  This is the basis of the `shibboleth` and `saml` conformance recorded here.
- **Fudan University Social Science Data Platform** (`rdr.fudan.edu.cn/datahome`). The institutional
  research data repository. Its JSON backend is live but undocumented and session-bound, so **no
  contract is saved for it**.

## Artifacts

- OpenAPI: [openapi/fudan-identity-openapi.yml](openapi/fudan-identity-openapi.yml) (derived) with a
  pristine copy in [openapi/_original/](openapi/_original/)
- Conformance: [conformance/fudan-conformance.yml](conformance/fudan-conformance.yml)
- Authentication: [authentication/fudan-authentication.yml](authentication/fudan-authentication.yml)
- Scopes: [scopes/fudan-scopes.yml](scopes/fudan-scopes.yml)
- Errors: [errors/fudan-errors.yml](errors/fudan-errors.yml)
- Lifecycle: [lifecycle/fudan-lifecycle.yml](lifecycle/fudan-lifecycle.yml)
- Vocabulary: [vocabulary/fudan-vocabulary.yml](vocabulary/fudan-vocabulary.yml)
- JSON Schema: [json-schema/fudan-openid-configuration-schema.json](json-schema/fudan-openid-configuration-schema.json)
- Verbatim captures: [examples/](examples/) — the discovery document, the JWKS, and the SAML metadata
  exactly as returned on 2026-08-30
- Plans & Pricing: [plans/fudan-plans-pricing.yml](plans/fudan-plans-pricing.yml)
- Rate Limits: [rate-limits/fudan-rate-limits.yml](rate-limits/fudan-rate-limits.yml)
- FinOps: [finops/fudan-finops.yml](finops/fudan-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.fudan.edu.cn
- Website (English): https://www.fudan.edu.cn/en/
- Identity Federation (SAML): https://idpfudan.fudan.edu.cn/idp/shibboleth
- Identity Federation (OIDC): https://id.fudan.edu.cn/idp/.well-known/openid-configuration
- Research Repository: https://rdr.fudan.edu.cn/datahome/open/dataResource
- Library: https://library.fudan.edu.cn/
- Course Catalog / Registrar: https://jwc.fudan.edu.cn/
- AI Policy: https://news.fudan.edu.cn/2024/1220/c3163a143685/page.htm
- Support (IT Office): https://xxb.fudan.edu.cn/
- GitHub: https://github.com/FudanUniversity (org exists, zero public repositories)
- GitHub (labs): https://github.com/FudanNLP, https://github.com/FudanSELab
- LinkedIn: https://www.linkedin.com/school/fudan-university/
- Review: [review.yml](review.yml)

## Corrections made on 2026-08-30

- **`dvn.fudan.edu.cn` is not geo-blocked.** The earlier profile recorded an access-forbidden
  ("禁止访问") page. It now serves a 341-byte meta-refresh redirect to
  `https://rdr.fudan.edu.cn/datahome/`.
- **There is no Dataverse REST API and no OAI-PMH.** `/api/info/version` and `/oai?verb=Identify`
  return 404 on both the old and the new host. The earlier entry stated in its own text that its
  endpoint paths "reflect standard Dataverse conventions, not Fudan-published documentation"; that
  entry has been replaced.
- **The vulnerability disclosure claim is withdrawn.** The 2026-07-11 source URL cannot be verified
  and has no Wayback snapshot. The artifact is re-based on the live IT Office security section, which
  describes internal services only and offers no reporting channel.
- **`github.com/OpenMOSS` is not Fudan's.** It self-describes as a research group under the Shanghai
  Innovation Institution collaborating with Fudan, and is not credited to the institution.

## Notes

- The OpenID Connect discovery document declares its end-session endpoint under the member name
  `"end_session_endpoint "` — with a trailing space. A strict OpenID Connect Discovery client will
  not find it. Recorded as observed, not corrected.
- The research data platform answers unauthenticated calls with **HTTP 200** and an in-body refusal
  (`{"status":4000,"message":"状态锁不得为空"}`), so status-code-only monitoring reads a refusal as a
  success.
- `library.fudan.edu.cn/oai` returns HTTP 200 with a generic HTML page — a soft 404, not OAI-PMH.
- `www.fudan.edu.cn` publishes no `robots.txt`, no `llms.txt` and no `security.txt`.
- LinkedIn returns 999 (anti-bot), which indicates the page exists rather than its absence.

## Maintainers

- Kin Lane — kin@apievangelist.com
