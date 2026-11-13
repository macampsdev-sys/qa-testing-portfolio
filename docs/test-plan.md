# Test Plan – SauceDemo E-commerce Application

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Testing Approach:** Manual Functional Testing  
**Application Under Test:** https://www.saucedemo.com/  
**Document Version:** 1.2  
**Status:** Portfolio Demonstration

---

## 1. Introduction

This document defines the testing strategy, scope, methodology, risks, and quality assessment criteria for a demonstration-based QA project focused on the SauceDemo e-commerce application.

The objective is to showcase structured test planning, risk-based analysis, functional test design, and defect management practices through a realistic e-commerce application scenario.

## 2. Testing Objectives

- Define a structured approach to functional testing.
- Identify critical business workflows.
- Design positive and negative test scenarios.
- Assess authentication and application-level access behavior.
- Define validation criteria for product inventory and sorting functionality.
- Design test scenarios for shopping cart operations.
- Define checkout workflow and input validation scenarios.
- Identify potential functional, usability, and consistency issues.
- Establish requirements traceability.
- Define defect classification and reporting standards.

## 3. Scope

### 3.1 In Scope

| Module | Testing Coverage | Priority |
|---|---|---|
| Authentication | Login, invalid credentials, locked users | High |
| Inventory | Product information, sorting and display | High |
| Shopping Cart | Add, remove and item consistency | High |
| Checkout | Input validation and purchase workflow | High |
| Order Summary | Item details, quantities and totals | High |
| Navigation | Page transitions and application usability | Medium |

### 3.2 Out of Scope

- Backend source code validation.
- Database-level integrity testing.
- Load and stress testing.
- Real payment processing.
- Production security penetration testing.
- Third-party payment integrations.

## 4. Testing Strategy

The proposed testing strategy follows a risk-based manual testing approach.

Test design prioritizes critical user journeys and functionality that directly impacts the shopping experience.

### Testing Types

| Testing Type | Purpose |
|---|---|
| Functional Testing | Define checks for expected application behavior |
| Positive Testing | Cover successful user interactions |
| Negative Testing | Address invalid inputs and error handling |
| Boundary Value Analysis | Identify input limits and edge conditions |
| Exploratory Testing | Explore potential unexpected behavior |
| Regression Testing | Define critical functionality for future regression checks |
| Usability Testing | Assess navigation and user experience criteria |

## 5. Risk Assessment

| Risk | Impact | Mitigation |
|---|---|---|
| Application availability issues | High | Consider environment availability as a project constraint |
| Demo environment changes | Medium | Reference the public demo environment and its limitations |
| Inconsistent application behavior | High | Define clear expected results and defect reporting criteria |
| Limited backend access | Medium | Restrict the testing scope to observable application behavior |
| Incomplete test coverage | High | Use requirements traceability and risk-based test design |

## 6. Test Environment

| Component | Configuration |
|---|---|
| Application | SauceDemo |
| Environment | Public demo |
| Operating System | Windows |
| Browser | Google Chrome |
| Testing Approach | Manual test design |
| Documentation | Markdown |
| Version Control | GitHub |

The environment configuration represents the intended context for the demonstration scenarios and does not constitute a record of test execution.

## 7. Test Data Management

Test scenarios use publicly provided demo accounts and non-sensitive sample information.

Credentials are treated as test data and must not be confused with production or personal credentials.

Test data examples must not contain real personal or financial information.

## 8. Test Design Criteria

Test scenarios are designed considering:

- Business-critical user journeys.
- Positive and negative input conditions.
- Equivalence partitioning.
- Boundary value analysis.
- Expected application behavior.
- Requirements traceability.
- Risk and business impact.

Each test case should include a unique identifier, objective, preconditions, test steps, expected result, priority, and associated requirement.

## 9. Requirements Traceability

Requirements and test scenarios are organized to establish traceability between application functionality and the corresponding test cases.

The traceability matrix supports:

- Identification of covered functional requirements.
- Detection of potential coverage gaps.
- Organization of test scenarios by application module.
- Association between requirements and potential defects.

## 10. Defect Management

Potential defects identified through the demonstration scenarios are documented using a structured reporting approach.

Each defect report should include:

- Unique defect ID.
- Summary and description.
- Preconditions.
- Steps to reproduce.
- Expected result.
- Actual result, when verified.
- Severity.
- Priority.
- Environment details.
- Supporting evidence, when available.

### Severity Classification

| Severity | Definition |
|---|---|
| Critical | Causes a critical workflow failure or major system impact |
| High | Significantly affects core functionality |
| Medium | Causes functional issues with a possible workaround |
| Low | Minor visual, usability or cosmetic issue |

### Priority Classification

| Priority | Definition |
|---|---|
| P1 – Critical | Requires immediate attention |
| P2 – High | Should be addressed in the next development cycle |
| P3 – Medium | Should be addressed when resources allow |
| P4 – Low | Minor improvement or cosmetic correction |

Severity measures impact. Priority determines urgency.

Illustrative defect examples are identified as portfolio examples and are not presented as verified application findings.

## 11. Test Case Documentation

Test cases are organized using the following status values:

- NOT EXECUTED
- PASSED
- FAILED
- BLOCKED
- NOT APPLICABLE

These values define the available test case status model. This portfolio demonstrates test design and documentation rather than executed test results.

## 12. Quality Assessment Criteria

The proposed quality assessment considers:

- Coverage of critical application workflows.
- Clarity and completeness of test scenarios.
- Traceability between requirements and test cases.
- Consistency of expected results.
- Defect reporting structure.
- Identification of testing limitations and risks.

The assessment framework provides a basis for evaluating the quality of the test design documentation.

## 13. Project Deliverables

- Test Plan and Testing Strategy.
- Functional Test Case Documentation.
- Requirements Traceability Matrix.
- Defect Reporting Templates and Illustrative Examples.
- QA Quality Assessment Framework.
- API Testing Collection and Configuration.
- Supporting Technical Documentation.

## 14. Limitations

- The project uses a publicly accessible demo application.
- No access to application source code or backend infrastructure is assumed.
- Test scenarios and defect examples are intended for portfolio demonstration.
- No executed test results or verified application defects are claimed.
- Findings from a demo environment must not be generalized to production environments.

## 15. Document Status

**Document Status:** Completed – Portfolio Demonstration.

**Author:** Mariana Camps  
**Professional Focus:** Manual QA | API Testing | Software Quality
