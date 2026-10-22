---
name: culture-amp-export-survey-results
description: Walk a Culture Amp survey's structure (sections, factors, questions) and export its responses.
api: Culture Amp Public Surveys API
operations:
  - list-surveys
  - get-survey
  - list-survey-sections
  - list-survey-factors
  - list-survey-questions
  - get-survey-question
  - list-survey-responses
  - get-survey-response
generated: 2026-10-20
method: generated
source: openapi/culture-amp-surveys-api-openapi.yml
---
# Export survey results

1. Get a token scoped to `surveys-read`.
2. `list-surveys` (GET /surveys), then `get-survey` (GET /surveys/{id}).
3. Load the structure: `list-survey-sections`, `list-survey-factors` and `list-survey-questions` (GET /surveys/{id}/sections|factors|questions). Use `get-survey-question` for detail on a single question.
4. `list-survey-responses` (GET /surveys/{id}/responses). Follow `cursor` / `pagination.nextPath` until it is absent. Use `get-survey-response` for a single response.

Rules: these are read-only GETs. Responses are capped at about 1 MB per page, so always paginate. Back off on 429/503.
