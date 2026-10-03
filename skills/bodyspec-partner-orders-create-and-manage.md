---
name: bodyspec-partner-orders-create-and-manage
description: Create a new partner order, view the list of orders, retrieve the created order, and update it.
api: openapi/bodyspec-openapi.json
operations:
- _create_order_api_v1_partners__partner_id__orders_post
- _list_orders_api_v1_partners__partner_id__orders_get
- _get_order_api_v1_partners__partner_id__orders__order_id__get
- _update_order_api_v1_partners__partner_id__orders__order_id__patch
generated: '2026-10-02'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/bodyspec-openapi.json ; every operationId checked against the contract
---

# bodyspec-partner-orders-create-and-manage

Create a new partner order, view the list of orders, retrieve the created order, and update it.

## Steps

1. 1. Use ` _create_order_api_v1_partners__partner_id__orders_post ` with header `Authorization: Bearer <token>` and path parameter `partner_id`.
2. 2. Use ` _list_orders_api_v1_partners__partner_id__orders_get ` with header `Authorization: Bearer <token>` and path parameter `partner_id`.
3. 3. Use ` _get_order_api_v1_partners__partner_id__orders__order_id__get ` with header `Authorization: Bearer <token>` and path parameters `partner_id` and `order_id`.
4. 4. Use ` _update_order_api_v1_partners__partner_id__orders__order_id__patch ` with header `Authorization: Bearer <token>` and path parameters `partner_id` and `order_id`.

## Rules

- Auth header: `Authorization: Bearer <token>` (BearerAuth).
