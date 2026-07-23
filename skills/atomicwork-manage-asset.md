---
name: Create and update an asset
description: Create an IT asset in Atomicwork, read it, update it, and review its activity history.
api: openapi/atomicwork-public-api-openapi.yaml
operations:
  - postapi-v-1-assets
  - getapi-v-1-assets-asset-id
  - putapi-v-1-assets-asset-id
  - getapi-v-1-assets-asset-id-activities
---

# Create and update an asset

Manage IT asset records in the Atomicwork CMDB.

## Auth & setup
- `X-Api-Key` and `X-Workspace-Id` headers.
- Base URL: `https://{tenant}.atomicwork.com/api/v1`.

## Steps
1. **(Optional) Inspect the schema** — `GET /api/v1/assets/types/{asset_type_id}/form-fields` to learn required fields, and `GET /api/v1/assets/attributes` for filterable attributes.
2. **Create the asset** — `POST /api/v1/assets` (`postapi-v-1-assets`) with the asset type and its fields.
3. **Read it back** — `GET /api/v1/assets/{asset_id}` (`getapi-v-1-assets-asset-id`).
4. **Update it** — `PUT /api/v1/assets/{asset_id}` (`putapi-v-1-assets-asset-id`).
5. **Review history** — `GET /api/v1/assets/{asset_id}/activities` (`getapi-v-1-assets-asset-id-activities`).

## Conventions & errors
- Asset listing uses `POST /api/v1/assets/list` with the structured filter body (`attribute`/`operator`/`values`).
- Errors return `{ "error": "...", "code": "..." }`; honor `Retry-After` on `429`.
- No idempotency-key header — avoid duplicate creates on retry.
