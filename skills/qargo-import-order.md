---
name: Import an order into Qargo and track its status
description: Authenticate to the Qargo TMS API, import (create) an order, poll its import status, then read order details and operational status.
api: openapi/qargo-tms-openapi-original.yml
operations: [generate_token_v1_auth_token_post, import_order_v1_orders_order_upload_post, get_order_import_status_v1_orders_order_upload__upload_id__get, get_order_details_v1_orders_order__order_id__get, order_status_v1_orders_order__order_id__status_get]
---

# Import an order into Qargo

Use this skill to push a transport order into Qargo and confirm it landed.

## Auth
1. Call `generate_token_v1_auth_token_post` — `POST https://api.qargo.com/v1/auth/token` with HTTP Basic (`client_id:secret_id`, base64) and `Content-Type: application/json`, empty body. Store the returned JWT and `expires_in`; send it as `Authorization: Bearer <token>` on every subsequent call. Refresh when it expires.

## Steps
2. `import_order_v1_orders_order_upload_post` — `POST /v1/orders/order/upload` with the order payload. Capture the returned `upload_id`.
3. `get_order_import_status_v1_orders_order_upload__upload_id__get` — `GET /v1/orders/order/upload/{upload_id}`. Poll until the import completes; on success it yields the created `order_id`.
4. `get_order_details_v1_orders_order__order_id__get` — `GET /v1/orders/order/{order_id}` to read back the persisted order.
5. `order_status_v1_orders_order__order_id__status_get` — `GET /v1/orders/order/{order_id}/status` for operational status (pickup/delivery stops).

## Rules
- Validation failures return HTTP 400 with a `ValidationErrorResponse`: a non-empty `errors[]` array of `ValidationErrorDetail` (`message`, `field`, `path`, `detail`). Handle one and many failures the same way.
- Honour `Retry-After` on HTTP 429.
- No idempotency-key header exists; use `external_id` to correlate and avoid duplicate imports.
- See conventions/qargo-conventions.yml and errors/qargo-problem-types.yml.
