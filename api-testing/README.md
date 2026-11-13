
# API Testing – JSONPlaceholder

## Overview

This project demonstrates REST API testing knowledge through a structured Postman collection designed for the JSONPlaceholder demo API.

The collection includes request definitions, automated assertion scripts, reusable configuration, and positive and negative test scenarios.

The project is presented as a QA portfolio demonstration. No test execution results are claimed.

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

These status codes represent the expected validation criteria defined in the collection. They are not reported as observed execution results.

## Automated Assertions

The Postman collection includes scripts designed to validate:

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
│   └── api-test-documentation.md
├── environments/
│   └── jsonplaceholder.postman_environment.json
└── README.md
```

## Documentation and Configuration

The Postman collection and environment are included as portfolio deliverables.

The collection demonstrates REST API test design, reusable request configuration, and automated assertion scripts.

The accompanying documentation describes the testing approach, expected responses, validation criteria, and technical limitations.

## Configuration

The collection uses variables to make requests reusable and configurable.

| Variable | Purpose |
|---|---|
| `baseUrl` | API base URL |
| `postId` | Existing post identifier |
| `nonExistingUserId` | User ID used for negative filtering |
| `nonExistingPostId` | Non-existing resource identifier |
| `maxResponseTimeMs` | Response-time threshold in milliseconds |

## Important Limitations

JSONPlaceholder is a mock REST API.

POST, PUT, and DELETE operations simulate successful write operations but do not persist changes to the underlying database.

Response-time assertions are basic threshold checks and should not be interpreted as formal performance or load testing.

## Project Status

- Postman collection designed and documented.
- Positive and negative scenarios included.
- Automated assertions prepared.
- Environment configuration documented.
- Portfolio documentation completed.

No test execution results or verified defects are claimed.

## Author

**Mariana Camps**

QA Testing | Manual Testing | API Testing | AI Training & Evaluation
