---
name: bodyspec-manage-partner-webhooks
description: Create, view, update, list, and delete partner webhooks.
api: openapi/bodyspec-openapi.json
operations:
- list_webhooks_api_v1_partners__partner_id__webhooks_get
- create_webhook_api_v1_partners__partner_id__webhooks_post
- get_webhook_api_v1_partners__partner_id__webhooks__webhook_id__get
- update_webhook_api_v1_partners__partner_id__webhooks__webhook_id__patch
- delete_webhook_api_v1_partners__partner_id__webhooks__webhook_id__delete
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bodyspec-openapi.json ; every operationId checked against the contract
---

# bodyspec-manage-partner-webhooks

Create, view, update, list, and delete partner webhooks.

## Steps

1. 1. `list_webhooks_api_v1_partners__partner_id__webhooks_get` – requires `Authorization: Bearer <token>` header; path parameter `partner_id`.
2. 2. `create_webhook_api_v1_partners__partner_id__webhooks_post` – requires `Authorization: Bearer <token>` header; path parameter `partner_id`; request body with webhook definition.
3. 3. `get_webhook_api_v1_partners__partner_id__webhooks__webhook_id__get` – requires `Authorization: Bearer <token>` header; path parameters `partner_id` and `webhook_id`.
4. 4. `update_webhook_api_v1_partners__partner_id__webhooks__webhook_id__patch` – requires `Authorization: Bearer <token>` header; path parameters `partner_id` and `webhook_id`; request body with fields to modify.
5. 5. `delete_webhook_api_v1_partners__partner_id__webhooks__webhook_id__delete` – requires `Authorization: Bearer <token>` header; path parameters `partner_id` and `webhook_id`.

## Rules

- All requests must include an `Authorization: Bearer <token>` header (BearerAuth).
- Use the server base URL `https://app.bodyspec.com` for all calls.
- Responses follow standard HTTP status codes: 200/201 for success, 4xx for client errors, 5xx for server errors.
