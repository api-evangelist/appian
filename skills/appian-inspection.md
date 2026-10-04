---
name: appian-inspection
description: Create an inspection for a package and then retrieve its results.
api: openapi/appian-inspection-api-openapi.yml
operations:
- createInspection
- getInspectionResults
generated: '2026-10-03'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/appian-inspection-api-openapi.yml ; every operationId checked against the contract
---

# appian-inspection

Create an inspection for a package and then retrieve its results.

## Steps

1. 1. Call `createInspection` with the required request body and include the header `appian-api-key` for authentication.
2. 2. Call `getInspectionResults` with the path parameter `inspectionUuid` returned from the previous step and include the header `appian-api-key` for authentication.

## Rules

- Authentication: Provide the API key in the `appian-api-key` header.
- Idempotency: Not applicable.
- Pagination: Not applicable.
- Error handling: Follow the HTTP status codes returned by each endpoint.
