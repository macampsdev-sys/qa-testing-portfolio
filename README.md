# Postman API Testing – JSONPlaceholder

## Overview
A Postman collection demonstrating API test design and automated response validation against the JSONPlaceholder demo REST API.

## Coverage
- GET all posts: status, JSON content type, array shape, required fields, data types, response time.
- GET post by ID: status, ID consistency, required fields and data types.
- POST: response status and request/response field consistency.
- PUT: response status, resource ID and replacement-field consistency.
- DELETE: successful HTTP status handling.
- Negative data scenario: unmatched `userId` filter returns an empty collection.
- Negative resource scenario: request for a non-existing post.

## Files
- `collections/jsonplaceholder.postman_collection.json`
- `environments/jsonplaceholder.postman_environment.json`
- `docs/execution-report.md`

## Import and run
1. Open Postman.
2. Select **Import** and import the collection JSON.
3. Import the environment JSON.
4. Select the `QA - JSONPlaceholder` environment.
5. Run the collection using Collection Runner.
6. Review each request's **Test Results** and export the run report if required.

## Configuration
`baseUrl` is stored in the environment. `postId`, `nonExistingUserId`, `nonExistingPostId`, and `maxResponseTimeMs` are collection variables and can be changed in the collection's Variables tab.

## Important service limitations
JSONPlaceholder is a mock API. POST, PUT and DELETE responses simulate successful write operations but do not persist changes to the underlying data. A successful response therefore validates the mock response contract, not durable creation, update, or deletion.

The non-existing-resource scenario expects HTTP 404. Verify the live response when executing the collection; if the service contract differs, record the observed behavior and update the assertion based on evidence rather than forcing a pass.

## Scope and limitations
This collection is an educational portfolio artifact. Response-time assertions use a configurable threshold and can vary with network conditions. They are not a performance benchmark or SLA test.

## Author
Mariana Camps | QA Testing | API Testing | AI Training & Evaluation
