---
name: Create and track an incident
description: Open an incident in Atomicwork, read it back, update it, and add a work note.
api: openapi/atomicwork-public-api-openapi.yaml
operations:
  - postapi-v-1-requests
  - getapi-v-1-requests-request-id
  - patchapi-v-1-requests-request-id
  - postapi-v-1-requests-request-id-notes
---

# Create and track an incident

Use the Atomicwork Public API to open and manage an IT incident.

## Auth & setup
- Send `X-Api-Key: <workspace-scoped key>` on every request (Settings > Integrations > API Keys).
- Send `X-Workspace-Id: <numeric workspace id>` — most endpoints are workspace-scoped.
- Base URL: `https://{tenant}.atomicwork.com/api/v1`.

## Steps
1. **Create the request** — `POST /api/v1/requests` (`postapi-v-1-requests`). Set the request kind to incident and supply subject/description and any required form fields. Discover required fields with the forms endpoints first if unsure.
2. **Read it back** — `GET /api/v1/requests/{requestId}` (`getapi-v-1-requests-request-id`) using the id returned in step 1.
3. **Update as work progresses** — `PATCH /api/v1/requests/{requestId}` (`patchapi-v-1-requests-request-id`) to change status, priority, or assignee.
4. **Add a work note** — `POST /api/v1/requests/{requestId}/notes` (`postapi-v-1-requests-request-id-notes`).

## Conventions & errors
- List endpoints paginate with `page`/`per_page` (max 100) or a `next_page_token` cursor.
- Errors return `{ "error": "...", "code": "..." }`. On `429`, back off using the `Retry-After` header.
- No idempotency-key header is supported — guard against duplicate creates on retry yourself.
