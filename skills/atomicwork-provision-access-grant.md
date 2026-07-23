---
name: Provision an identity access grant (IGA)
description: Discover apps and entitlements, grant access to a user, and revoke it — Atomicwork identity governance.
api: openapi/atomicwork-public-api-openapi.yaml
operations:
  - getapi-v-1-iga-apps
  - getapi-v-1-iga-entitlements
  - postapi-v-1-iga-grants
  - postapi-v-1-iga-grants-grant-id-revoke
---

# Provision an identity access grant (IGA)

Directly provision access for a user through Atomicwork's identity governance (IGA) surface, bypassing the interactive approval workflow — for use by HRMS, onboarding, or compliance systems.

## Auth & setup
- `X-Api-Key` and `X-Workspace-Id` headers as in every Atomicwork call.
- Base URL: `https://{tenant}.atomicwork.com/api/v1`.

## Steps
1. **Discover apps** — `GET /api/v1/iga/apps` (`getapi-v-1-iga-apps`).
2. **Discover entitlements** — `GET /api/v1/iga/entitlements?app_id={id}` (`getapi-v-1-iga-entitlements`) to find valid `entitlement_id`s.
3. **Create the grant** — `POST /api/v1/iga/grants` (`postapi-v-1-iga-grants`) with required `user_id` and `entitlement_id`. Optional: `policy_id`/`policy_key`, `granted_by`, `granted_at`. The provisioning method (Okta, Azure AD, JumpCloud, Google Workspace, or manual) is derived from the entitlement config.
4. **Revoke when done** — `POST /api/v1/iga/grants/{grant_id}/revoke` (`postapi-v-1-iga-grants-grant-id-revoke`).

## Conventions & errors
- `403` means the API key lacks IGA permission; `404` a bad app/entitlement/grant id.
- No idempotency key — de-duplicate grant creation on your side.
- Audit trail is queryable via the audit-logs endpoints and per-grant history (`getapi-v-1-iga-grants-grant-id-history`).
