
# Test Cases & Traceability Matrix – SauceDemo

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Application:** https://www.saucedemo.com/  
**Document Version:** 1.0  
**Testing Type:** Manual Functional Testing  
**Execution Status:** Not Executed

---

## 1. Test Coverage Overview

This document defines the functional test scenarios designed to validate the main user journeys of the SauceDemo e-commerce application.

Test cases are organized by functional module and prioritized according to business impact and risk.

## 2. Test Execution Status

| Status | Description |
|---|---|
| NOT EXECUTED | Test has not been executed |
| PASSED | Actual result matches expected result |
| FAILED | Actual result differs from expected result |
| BLOCKED | Execution cannot continue |
| NOT APPLICABLE | Test is outside the applicable scope |

## 3. Test Cases

### Module A – Authentication

| ID | Scenario | Priority | Preconditions | Expected Result | Status |
|---|---|---|---|---|---|
| TC-001 | Login with valid credentials | P1 | Login page accessible | User is redirected to inventory | NOT EXECUTED |
| TC-002 | Login with invalid username | P1 | Login page accessible | Authentication error is displayed | NOT EXECUTED |
| TC-003 | Login with invalid password | P1 | Login page accessible | Authentication error is displayed | NOT EXECUTED |
| TC-004 | Login with empty credentials | P2 | Login page accessible | Input validation error is displayed | NOT EXECUTED |
| TC-005 | Login with locked account | P1 | Login page accessible | Access is denied with an appropriate message | NOT EXECUTED |

### Module B – Product Inventory

| ID | Scenario | Priority | Preconditions | Expected Result | Status |
|---|---|---|---|---|---|
| TC-006 | Verify inventory loading | P1 | Standard user authenticated | Inventory page loads successfully | NOT EXECUTED |
| TC-007 | Validate product information | P2 | Inventory page accessible | Product names, prices and images are displayed | NOT EXECUTED |
| TC-008 | Sort products alphabetically | P2 | Inventory page accessible | Products are sorted A–Z | NOT EXECUTED |
| TC-009 | Sort products by ascending price | P2 | Inventory page accessible | Products are sorted from lowest to highest price | NOT EXECUTED |

### Module C – Shopping Cart

| ID | Scenario | Priority | Preconditions | Expected Result | Status |
|---|---|---|---|---|---|
| TC-010 | Add one product to cart | P1 | Inventory page accessible | Cart counter reflects one item | NOT EXECUTED |
| TC-011 | Add multiple products | P1 | Inventory page accessible | Cart counter reflects selected quantity | NOT EXECUTED |
| TC-012 | Remove product from inventory | P2 | Product previously added | Product is removed from cart | NOT EXECUTED |
| TC-013 | Verify cart contents | P1 | At least one product added | Selected products appear in cart | NOT EXECUTED |

### Module D – Checkout

| ID | Scenario | Priority | Preconditions | Expected Result | Status |
|---|---|---|---|---|---|
| TC-014 | Start checkout process | P1 | Cart contains a product | Checkout information page opens | NOT EXECUTED |
| TC-015 | Submit empty checkout information | P1 | Checkout information page accessible | Required field validation is displayed | NOT EXECUTED |
| TC-016 | Submit incomplete customer information | P2 | Checkout information page accessible | Missing required information is identified | NOT EXECUTED |
| TC-017 | Complete purchase workflow | P1 | Valid customer information available | Order confirmation is displayed | NOT EXECUTED |
| TC-018 | Verify order summary | P1 | Checkout overview accessible | Products, quantities and totals are displayed correctly | NOT EXECUTED |

---

## 4. Detailed Test Case Specification

The following specification defines the required execution record for each test case.

| Field | Description |
|---|---|
| Test Case ID | Unique test identifier |
| Preconditions | Required initial application state |
| Test Data | Input values used during execution |
| Test Steps | Ordered execution instructions |
| Expected Result | Expected application behavior |
| Actual Result | Observed behavior |
| Execution Status | Final test outcome |
| Evidence | Screenshot or supporting artifact |
| Defect Reference | Related bug ID, when applicable |

## 5. Requirements Traceability Matrix

| Requirement ID | Functional Requirement | Related Test Cases |
|---|---|---|
| REQ-001 | User authentication | TC-001 to TC-005 |
| REQ-002 | Product inventory | TC-006 to TC-009 |
| REQ-003 | Shopping cart operations | TC-010 to TC-013 |
| REQ-004 | Checkout workflow | TC-014 to TC-018 |

## 6. Test Data

| Data Type | Example |
|---|---|
| Valid username | standard_user |
| Valid password | secret_sauce |
| Locked username | locked_out_user |
| Invalid username | invalid_user |
| Invalid password | invalid_password |
| Customer first name | Test |
| Customer last name | User |
| Postal code | 1900 |

All test data is intended for the public demo environment only.

## 7. Execution Summary

| Metric | Initial Value |
|---|---:|
| Total Test Cases | 18 |
| Passed | 0 |
| Failed | 0 |
| Blocked | 0 |
| Not Executed | 18 |

**Execution Status:** Pending.

Results must be updated only after actual test execution.

## 8. Execution Notes

- Test execution must follow the defined preconditions.
- Actual results must reflect observed application behavior.
- Failed cases must be linked to defect reports where applicable.
- Relevant evidence should be collected.
- Any change to the test environment must be documented.

---

**Author:** Mariana Camps  
**QA Engineering Portfolio**  
**Manual Testing | Functional Testing | Test Documentation**
