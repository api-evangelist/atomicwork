# Atomicwork

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Atomicwork is an agentic service management (ITSM/ESM) platform that pairs an AI "coworker" (Atom) with a modern service desk for IT, HR, and other enterprise teams. The Atomicwork Public API gives programmatic, workspace-scoped access to the core platform — requests and tickets (incidents, service requests, problems, changes, major incidents), assets and a CMDB, users and workspaces, service catalog, automation workflows, custom objects, audit logs, and identity governance (IGA) grants and entitlements. Authentication is via a workspace-scoped API key (X-Api-Key) with an X-Workspace-Id scoping header. Atomicwork also ships an official hosted MCP server so AI clients (Claude, Cursor, Copilot, Codex) can drive the same operations as tools. The API is documented as OpenAPI 3.1 with 102 paths across 16 tags, offset and cursor pagination, and a structured filter model.

**Areas:** Company · Service Management · ITSM · ESM · IT Service Desk · Identity Governance · Asset Management · AI Agents · MCP · Enterprise

## Atomicwork on APIs.io

Everything profiled for Atomicwork is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/atomicwork/](https://apis.io/providers/atomicwork/)** — or go straight to one of the APIs or properties below.

### APIs (16)

- [Atomicwork Assets API](https://apis.io/apis/atomicwork/atomicwork-assets-api/) — The assets API from Atomicwork — 7 operation(s) for assets.
- [Atomicwork Business Hour Config API](https://apis.io/apis/atomicwork/atomicwork-businesshourconfig-api/) — The businessHourConfig API from Atomicwork — 2 operation(s) for businesshourconfig.
- [Atomicwork Entities API](https://apis.io/apis/atomicwork/atomicwork-entities-api/) — The entities API from Atomicwork — 1 operation(s) for entities.
- [Atomicwork Forms API](https://apis.io/apis/atomicwork/atomicwork-forms-api/) — The forms API from Atomicwork — 5 operation(s) for forms.
- [Atomicwork Problems API](https://apis.io/apis/atomicwork/atomicwork-problems-api/) — The problems API from Atomicwork — 4 operation(s) for problems.
- [Atomicwork Requests API](https://apis.io/apis/atomicwork/atomicwork-requests-api/) — The requests API from Atomicwork — 19 operation(s) for requests.
- [Atomicwork Tags API](https://apis.io/apis/atomicwork/atomicwork-tags-api/) — The tags API from Atomicwork — 2 operation(s) for tags.
- [Atomicwork Users API](https://apis.io/apis/atomicwork/atomicwork-users-api/) — The users API from Atomicwork — 10 operation(s) for users.
- [Atomicwork Workflows API](https://apis.io/apis/atomicwork/atomicwork-workflows-api/) — The workflows API from Atomicwork — 14 operation(s) for workflows.
- [Atomicwork Workspaces API](https://apis.io/apis/atomicwork/atomicwork-workspaces-api/) — The workspaces API from Atomicwork — 3 operation(s) for workspaces.
- [Atomicwork Access Management API](https://apis.io/apis/atomicwork/atomicwork-access-management-api/) — The Access Management API from Atomicwork — 8 operation(s) for access management.
- [Atomicwork Agent Groups API](https://apis.io/apis/atomicwork/atomicwork-agent-groups-api/) — The Agent Groups API from Atomicwork — 3 operation(s) for agent groups.
- [Atomicwork Audit Logs API](https://apis.io/apis/atomicwork/atomicwork-audit-logs-api/) — The Audit Logs API from Atomicwork — 3 operation(s) for audit logs.
- [Atomicwork Change Management API](https://apis.io/apis/atomicwork/atomicwork-change-management-api/) — The Change Management API from Atomicwork — 7 operation(s) for change management.
- [Atomicwork Custom Objects API](https://apis.io/apis/atomicwork/atomicwork-custom-objects-api/) — The Custom Objects API from Atomicwork — 7 operation(s) for custom objects.
- [Atomicwork Service Catalog API](https://apis.io/apis/atomicwork/atomicwork-service-catalog-api/) — The Service Catalog API from Atomicwork — 7 operation(s) for service catalog.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [server](https://apis.io/servers/atomicwork/server/)

#### Collections (16)

Postman and Open Collection request collections.

- [Atomicwork Public accessManagement API](https://apis.io/collections/atomicwork/open-atomicwork-accessmanagement-api/)
- [Atomicwork Public accessManagement agentGroups API](https://apis.io/collections/atomicwork/open-atomicwork-agentgroups-api/)
- [Atomicwork Public accessManagement assets API](https://apis.io/collections/atomicwork/open-atomicwork-assets-api/)
- [Atomicwork Public accessManagement auditLogs API](https://apis.io/collections/atomicwork/open-atomicwork-auditlogs-api/)
- [Atomicwork Public accessManagement businessHourConfig API](https://apis.io/collections/atomicwork/open-atomicwork-businesshourconfig-api/)
- [Atomicwork Public accessManagement changeManagement API](https://apis.io/collections/atomicwork/open-atomicwork-changemanagement-api/)
- [Atomicwork Public accessManagement customObjects API](https://apis.io/collections/atomicwork/open-atomicwork-customobjects-api/)
- [Atomicwork Public accessManagement entities API](https://apis.io/collections/atomicwork/open-atomicwork-entities-api/)
- [Atomicwork Public accessManagement forms API](https://apis.io/collections/atomicwork/open-atomicwork-forms-api/)
- [Atomicwork Public accessManagement problems API](https://apis.io/collections/atomicwork/open-atomicwork-problems-api/)
- [Atomicwork Public accessManagement requests API](https://apis.io/collections/atomicwork/open-atomicwork-requests-api/)
- [Atomicwork Public accessManagement serviceCatalog API](https://apis.io/collections/atomicwork/open-atomicwork-servicecatalog-api/)
- [Atomicwork Public accessManagement tags API](https://apis.io/collections/atomicwork/open-atomicwork-tags-api/)
- [Atomicwork Public accessManagement users API](https://apis.io/collections/atomicwork/open-atomicwork-users-api/)
- [Atomicwork Public accessManagement workflows API](https://apis.io/collections/atomicwork/open-atomicwork-workflows-api/)
- [Atomicwork Public accessManagement workspaces API](https://apis.io/collections/atomicwork/open-atomicwork-workspaces-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Atomicwork Public Api Overlay](https://apis.io/overlays/atomicwork/atomicwork-public-api-overlay/)

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Atomicwork Authentication](https://apis.io/security/atomicwork/atomicwork-authentication/)
- [Atomicwork Domain Security](https://apis.io/security/atomicwork/atomicwork-domain-security/)
- [Atomicwork Trust Center](https://apis.io/security/atomicwork/atomicwork-trust-center/)
- [Atomicwork Vulnerability Disclosure](https://apis.io/security/atomicwork/atomicwork-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.atomicwork.com)
- [Documentation](https://developers.atomicwork.com)
- [Getting started](https://developers.atomicwork.com/api-reference/introduction)
- [API reference](https://developers.atomicwork.com/api-reference/introduction)
- [Pricing](https://www.atomicwork.com/pricing)
- [Sign up](https://app.atomicwork.com)
- [Blog](https://www.atomicwork.com/blog)
- [Security](https://www.atomicwork.com/security)
- [Compliance](https://trust.atomicwork.com/)
- [Terms of service](https://www.atomicwork.com/terms)
- [Privacy policy](https://www.atomicwork.com/privacy)
- [Status](https://status.atomicwork.com)

## API Evangelist rating

**Kin Score 51.3** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 44.6 |
| Contract governance | 18.2 |
| Operational transparency | 18.4 |
| Developer ergonomics | 54.2 |
| Access clarity | 60.5 |

**Agent readiness 26.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | documented (partial credit) |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | yes |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | na |
| Operation Distinctiveness | — |

**Regulatory alignment 35.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/atomicwork/](https://apis.io/providers/atomicwork/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Atomicwork: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/atomicwork/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
