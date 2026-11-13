# Bug Reports & Defect Management

**Project:** QA Engineering Portfolio  
**Author:** Mariana Camps  
**Application:** SauceDemo  
**Document Version:** 1.1  
**Document Status:** Portfolio Demonstration

---

## 1. Purpose

This document defines the defect reporting standards and management methodology demonstrated throughout this QA portfolio.

The objective is to establish a consistent approach to documenting potential software defects, supporting reproducibility, clear communication, prioritization, and traceability.

## 2. Bug Report Template

The following template defines the standard information required for structured defect documentation.

| Field | Description |
|---|---|
| Bug ID | Unique defect identifier |
| Summary | Concise description of the issue |
| Module | Affected application component |
| Environment | Browser, OS and application version |
| Preconditions | Required initial state |
| Steps to Reproduce | Detailed reproduction instructions |
| Expected Result | Expected application behavior |
| Actual Result | Observed behavior, when verified |
| Severity | Impact of the defect |
| Priority | Urgency of resolution |
| Status | Current defect lifecycle state |
| Evidence | Supporting screenshots, logs or recordings |

## 3. Severity Classification

Severity represents the impact a defect may have on application functionality and user experience.

| Severity | Description |
|---|---|
| Critical | Major system failure or critical workflow unavailable |
| High | Core functionality significantly affected |
| Medium | Functional issue with a possible workaround |
| Low | Minor visual or usability issue |

## 4. Priority Classification

Priority determines the urgency with which a defect should be addressed.

| Priority | Description |
|---|---|
| P1 – Critical | Requires immediate attention |
| P2 – High | Should be addressed urgently |
| P3 – Medium | Should be scheduled for resolution |
| P4 – Low | Minor improvement or cosmetic correction |

Severity measures impact, while priority determines how urgently the issue should be addressed.

## 5. Defect Lifecycle

The following lifecycle represents a typical defect management workflow:

1. New
2. Assigned
3. In Progress
4. Fixed
5. Ready for Retest
6. Verified
7. Closed

Alternative outcomes include:

- Reopened
- Rejected
- Duplicate
- Cannot Reproduce
- Deferred

The lifecycle may vary according to the team's workflow and defect management tool.

## 6. Defect Reporting Standards

A structured defect report should:

- Have a clear and specific title.
- Describe one issue per report.
- Include reproducible steps.
- Separate expected and actual results.
- Include relevant environment details.
- Apply severity and priority consistently.
- Include supporting evidence when available.
- Avoid assumptions about the technical root cause.

## 7. Illustrative Defect Examples

The following examples are hypothetical and demonstrate how potential defects can be documented.

They are not verified findings from an actual application test execution.

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

**Illustrative Actual Result:**

The cart displays a different price from the inventory.

**Status:** Hypothetical example – Not a verified application defect.

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

**Illustrative Actual Result:**

Validation feedback is unclear.

**Status:** Hypothetical example – Not a verified application defect.

## 8. Defect Metrics

The following metrics are commonly used to assess defect trends and quality:

- Total defects identified.
- Defects by severity.
- Defects by priority.
- Open versus closed defects.
- Reopened defect rate.
- Defect distribution by functional module.

These metrics require verified defect records and are presented here as quality management concepts, not actual project results.

## 9. Traceability

A confirmed defect should be linked to relevant testing documentation whenever applicable:

- Related test case ID.
- Affected functional requirement.
- Supporting evidence.
- Retest result, when available.

Traceability supports impact analysis, defect investigation, and quality reporting.

## 10. Conclusion

A consistent defect management process improves communication between QA and development teams, supports prioritization, and provides traceability throughout the software quality lifecycle.

This document demonstrates defect reporting practices, classification criteria, and lifecycle management through illustrative examples.

---

**Author:** Mariana Camps  
**QA Engineering Portfolio**  
**Manual Testing | Defect Management | Software Quality**
