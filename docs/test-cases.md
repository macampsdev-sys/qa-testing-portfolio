# Test Cases & Requirements Traceability Matrix – SauceDemo

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Application:** https://www.saucedemo.com/  
**Document Version:** 1.1  
**Testing Type:** Manual Functional Testing  
**Document Status:** Designed – Not Executed

---

## 1. Test Coverage Overview

This document defines the functional test scenarios designed to assess the main user journeys of the SauceDemo e-commerce application.

Test cases are organized by functional module and prioritized according to business impact and risk.

The scenarios demonstrate structured test design, expected result definition, and requirements traceability.

## 2. Test Case Status Definitions

The following status values define the classification model available for test case management:

| Status | Description |
|---|---|
| NOT EXECUTED | Test case has been designed but not executed |
| PASSED | Actual result matches expected result |
| FAILED | Actual result differs from expected result |
| BLOCKED | Execution cannot continue due to a blocking condition |
| NOT APPLICABLE | Test case is outside the applicable scope |

All test cases in this portfolio are presented as designed scenarios and do not represent executed test results.

## 3. Test Cases

### Module A – Authentication

| ID | Scenario | Priority | Preconditions | Expected Result |
|---|---|---|---|---|
| TC-001 | Login with valid credentials | P1 | Login page accessible | User is redirected to inventory |
| TC-002 | Login with invalid username | P1 | Login page accessible | Authentication error is displayed |
| TC-003 | Login with invalid password | P1 | Login page accessible | Authentication error is displayed |
| TC-004 | Login with empty credentials | P2 | Login page accessible | Input validation error is displayed |
| TC-005 | Login with locked account | P1 | Login page accessible | Access is denied with an appropriate message |

### Module B – Product Inventory

| ID | Scenario | Priority | Preconditions | Expected Result |
|---|---|---|---|---|
| TC-006 | Verify inventory loading | P1 | Standard user authenticated | Inventory page loads successfully |
| TC-007 | Validate product information | P2 | Inventory page accessible | Product names, prices and images are displayed |
| TC-008 | Sort products alphabetically | P2 | Inventory page accessible | Products are sorted A–Z |
| TC-009 | Sort products by ascending price | P2 | Inventory page accessible | Products are sorted from lowest to highest price |

### Module C – Shopping Cart

| ID | Scenario | Priority | Preconditions | Expected Result |
|---|---|---|---|---|
| TC-010 | Add one product to cart | P1 | Inventory page accessible | Cart counter reflects one item |
| TC-011 | Add multiple products | P1 | Inventory page accessible | Cart counter reflects selected quantity |
| TC-012 | Remove product from inventory | P2 | Product previously added | Product is removed from cart |
| TC-013 | Verify cart contents | P1 | At least one product added | Selected products appear in cart |

### Module D – Checkout

| ID | Scenario | Priority | Preconditions | Expected Result |
|---|---|---|---|---|
| TC-014 | Start checkout process | P1 | Cart contains a product | Checkout information page opens |
| TC-015 | Submit empty checkout information | P1 | Checkout information page accessible | Required field validation is displayed |
| TC-016 | Submit incomplete customer information | P2 | Checkout information page accessible | Missing required information is identified |
| TC-017 | Complete purchase workflow | P1 | Valid customer information available | Order confirmation is displayed |
| TC-018 | Verify order summary | P1 | Checkout overview accessible | Products, quantities and totals are displayed correctly |

## 4. Detailed Test Case Specification

The following fields define the standard structure used to document each test case:

| Field | Description |
|---|---|
| Test Case ID | Unique test identifier |
| Preconditions | Required initial application state |
| Test Data | Input values used in the scenario |
| Test Steps | Ordered instructions describing the scenario |
| Expected Result | Expected application behavior |
| Actual Result | Observed behavior, when applicable |
| Execution Status | Test outcome, when applicable |
| Evidence | Supporting artifact, when available |
| Defect Reference | Related defect ID, when applicable |

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

## 7. Test Design Summary

| Metric | Value |
|---|---:|
| Total Test Cases Designed | 18 |
| Functional Modules Covered | 4 |
| Requirements Documented | 4 |
| Priority Levels Defined | P1, P2 |

The summary represents test design coverage, not execution results.

## 8. Test Design Considerations

- Test scenarios cover the main functional workflows.
- Preconditions define the initial context for each scenario.
- Expected results describe the intended application behavior.
- Priorities reflect functional importance and business impact.
- Requirements traceability supports coverage analysis.
- Illustrative scenarios are not presented as verified application findings.

---

**Author:** Mariana Camps  
**QA Engineering Portfolio**  
**Manual Testing | Functional Testing | Test Design | Requirements Traceability**
