# Fudan University (fudan)

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
