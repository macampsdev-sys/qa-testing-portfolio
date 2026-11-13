# API Testing – JSONPlaceholder

## Overview

This project demonstrates practical REST API testing using Postman and the JSONPlaceholder demo API.

The test suite focuses on request validation, response assertions, positive and negative scenarios, data integrity checks, and basic response-time thresholds.

## Tools & Technologies

- Postman
- REST API
- JavaScript (Postman test scripts)
- JSON
- Git and GitHub

## API Under Test

**Base URL:** https://jsonplaceholder.typicode.com

JSONPlaceholder is a public mock REST API used for testing and prototyping.

## Test Coverage

| Method | Scenario | Expected Status |
|---|---|---:|
| GET | Retrieve all posts | 200 |
| GET | Retrieve post by ID | 200 |
| POST | Create a post | 201 |
| PUT | Update a post | 200 |
| DELETE | Delete a post | 200, 202 or 204 |
| GET | Filter posts using a non-existing user ID | 200 |
| GET | Retrieve a non-existing post | 404 |

Expected responses must be verified against the actual API behavior during execution.

## Automated Assertions

The Postman collection includes automated checks for:

- HTTP status codes.
- Response content type.
- JSON structure and data types.
- Required properties and expected values.
- Resource identifier consistency.
- Empty and non-empty response collections.
- Response-time thresholds.

## Collection Structure

```text
api-testing/
├── collections/
│   └── jsonplaceholder.postman_collection.json
├── docs/
│   └── execution-report.md
├── environments/
│   └── jsonplaceholder.postman_environment.json
└── README.md
```

## Execution Instructions

1. Open Postman.
2. Import the collection from `collections/`.
3. Import the environment from `environments/`.
4. Select the `QA - JSONPlaceholder` environment.
5. Verify that the `baseUrl` variable is configured.
6. Run individual requests or execute the complete collection using Collection Runner.
7. Review the test results and record the actual outcomes.

## Configuration

The collection uses variables to make requests reusable and configurable.

| Variable | Purpose |
|---|---|
| `baseUrl` | API base URL |
| `postId` | Existing post identifier |
| `nonExistingUserId` | User ID used for negative filtering |
| `nonExistingPostId` | Non-existing resource identifier |
| `maxResponseTimeMs` | Response-time threshold in milliseconds |

## Execution Reporting

Execution results, observations, and evidence will be documented in:

`docs/execution-report.md`

No execution results are assumed or reported until the collection has been run and verified.

## Important Limitations

JSONPlaceholder is a mock REST API.

POST, PUT, and DELETE operations simulate successful write operations but do not persist changes to the underlying database.

Response-time assertions are basic threshold checks and should not be interpreted as formal performance or load testing.

## Project Status

- Collection v2.0 created.
- Positive and negative scenarios documented.
- Automated assertions implemented.
- Environment configuration prepared.
- Execution and result verification pending.

## Author

**Mariana Camps**

QA Testing | Manual Testing | API Testing | AI Training & Evaluation
