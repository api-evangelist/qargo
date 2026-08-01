---
name: Create and reconcile a Qargo sales invoice
description: Authenticate, create a sales invoice, retrieve it and its documents, then report payment status back to Qargo.
api: openapi/qargo-tms-openapi-original.yml
operations: [generate_token_v1_auth_token_post, Create_a_sales_invoice_v1_accounting_sales_invoice__post, Retrieve_sales_invoice_v1_accounting_sales_invoice__id__get, Retrieve_sales_invoice_documents_v1_accounting_sales_invoice__id__documents_get, Report_payment_status_for_sales_invoice_v1_accounting_sales_invoice__id__payment_update_status_post]
---

# Create and reconcile a Qargo sales invoice

Use this skill for the accounting use case: push a sales invoice into Qargo and close the loop on payment.

## Auth
1. `generate_token_v1_auth_token_post` — obtain a JWT from `POST /v1/auth/token` (HTTP Basic client credentials). Send `Authorization: Bearer <token>` thereafter.

## Steps
2. `Create_a_sales_invoice_v1_accounting_sales_invoice__post` — `POST /v1/accounting/sales-invoice/`. Capture the returned invoice `id`.
3. `Retrieve_sales_invoice_v1_accounting_sales_invoice__id__get` — `GET /v1/accounting/sales-invoice/{id}` to confirm; responses include `e_invoicing` registration metadata.
4. `Retrieve_sales_invoice_documents_v1_accounting_sales_invoice__id__documents_get` — `GET /v1/accounting/sales-invoice/{id}/documents` for generated PDFs.
5. `Report_payment_status_for_sales_invoice_v1_accounting_sales_invoice__id__payment_update_status_post` — `POST /v1/accounting/sales-invoice/{id}/payment/update-status` to write the payment state back.

## Rules
- Use the hyphenated paths (`/sales-invoice/`), not the deprecated underscore variants (`/sales_invoice/`) — see lifecycle/qargo-lifecycle.yml.
- Errors follow the standard `ValidationErrorResponse` envelope; honour `Retry-After` on 429.
- See conventions/qargo-conventions.yml.
