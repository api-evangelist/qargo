---
name: Sync master data (companies and resources) into Qargo
description: Authenticate, then create/update companies and fleet resources and incrementally list them for master-data synchronisation.
api: openapi/qargo-tms-openapi-original.yml
operations: [generate_token_v1_auth_token_post, create_company_v1_companies_company_post, list_companies_v1_companies_company_get, Create_resource_v1_resources_resource_post, List_resources_v1_resources_resource_get, Patch_resource_v1_resources_resource__resource_id__patch]
---

# Sync master data into Qargo

Use this skill for the master-data-sync use case: keep companies (customers/suppliers) and resources (vehicles/drivers) in step with an external system.

## Auth
1. `generate_token_v1_auth_token_post` — obtain a JWT from `POST /v1/auth/token`; send `Authorization: Bearer <token>`.

## Steps
2. `create_company_v1_companies_company_post` — `POST /v1/companies/company` to create a company. Set `external_id` to your source-system key.
3. `list_companies_v1_companies_company_get` — `GET /v1/companies/company` to reconcile; cursor-paginated.
4. `Create_resource_v1_resources_resource_post` — `POST /v1/resources/resource` to add a fleet resource.
5. `List_resources_v1_resources_resource_get` — `GET /v1/resources/resource` with `updated_after` + `cursor` for incremental pulls; filter by `external_id`/`external_id:in` and `resource_type`.
6. `Patch_resource_v1_resources_resource__resource_id__patch` — `PATCH /v1/resources/resource/{resource_id}` to apply changes (e.g. allocate a `resource_group`).

## Rules
- There is no idempotency key; use `external_id` to upsert and avoid duplicates.
- Paginate with `cursor`; pull incrementally with `updated_after` — see conventions/qargo-conventions.yml.
- Errors follow the `ValidationErrorResponse` envelope; honour `Retry-After` on 429.
