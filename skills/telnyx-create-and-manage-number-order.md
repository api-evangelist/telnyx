---
name: telnyx-create-and-manage-number-order
description: Create a new phone number order, retrieve its details, and list all existing number orders.
api: openapi/telnyx-openapi.json
operations:
- CreateNumberOrder
- RetrieveNumberOrder
- ListNumberOrders
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/telnyx-openapi.json ; every operationId checked against the contract
---

# telnyx-create-and-manage-number-order

Create a new phone number order, retrieve its details, and list all existing number orders.

## Steps

1. 1. Call `CreateNumberOrder` with the required request body fields for the order.
2. 2. Call `RetrieveNumberOrder` using the `number_order_id` returned from step 1.
3. 3. Call `ListNumberOrders` to view all number orders.

## Rules

- Auth: Include a Bearer token in the `Authorization` header (BearerAuth).
