---
name: Submit a GUARD credit-card underwriting
description: Score a customer for a partner-issued credit card with alt.bank GUARD and receive the risk band, score, and suggested limit via callback.
api: openapi/altbank-guard-openapi.yml
operations:
  - submitUnderwriting
method: generated
generated: '2026-07-17'
source: https://developers.altbank.ai/docs/guard-api
---

# Submit a GUARD credit-card underwriting

Use alt.bank's GUARD engine to underwrite a customer for a partner-issued credit
card. The flow is asynchronous: you submit the request and GUARD delivers the
result to your callback endpoint.

## Prerequisites

- A 64-character alphanumeric partner token from alt.bank, sent on every request
  in the `X-Partner-Auth` header (see `authentication/altbank-authentication.yml`).
- A callback URL registered with alt.bank **out-of-band** before first use —
  GUARD POSTs the underwriting result there (see `asyncapi/altbank-guard-webhooks.yml`).
- For testing, use the sandbox host `https://guard.stg.altbank.ai` with the test
  CPFs alt.bank provides (see `sandbox/altbank-sandbox.yml`). Never invent CPFs.

## Steps

1. **Submit the underwriting** — call `submitUnderwriting`:
   `POST https://guard.altbank.ai/api/partner/credit/cards/underwritings`
   with header `X-Partner-Auth: <token>` and a JSON body identifying the
   applicant by `cpf`. Expect a `202 Accepted` acknowledgement — the result is
   NOT in this response.

2. **Receive the result on your callback** — GUARD POSTs an `UnderwritingResult`
   to your configured callback URL with:
   - `riskBand` — the score-based risk band,
   - `score` — the model's final score,
   - `limit` — the suggested initial credit line.

3. **Interpret sentinels** — treat `-1` on `riskBand`, `score`, or `limit` as
   "not scored" (cost-saving policy active or model could not compute). A `limit`
   of `0` means the applicant was **not approved**; a positive `limit` is the
   approved initial credit line.

## Notes

- Authentication failures return `401`; verify the `X-Partner-Auth` token.
- No idempotency-key contract is documented — do not assume safe automatic retries
  of the submit call.
