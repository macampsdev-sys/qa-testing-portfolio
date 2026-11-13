
# API Testing – JSONPlaceholder

## Overview

This project demonstrates practical API testing skills using Postman and the JSONPlaceholder REST API.

The collection covers HTTP methods, response validation, automated assertions and basic API quality checks.

## Tools

- Postman
- REST API
- JavaScript (Postman test scripts)
- JSON
- GitHub

## Test Coverage

| HTTP Method | Scenario | Expected Status |
|---|---|---|
| GET | Retrieve all posts | 200 |
| GET | Retrieve post by ID | 200 |
| POST | Create a post | 201 |
| PUT | Update a post | 200 |
| DELETE | Delete a post | 200 or 204 |

## Automated Assertions

The collection includes validations for:

- HTTP status codes.
- Response data types.
- JSON structure.
- Required properties.
- Returned resource identifiers.
- Expected response values.

## Execution Instructions

1. Download the Postman collection from this repository.
2. Open Postman.
3. Import the JSON collection.
4. Execute individual requests or run the entire collection.
5. Review the automated test results.

## API Documentation

https://jsonplaceholder.typicode.com/

## Important Limitations

JSONPlaceholder is a mock REST API.

POST, PUT and DELETE operations simulate successful write operations but do not persist changes to the underlying database.

Therefore, this project demonstrates API request validation and response assertions, not persistent database modification.

## Project Status

Collection created. Execution results and evidence will be documented separately after validation.

## Author

Mariana Camps  
QA Testing | API Testing | AI Evaluation
