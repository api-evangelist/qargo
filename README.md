# Qargo

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

Qargo is an intelligent transport management platform (TMS) for road carriers, freight forwarders and 3PLs, using AI to automate operational and administrative work across planning, execution, tracking and accounting. Qargo publishes a public Qargo TMS API (OpenAPI 3.1, v1.2.0, base https://api.qargo.com) exposing tenant-level integration and operational endpoints for orders, trips, companies, resources, documents, tasks and accounting, plus inbound and outbound webhooks and separate Subcontractor and Customer APIs. Service-to-service authentication uses OAuth2 client-credentials (JWT); webhooks use HTTP Basic. Qargo is a Balderton Capital portfolio company.

**Areas:** Company · Transport Management · Logistics · Supply Chain · Freight · TMS · Accounting · Webhook

## Qargo on APIs.io

Everything profiled for Qargo is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/qargo/](https://apis.io/providers/qargo/)** — or go straight to one of the APIs or properties below.

### APIs (22)

- [Qargo Subcontractor API](https://apis.io/apis/qargo/qargo-subcontractor-api/) — Fleet dispatch and subcontractor-specific endpoints for transportation management.
- [Qargo Customer API](https://apis.io/apis/qargo/qargo-customer-api/) — Customer portal endpoints for order tracking, status monitoring and customer-facing operations.
- [Qargo API / Accounting API](https://apis.io/apis/qargo/qargo-api-accounting-api/) — The API / Accounting API from Qargo — 33 operation(s) for api / accounting.
- [Qargo API / Authentication API](https://apis.io/apis/qargo/qargo-api-authentication-api/) — The API / Authentication API from Qargo — 1 operation(s) for api / authentication.
- [Qargo API / Company API](https://apis.io/apis/qargo/qargo-api-company-api/) — The API / Company API from Qargo — 6 operation(s) for api / company.
- [Qargo API / Document API](https://apis.io/apis/qargo/qargo-api-document-api/) — The API / Document API from Qargo — 2 operation(s) for api / document.
- [Qargo API / Order API](https://apis.io/apis/qargo/qargo-api-order-api/) — The API / Order API from Qargo — 8 operation(s) for api / order.
- [Qargo API / Resource API](https://apis.io/apis/qargo/qargo-api-resource-api/) — The API / Resource API from Qargo — 8 operation(s) for api / resource.
- [Qargo API / Task API](https://apis.io/apis/qargo/qargo-api-task-api/) — The API / Task API from Qargo — 3 operation(s) for api / task.
- [Qargo API / Trip API](https://apis.io/apis/qargo/qargo-api-trip-api/) — The API / Trip API from Qargo — 3 operation(s) for api / trip.
- [Qargo System API](https://apis.io/apis/qargo/qargo-system-api/) — The System API from Qargo — 1 operation(s) for system.
- [Qargo Use case / Accounting API](https://apis.io/apis/qargo/qargo-use-case-accounting-api/) — Required role: `API_ACCOUNTING`. See [Accounting](/docs/section/accounting) for more information.
- [Qargo Use case / Document import API](https://apis.io/apis/qargo/qargo-use-case-document-import-api/) — This section provides an overview of all available methods to import documents into Qargo. ![Document import paths…
- [Qargo Use case / E-invoicing API](https://apis.io/apis/qargo/qargo-use-case-e-invoicing-api/) — Required api role: not applicable Purpose: This interface allows an external party to send e-invoices in a structured format. A…
- [Qargo Use case / Fleet dispatch API](https://apis.io/apis/qargo/qargo-use-case-fleet-dispatch-api/) — Required api role: not applicable (push/push) Purpose: This interface allows an external party to integrate with driver apps and on board computer systems.…
- [Qargo Use case / Intermodal [partner] API](https://apis.io/apis/qargo/qargo-use-case-intermodal-partner-api/) — Note: this is currently only a specification meant as a preview. Implementation is still pending.
- [Qargo Use case / Location booking API](https://apis.io/apis/qargo/qargo-use-case-location-booking-api/) — Required api role: not applicable (push/push) Purpose: This interface allows an external party to integrate with warehouse management systems and location…
- [Qargo Use case / Order API](https://apis.io/apis/qargo/qargo-use-case-order-api/) — Required api role: `API_ORDER` All endpoints related to order creation and status retrieval/subscription. ### Getting started See [this…
- [Qargo Use case / Subcontractor dispatch API](https://apis.io/apis/qargo/qargo-use-case-subcontractor-dispatch-api/) — Required api role: not applicable (push/push) Purpose: This interface allows an external party to integrate with 3rd party transport management systems for…
- [Qargo Use case / Tracking API](https://apis.io/apis/qargo/qargo-use-case-tracking-api/) — The Use case / Tracking API from Qargo — 1 operation(s) for use case / tracking.
- [Qargo Use case / Trip import API](https://apis.io/apis/qargo/qargo-use-case-trip-import-api/) — Required api role: `API_TRIP` Purpose: This interface allows an external system (e.g. a route optimisation tool) to send fully planned trips into Qargo.…
- [Qargo Use case / Visibility API](https://apis.io/apis/qargo/qargo-use-case-visibility-api/) — The Use case / Visibility API from Qargo — 2 operation(s) for use case / visibility.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Qargo Webhooks](https://apis.io/asyncapis/qargo/qargo-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Qargo API documentation](https://apis.io/servers/qargo/qargo-api-documentation/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Qargo Agentic Access](https://apis.io/agentic-access/qargo/qargo-agentic-access/)

#### Collections (24)

Postman and Open Collection request collections.

- [Qargo TMS API / Accounting API](https://apis.io/collections/qargo/open-qargo-api-accounting-api/)
- [Qargo TMS API / Accounting API / Authentication API](https://apis.io/collections/qargo/open-qargo-api-authentication-api/)
- [Qargo TMS API / Accounting API / Company API](https://apis.io/collections/qargo/open-qargo-api-company-api/)
- [Qargo TMS API / Accounting API / Document API](https://apis.io/collections/qargo/open-qargo-api-document-api/)
- [Qargo TMS API / Accounting API / Order API](https://apis.io/collections/qargo/open-qargo-api-order-api/)
- [Qargo TMS API / Accounting API / Resource API](https://apis.io/collections/qargo/open-qargo-api-resource-api/)
- [Qargo TMS API / Accounting API / Task API](https://apis.io/collections/qargo/open-qargo-api-task-api/)
- [Qargo TMS API / Accounting API / Trip API](https://apis.io/collections/qargo/open-qargo-api-trip-api/)
- [Qargo TMS API / Accounting System API](https://apis.io/collections/qargo/open-qargo-system-api/)
- [Qargo TMS API / Accounting Use case / Accounting API](https://apis.io/collections/qargo/open-qargo-use-case-accounting-api/)
- [Qargo TMS API / Accounting Use case / Customer portal API](https://apis.io/collections/qargo/open-qargo-use-case-customer-portal-api/)
- [Qargo TMS API / Accounting Use case / Document import API](https://apis.io/collections/qargo/open-qargo-use-case-document-import-api/)
- [Qargo TMS API / Accounting Use case / E-invoicing API](https://apis.io/collections/qargo/open-qargo-use-case-e-invoicing-api/)
- [Qargo TMS API / Accounting Use case / Fleet dispatch API](https://apis.io/collections/qargo/open-qargo-use-case-fleet-dispatch-api/)
- [Qargo TMS API / Accounting Use case / Intermodal [partner] API](https://apis.io/collections/qargo/open-qargo-use-case-intermodal-partner-api/)
- [Qargo TMS API / Accounting Use case / Location booking API](https://apis.io/collections/qargo/open-qargo-use-case-location-booking-api/)
- [Qargo TMS API / Accounting Use case / Master data sync API](https://apis.io/collections/qargo/open-qargo-use-case-master-data-sync-api/)
- [Qargo TMS API / Accounting Use case / Order API](https://apis.io/collections/qargo/open-qargo-use-case-order-api/)
- [Qargo TMS API / Accounting Use case / Subcontractor dispatch API](https://apis.io/collections/qargo/open-qargo-use-case-subcontractor-dispatch-api/)
- [Qargo TMS API / Accounting Use case / Tracking API](https://apis.io/collections/qargo/open-qargo-use-case-tracking-api/)
- [Qargo TMS API / Accounting Use case / Trip import API](https://apis.io/collections/qargo/open-qargo-use-case-trip-import-api/)
- [Qargo TMS API / Accounting Use case / Visibility API](https://apis.io/collections/qargo/open-qargo-use-case-visibility-api/)
- [Qargo TMS API / Accounting Webhooks / Inbound API](https://apis.io/collections/qargo/open-qargo-webhooks-inbound-api/)
- [Qargo TMS API / Accounting Webhooks / Outbound API](https://apis.io/collections/qargo/open-qargo-webhooks-outbound-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Qargo Tms Overlay](https://apis.io/overlays/qargo/qargo-tms-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Qargo Authentication](https://apis.io/security/qargo/qargo-authentication/)
- [Qargo Domain Security](https://apis.io/security/qargo/qargo-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.qargo.com/)
- [Documentation](https://api-docs.qargo.com/docs)
- [Getting started](https://api-docs.qargo.com/docs/section/authentication/the-api-call-to-request-tokens)
- [API reference](https://api-docs.qargo.com/docs)
- [Support](https://help.qargo.com/en/)
- [Changelog](https://api-docs.qargo.com/docs/section/changelog)
- [Blog](https://www.qargo.com/resources/news-and-blogs/)
- [Terms of service](https://www.qargo.com/terms-and-conditions/)
- [Privacy policy](https://www.qargo.com/privacy-notice/)

## API Evangelist rating

**Kin Score 48.2** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 55.7 |
| Contract governance | 4.5 |
| Operational transparency | 31.6 |
| Developer ergonomics | 60.1 |
| Access clarity | 27.6 |

**Agent readiness 37.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | documented (partial credit) |
| Auth Clarity | negotiable (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | mostly (partial credit) |

**Regulatory alignment 34.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/qargo/](https://apis.io/providers/qargo/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Qargo: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/qargo/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
