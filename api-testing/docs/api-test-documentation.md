# API Test Execution Report

**Collection:** QA API Testing - JSONPlaceholder (v2.0)  
**Environment:** QA - JSONPlaceholder  
**Execution date:** Pending  
**Postman version:** Record at execution  
**Executed by:** Mariana Camps  
**Status:** Not executed / pending evidence

## Execution summary

| Metric | Result |
|---|---:|
| Total requests | 7 |
| Passed requests | Pending |
| Failed requests | Pending |
| Blocked requests | Pending |
| Not executed | 7 |

## Request-level results

| Request | Expected behavior | Actual status / result | Test result | Evidence / notes |
|---|---|---|---|---|
| GET all posts | 200; JSON array with expected fields | Pending | Not executed | |
| GET post by ID | 200; requested ID and fields returned | Pending | Not executed | |
| POST create | 201; response echoes submitted fields | Pending | Not executed | Mock response; no persistence |
| PUT replace | 200; response echoes replacement fields | Pending | Not executed | Mock response; no persistence |
| DELETE | Successful status (200, 202 or 204) | Pending | Not executed | Mock response; no persistence |
| GET unmatched user filter | 200; empty array | Pending | Not executed | |
| GET non-existing post | 404 expected | Pending | Not executed | Verify actual service contract |

## Defects and observations

Record confirmed deviations only. Include request name, timestamp, response status, relevant response excerpt, reproduction details, and severity / priority where applicable.

## Limitations
- JSONPlaceholder simulates write operations; changes are not persisted.
- Response-time checks are affected by network conditions.
- The non-existing-resource response must be confirmed during execution.
- This report must be completed with actual Postman run results; no results are pre-populated.

## Conclusion
Pending execution. No quality conclusion is made until the collection has been run and results reviewed.
