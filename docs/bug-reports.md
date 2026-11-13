
# Bug Reports & Defect Management

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Application:** SauceDemo  
**Document Version:** 1.0

---

## 1. Purpose

This document defines the defect reporting and tracking approach used throughout the QA testing process.

The objective is to ensure that identified issues are documented consistently, are reproducible, and provide sufficient information for investigation and resolution.

## 2. Bug Report Template

| Field | Description |
|---|---|
| Bug ID | Unique defect identifier |
| Summary | Concise description of the issue |
| Module | Affected application component |
| Environment | Browser, OS and application version |
| Preconditions | Required initial state |
| Steps to Reproduce | Detailed reproduction instructions |
| Expected Result | Expected application behavior |
| Actual Result | Observed application behavior |
| Severity | Impact of the defect |
| Priority | Urgency of resolution |
| Status | Current defect lifecycle state |
| Evidence | Screenshots, logs or recordings |

## 3. Severity Classification

| Severity | Description |
|---|---|
| Critical | Major system failure or critical workflow unavailable |
| High | Core functionality significantly affected |
| Medium | Functional issue with a possible workaround |
| Low | Minor visual or usability issue |

## 4. Priority Classification

| Priority | Description |
|---|---|
| P1 – Critical | Requires immediate attention |
| P2 – High | Should be addressed urgently |
| P3 – Medium | Should be scheduled for resolution |
| P4 – Low | Minor improvement or cosmetic correction |

Severity measures impact, while priority determines how urgently the issue should be addressed.

## 5. Defect Lifecycle

Typical defect lifecycle:

1. New
2. Assigned
3. In Progress
4. Fixed
5. Ready for Retest
6. Verified
7. Closed

Alternative outcomes:
- Reopened
- Rejected
- Duplicate
- Cannot Reproduce
- Deferred

## 6. Defect Reporting Standards

Every defect report should:

- Have a clear and specific title.
- Describe one issue per report.
- Include reproducible steps.
- Separate expected and actual results.
- Include relevant environment details.
- Use severity and priority consistently.
- Include evidence whenever possible.
- Avoid assumptions about the technical root cause.

## 7. Illustrative Defect Examples

The following examples are hypothetical and are included only to demonstrate defect documentation structure.

### Example BUG-DEMO-001

**Summary:** Product price is displayed incorrectly in the cart.

**Module:** Shopping Cart

**Severity:** Medium  
**Priority:** P2 – High

**Preconditions:**
- User is authenticated.
- Inventory page is accessible.

**Steps to Reproduce:**
1. Open the inventory page.
2. Select a product.
3. Add the product to the cart.
4. Open the shopping cart.
5. Compare the displayed price with the inventory price.

**Expected Result:**

The product price should remain consistent between inventory and cart.

**Actual Result:**

Hypothetical scenario: the cart displays a different price.

**Status:** Illustrative – Not a verified application defect.

### Example BUG-DEMO-002

**Summary:** Checkout form does not provide clear validation feedback.

**Module:** Checkout

**Severity:** Low  
**Priority:** P3 – Medium

**Preconditions:**
- User has at least one product in the cart.
- Checkout information page is accessible.

**Steps to Reproduce:**
1. Open the checkout information page.
2. Leave a required field empty.
3. Submit the form.

**Expected Result:**

The application should clearly identify the missing required information.

**Actual Result:**

Hypothetical scenario: validation feedback is unclear.

**Status:** Illustrative – Not a verified application defect.

## 8. Defect Metrics

The following metrics may be used after actual test execution:

- Total defects identified.
- Defects by severity.
- Defects by priority.
- Open versus closed defects.
- Reopened defect rate.
- Defect distribution by functional module.

No actual defect metrics are reported until verified findings are available.

## 9. Traceability

Each confirmed defect should reference:

- Related test case ID.
- Affected functional requirement.
- Execution evidence.
- Retest result.

## 10. Conclusion

A consistent defect management process improves communication between QA and development teams, supports prioritization, and provides traceability throughout the software testing lifecycle.

---

**Author:** Mariana Camps  
**QA Engineering Portfolio**
