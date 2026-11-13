# API Testing Documentation

**Collection:** QA API Testing - JSONPlaceholder (v2.0)

**Environment:** QA - JSONPlaceholder

## Overview

This document describes the API testing collection designed to demonstrate REST API testing concepts, request configuration, automated assertions, and response validation using Postman.

The collection uses JSONPlaceholder, a public mock REST API.

## Testing Scope

The collection includes the following scenarios:

| Method | Scenario | Expected Status |
|---|---|---:|
| GET | Retrieve all posts | 200 |
| GET | Retrieve a post by ID | 200 |
| POST | Create a post | 201 |
| PUT | Update a post | 200 |
| DELETE | Delete a post | 200, 202 or 204 |
| GET | Filter posts using a non-existing user ID | 200 |
| GET | Retrieve a non-existing post | 404 |

Expected status codes are defined as test assertions and should be interpreted according to the demo API contract.

## Automated Validation

The collection includes JavaScript assertions designed to validate:

- HTTP response status codes.
- Response content type.
- JSON response structure.
- Required properties and data types.
- Resource identifier consistency.
- Expected response values.
- Empty and non-empty response collections.
- Response-time thresholds.

## Environment Configuration

The collection uses configurable variables to support reusable requests.

| Variable | Description |
|---|---|
| `baseUrl` | API base URL |
| `postId` | Existing post identifier |
| `nonExistingUserId` | Identifier used for negative filtering |
| `nonExistingPostId` | Identifier for a non-existing resource |
| `maxResponseTimeMs` | Maximum response-time threshold |

## API Endpoints

**Base URL:** https://jsonplaceholder.typicode.com

**Resource:** `/posts`

The collection covers standard REST operations using GET, POST, PUT, and DELETE methods.

## Testing Approach

The collection was designed to demonstrate:

- Positive and negative testing scenarios.
- HTTP response validation.
- Data structure and type validation.
- Request and environment variable management.
- Automated assertions using Postman scripts.

## Limitations

JSONPlaceholder is a mock REST API.

POST, PUT, and DELETE operations simulate successful write operations but do not persist changes to the underlying database.

Response-time assertions represent basic threshold checks and are
