---
name: culture-amp-look-up-an-employee
description: Find a Culture Amp employee by email or employee identifier, then fetch their record and demographics.
api: Culture Amp Public Employees API
operations:
  - list-employees
  - get-employee
  - list-demographics-by-employee
generated: 2026-10-20
method: generated
source: openapi/culture-amp-employees-api-openapi.yml
---
# Look up an employee

1. Get an access token with the OAuth2 client-credentials flow (tokenUrl `/oauth2/token`), requesting `employees-read` (and `employee-demographics-read` for step 4). See https://docs.api.cultureamp.com/docs/customer-guide-authentication.md.
2. `list-employees` (GET /employees). Filter with `email` or `employee_identifier`. If the response includes a `pagination` object, follow `pagination.nextPath` or pass its `cursor`.
3. `get-employee` (GET /employees/{id}) with the `id` you found.
4. `list-demographics-by-employee` (GET /employees/{id}/demographics).

Rules: every operation is a read-only GET, so retrying is safe. On 429/503 throttling, back off and retry (https://docs.api.cultureamp.com/docs/resources-usage-limits.md).
