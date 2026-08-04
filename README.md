# Culture Amp (culture-amp)

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

Culture Amp is the leading employee experience platform providing tools for employee engagement surveys, performance management, and people analytics. The Culture Amp Public API is a RESTful, read-only interface that enables organizations to programmatically retrieve their people data—including employee records, demographics, performance cycles, manager reviews, and survey results—for integration with external systems and custom analytics workflows. The API uses OAuth 2.0 Client Credentials Flow for authentication and is available to all subscribers at no additional cost as part of standard subscription fees.

APIs.json: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/apis.yml

Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=culture-amp-api-evangelist&utm_content=repo

## Tags

- HR
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Human Resources

## APIs

### Culture Amp Public API

The Culture Amp Public API provides read-only programmatic access to employee data, performance cycles, manager reviews, and survey data. It follows OAuth 2.0 Client Credentials Flow and returns paginated JSON responses.

- **Human URL:** https://www.cultureamp.com/company/api
- **Base URL:** https://api.cultureamp.com
- **OpenAPI Spec:** https://api.cultureamp.com/spec
- **Documentation:** https://docs.api.cultureamp.com/docs/resources-getting-started

**Endpoints include:**

- `GET /employees` — List all employees
- `GET /employees/{id}` — Retrieve specific employee details
- `GET /employees/{id}/demographics` — Get employee demographic assignments
- `GET /employees/{id}/manager-reviews` — Access manager reviews for an employee
- `GET /performance-cycles` — List performance cycles
- `GET /performance-cycles/{id}` — Retrieve specific cycle details
- `GET /performance-cycles/{id}/manager-reviews` — Manager reviews by cycle
- `GET /manager-reviews` — List all manager reviews
- `GET /manager-reviews/{id}` — Get individual review details

## Plans / Rate Limits / FinOps

### Plans

Culture Amp offers four main product modules priced on a per-employee-per-month basis with annual subscriptions. All pricing is quote-based.

| Plan | Type | Price Range |
|------|------|-------------|
| Engage | Paid | ~$9–$14 PEPM |
| Perform | Paid | Quote-based |
| Develop | Paid | Quote-based |
| People Analytics | Enterprise | ~$118–$122 PEPM |

API access is included in all plans at no additional charge.

Full details: [plans/culture-amp-plans-pricing.yml](plans/culture-amp-plans-pricing.yml)

### Rate Limits

Culture Amp applies client-based and service-based throttling. Specific numeric limits are not publicly disclosed. The platform returns HTTP 429 (Too Many Requests) and 503 (Service Unavailable) when throttled. Response payloads are limited to ~1 MB per request with automatic pagination.

Full details: [rate-limits/culture-amp-rate-limits.yml](rate-limits/culture-amp-rate-limits.yml)

### FinOps

Culture Amp follows a per-employee-per-month subscription model billed annually. API usage does not incur additional cost. Primary cost drivers are employee headcount and module selection.

Full details: [finops/culture-amp-finops.yml](finops/culture-amp-finops.yml)

## Timestamps

- **Created:** 2026-06-12
- **Modified:** 2026-06-12

## Common Properties

| Type | URL |
|------|-----|
| Website | https://www.cultureamp.com |
| Documentation | https://docs.api.cultureamp.com |
| GitHub Organization | https://github.com/cultureamp |
| LinkedIn | https://www.linkedin.com/company/cultureamp |
| X (Twitter) | https://x.com/CultureAmp |
| Blog | https://www.cultureamp.com/blog |
| Pricing | https://www.cultureamp.com/platform/pricing |
| Status Page | https://status.cultureamp.com |

## Maintainers

- **Kin Lane** — kin@apievangelist.com
