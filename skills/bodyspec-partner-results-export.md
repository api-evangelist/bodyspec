---
name: bodyspec-partner-results-export
description: Export a partner user's result after locating it.
api: openapi/bodyspec-openapi.json
operations:
- _list_partner_user_results_api_v1_partners__partner_id__users__user_id__results_get
- _get_partner_user_result_detail_api_v1_partners__partner_id__users__user_id__results__result_id__get
- _create_partner_user_result_export_api_v1_partners__partner_id__users__user_id__results__result_id__export_post
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bodyspec-openapi.json ; every operationId checked against the contract
---

# bodyspec-partner-results-export

Export a partner user's result after locating it.

## Steps

1. 1. Call ` _list_partner_user_results_api_v1_partners__partner_id__users__user_id__results_get ` with path parameters `partner_id` and `user_id` (supports pagination via standard query parameters).
2. 2. Call ` _get_partner_user_result_detail_api_v1_partners__partner_id__users__user_id__results__result_id__get ` with path parameters `partner_id`, `user_id`, and `result_id` to retrieve result details.
3. 3. Call ` _create_partner_user_result_export_api_v1_partners__partner_id__users__user_id__results__result_id__export_post ` with path parameters `partner_id`, `user_id`, `result_id` to create an export of the result.

## Rules

- Auth: Include a `Authorization: Bearer <token>` header (BearerAuth) or use OAuth2 token as required by the endpoint.
- Pagination: List operation may return paginated results; use `page` and `pageSize` query parameters if provided by the API.
- Idempotency: Export creation is not idempotent; avoid repeating the POST without checking prior export status.
