
# Test Plan – SauceDemo E-commerce Application

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Testing Approach:** Manual Functional Testing  
**Application Under Test:** https://www.saucedemo.com/  
**Document Version:** 1.1  
**Status:** Planned

---

## 1. Introduction

This document defines the testing strategy, scope, resources, methodology and execution criteria for the Quality Assurance assessment of the SauceDemo e-commerce application.

The objective is to evaluate critical user workflows, identify functional inconsistencies, assess application behavior and document findings through a structured QA process.

## 2. Testing Objectives

- Validate core business workflows.
- Verify authentication and authorization behavior at the application level.
- Assess product inventory and sorting functionality.
- Validate shopping cart operations.
- Verify checkout workflows and input validation.
- Identify functional, usability and consistency issues.
- Assess error handling and user feedback.
- Maintain traceability between requirements, test cases and defects.
- Provide an objective assessment of application quality.

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

The project follows a risk-based manual testing approach.

Testing activities will prioritize critical user journeys and functionality that directly impacts the shopping experience.

### Testing Types

| Testing Type | Purpose |
|---|---|
| Functional Testing | Verify expected application behavior |
| Positive Testing | Validate successful user interactions |
| Negative Testing | Evaluate invalid inputs and error handling |
| Boundary Value Analysis | Assess input limits and edge conditions |
| Exploratory Testing | Identify unexpected behavior |
| Regression Testing | Verify existing functionality after changes |
| Usability Testing | Assess navigation and user experience |

## 5. Risk Assessment

| Risk | Impact | Mitigation |
|---|---|---|
| Application availability issues | High | Record environment interruptions |
| Demo environment changes | Medium | Document execution date and conditions |
| Inconsistent application behavior | High | Repeat tests and preserve evidence |
| Limited backend access | Medium | Restrict conclusions to observable behavior |
| Incomplete test coverage | High | Maintain test case traceability |

## 6. Test Environment

| Component | Configuration |
|---|---|
| Application | SauceDemo |
| Environment | Public demo |
| Operating System | Windows |
| Browser | Google Chrome |
| Testing Approach | Manual |
| Documentation | Markdown |
| Version Control | GitHub |

Exact browser and operating system versions will be recorded during test execution.

## 7. Test Data Management

Test data will use publicly provided demo accounts and non-sensitive sample information.

Credentials will be documented separately from production or personal credentials.

Test data must not contain real personal or financial information.

## 8. Entry Criteria

Testing may begin when:

- The application is accessible.
- The testing environment is available.
- Test scenarios have been reviewed.
- Valid test credentials are available.
- Expected results have been defined.

## 9. Exit Criteria

Testing may be considered complete when:

- Planned test cases have been executed or formally marked as blocked.
- Actual results have been documented.
- Identified defects have been recorded.
- Critical findings have been reviewed.
- Relevant evidence has been collected.
- A final QA report has been prepared.

## 10. Defect Management

All identified defects must include:

- Unique defect ID.
- Summary and description.
- Preconditions.
- Steps to reproduce.
- Expected result.
- Actual result.
- Severity.
- Priority.
- Execution environment.
- Supporting evidence.

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

## 11. Test Execution Management

Each test case will be assigned an execution status:

- NOT EXECUTED
- PASSED
- FAILED
- BLOCKED
- NOT APPLICABLE

Failed test cases must be linked to their corresponding defect reports whenever applicable.

Execution evidence will be stored in the repository.

## 12. Suspension and Resumption Criteria

Testing may be suspended when:

- The application becomes unavailable.
- A critical issue prevents further execution.
- The testing environment becomes unreliable.
- Test data is no longer valid.

Testing may resume once the blocking condition has been resolved and the environment has been validated.

## 13. Deliverables

- Test Strategy and Test Plan.
- Test Case Documentation.
- Test Execution Results.
- Defect Reports.
- API Testing Collection.
- SQL Validation Scripts.
- Evidence and Supporting Documentation.
- Final QA Assessment Report.

## 14. Limitations

- Testing is limited to the publicly accessible demo environment.
- No access to application source code or backend infrastructure is assumed.
- Results represent the observed behavior during the documented execution period.
- Findings must not be generalized to production environments.

## 15. Approval and Document Status

**Document Status:** Planned – Pending Test Execution.

**Author:** Mariana Camps  
**Professional Focus:** Manual QA | API Testing | Software Quality

