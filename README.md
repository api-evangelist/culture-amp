# Culture Amp (culture-amp)

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
