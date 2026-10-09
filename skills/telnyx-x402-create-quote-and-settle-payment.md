---
name: telnyx-x402-create-quote-and-settle-payment
description: Create a payment quote for an X402 transaction and then settle the payment.
api: openapi/telnyx-openapi.json
operations:
- createX402Quote
- settleX402Payment
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/telnyx-openapi.json ; every operationId checked against the contract
---

# telnyx-x402-create-quote-and-settle-payment

Create a payment quote for an X402 transaction and then settle the payment.

## Steps

1. 1. `createX402Quote` – send required quote fields in the request body as defined in the contract.
2. 2. `settleX402Payment` – use the quote ID returned from the previous step in the request body to settle the payment.

## Rules

- Auth: Include a `Authorization: Bearer <token>` header (BearerAuth).
- Idempotency: No specific idempotency key is documented for these endpoints.
- Rate limit: 50 messages/second; exceeding the limit returns no specific HTTP status code.
