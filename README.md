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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Fudan University is a major public research university in Shanghai, China, ranked #84 in the QS World University Rankings 2025. This repository catalogs Fudan's public developer and API footprint as an [APIs.json](https://apisjson.org) profile. At the time of review, Fudan exposes no openly documented, publicly reachable developer API program; its primary machine-readable asset is a Dataverse research-data repository whose API is geo-restricted to mainland China.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=fudan-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research Data
- Open Data
- China
- Shanghai

## APIs

- **Fudan University Dataverse (Research Data Repository)** — Research data repository built on the Dataverse open-source platform (social science, demography, economics datasets). Dataverse software ships a native REST/Search API and OAI-PMH by design, but the host returns an access-forbidden page from outside mainland China, so the API is gated and undocumented for public use. Docs/portal: https://dvn.fudan.edu.cn

## Plans, Rate Limits, and FinOps

- Plans & Pricing: [plans/fudan-plans-pricing.yml](plans/fudan-plans-pricing.yml)
- Rate Limits: [rate-limits/fudan-rate-limits.yml](rate-limits/fudan-rate-limits.yml)
- FinOps: [finops/fudan-finops.yml](finops/fudan-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.fudan.edu.cn
- Website (English): https://www.fudan.edu.cn/en/
- GitHub: https://github.com/FudanUniversity (org exists, no public repos)
- LinkedIn: https://www.linkedin.com/school/fudan-university/
- Review: [review.yml](review.yml)

## Notes

- Verification caveat: `dvn.fudan.edu.cn` returns HTTP 200 but serves an access-forbidden ("禁止访问") page to requests originating outside mainland China. The standard Dataverse REST API (`/api/info/version`) and OAI-PMH (`/oai?verb=Identify`) endpoints could not be verified live and are effectively geo-restricted.
- The Dataverse endpoint paths referenced reflect standard Dataverse conventions, not Fudan-published documentation. No endpoints, credentials, or specifications were fabricated.
- The official GitHub organization exists but exposes no public repositories. LinkedIn returns 999 (anti-bot), which indicates the page exists rather than its absence.

## Maintainers

- Kin Lane — kin@apievangelist.com
