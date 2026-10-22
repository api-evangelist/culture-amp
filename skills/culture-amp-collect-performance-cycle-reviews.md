---
name: culture-amp-collect-performance-cycle-reviews
description: List Culture Amp performance cycles, pick one, and collect every manager review in it, or every review for one employee.
api: Culture Amp Public Performance API
operations:
  - list-performance-cycles
  - get-performance-cycle
  - list-manager-reviews-by-performance-cycle
  - get-manager-review
  - list-manager-reviews-by-employee
generated: 2026-10-20
method: generated
source: openapi/culture-amp-performance-api-openapi.yml
---
# Collect performance cycle reviews

1. Get a token scoped to `performance-evaluations-read`.
2. `list-performance-cycles` (GET /performance-cycles). You can filter by `state` and by the after-date parameter.
3. `get-performance-cycle` (GET /performance-cycles/{id}) for the cycle you chose.
4. `list-manager-reviews-by-performance-cycle` (GET /performance-cycles/{id}/manager-reviews). Page with `cursor` until no `pagination` object comes back.
5. `get-manager-review` (GET /manager-reviews/{id}) for full detail. For one person, use `list-manager-reviews-by-employee` (GET /employees/{id}/manager-reviews).

Rules: these are read-only GETs and safe to retry. Back off on 429/503.
