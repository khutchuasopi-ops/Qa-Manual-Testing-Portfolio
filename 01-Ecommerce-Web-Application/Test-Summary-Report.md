# Test Summary Report

## 1. Project Information

| Field                 | Details                                                  |
| --------------------- | -------------------------------------------------------- |
| Project               | E-commerce Web Application                               |
| Testing Type          | Manual Software Testing                                  |
| QA Role               | Junior Manual QA Tester                                  |
| Test Approach         | Functional, UI, Positive, Negative, Boundary, Regression |
| Execution Environment | Web Browser                                              |
| Test Suite            | 60 Test Cases                                            |
| Defects Identified    | 3                                                        |

---

# 2. Testing Objective

The objective of this testing activity was to evaluate the core functionality and usability of an e-commerce web application.

Testing focused on the main customer journey:

```text
Login
  ↓
Product Search
  ↓
Product Selection
  ↓
Size / Quantity Selection
  ↓
Shopping Cart
  ↓
Checkout
  ↓
Order Completion
```

Additional attention was given to localization, input validation, session behavior, UI, and cart price calculations.

---

# 3. Test Scope

## In Scope

* User authentication
* Login validation
* Logout functionality
* Session behavior
* Product search
* Product details
* Product size selection
* Product quantity
* Shopping cart
* Cart calculations
* Cart state
* Checkout
* Checkout validation
* Delivery information
* Payment method selection
* Order summary
* Localization
* UI and navigation
* Negative and boundary scenarios

## Out of Scope

The following areas were not included in the manual test execution:

* Performance testing
* Load testing
* Stress testing
* Automated testing
* Source code review
* Database testing
* Full security penetration testing
* Production monitoring
* Infrastructure testing

---

# 4. Test Execution Summary

| Status           |  Count |
| ---------------- | -----: |
| Total Test Cases | **60** |
| Passed           |  **2** |
| Failed           |  **3** |
| Blocked          |  **0** |
| Not Recorded     | **35** |
| Not Executed     | **20** |

### Recorded Execution Coverage

The historical execution contains reliable results for **5 of the original 40 test cases**.

**Recorded execution rate: 12.5%**

The remaining historical cases are marked `NOT RECORDED`.

The additional 20 test cases added during the test suite expansion are marked `NOT EXECUTED`.

> No test result has been fabricated to increase the apparent test coverage or pass rate.

---

# 5. Passed Test Cases

## TC-001 — Login with Valid Credentials

**Result:** PASS

The application successfully authenticated the user when valid credentials were provided.

---

## TC-003 — Login with Invalid Password

**Result:** PASS

The application rejected the login attempt when an invalid password was provided.

---

# 6. Failed Test Cases

## TC-002 — Login with Invalid Email

**Result:** FAIL

### Expected

Invalid email credentials should be rejected and the user should remain unauthenticated.

### Actual

The invalid email credentials were accepted and the user was redirected to the home page.

### Related Defect

**BUG-003 — Invalid Email Accepted During Login**

**Severity:** Medium
**Priority:** High
**Status:** Open

---

## TC-024 — Cart Total Calculation

**Result:** FAIL

### Expected

The cart total should be recalculated whenever the product quantity changes.

### Actual

The cart total did not update correctly after the product quantity was changed.

### Related Defect

**BUG-002 — Cart Total Price Does Not Change When Product Quantity Is Updated**

**Severity:** High
**Priority:** High
**Status:** Reported

---

## TC-036 — Selected Language Content

**Result:** FAIL

### Expected

Application content should be displayed in the language selected by the user.

### Actual

The website content remained in English after another language was selected.

### Related Defect

**BUG-001 — Website Content Remains in English After Changing Language**

**Severity:** Medium
**Priority:** Medium
**Status:** Reported

---

# 7. Defect Summary

| Bug ID  | Area           | Severity | Priority | Status   | Related Test Case |
| ------- | -------------- | -------- | -------- | -------- | ----------------- |
| BUG-001 | Localization   | Medium   | Medium   | Reported | TC-036            |
| BUG-002 | Shopping Cart  | High     | High     | Reported | TC-024            |
| BUG-003 | Authentication | Medium   | High     | Open     | TC-002            |

---

# 8. Defect Distribution by Area

| Area            | Defects |
| --------------- | ------: |
| Authentication  |       1 |
| Shopping Cart   |       1 |
| Localization    |       1 |
| Product Search  |       0 |
| Product Details |       0 |
| Checkout        |       0 |
| UI / Navigation |       0 |

### Observation

The currently recorded failures are distributed across three different functional areas.

The most business-critical recorded defect is the shopping cart calculation issue because incorrect pricing can directly affect the customer's purchase decision and order value.

---

# 9. Risk Assessment

## High Risk

### Shopping Cart Price Calculation

Incorrect cart totals represent a high business risk because pricing is a critical part of an e-commerce transaction.

**Related defect:** BUG-002

Recommended action:

* Fix calculation logic.
* Retest quantity changes.
* Test multiple products.
* Test minimum and maximum quantities.
* Verify cart-to-checkout total consistency.

---

## High Risk

### Authentication Validation

Accepting invalid email credentials can create unexpected authentication behavior and potentially expose an access-control weakness.

**Related defect:** BUG-003

Recommended action:

* Validate email format.
* Verify invalid credentials are rejected.
* Test malformed email values.
* Test protected pages after logout.
* Execute regression testing after the fix.

---

## Medium Risk

### Localization

Failure to display content in the selected language negatively affects usability and international users.

**Related defect:** BUG-001

Recommended action:

* Verify navigation labels.
* Verify buttons and UI text.
* Verify validation messages.
* Verify product information.
* Check for mixed-language content.

---

# 10. Regression Testing Recommendations

After defects are fixed, the following tests should be executed.

| Defect  | Retest | Regression Tests       |
| ------- | ------ | ---------------------- |
| BUG-001 | TC-036 | TC-059, TC-060         |
| BUG-002 | TC-024 | TC-052, TC-051, TC-058 |
| BUG-003 | TC-002 | TC-044, TC-042         |

The purpose of regression testing is to confirm that the defect fix works and that related functionality has not been negatively affected.

---

# 11. Test Coverage Improvements

The expanded test suite improves coverage in the following areas:

### Authentication

* Invalid credentials
* Empty fields
* Malformed email
* Whitespace handling
* Session persistence
* Protected-page access after logout

### Search

* Empty search
* Whitespace-only input
* Invalid keywords
* Partial product names
* Case sensitivity
* Special characters

### Shopping Cart

* Quantity boundaries
* Invalid quantities
* Multiple-product calculations
* Cart persistence
* Total recalculation

### Checkout

* Invalid email
* Invalid phone number
* Missing required information
* Duplicate submission
* Cart-to-checkout total consistency

### Localization

* Validation messages
* UI labels
* Product information
* Mixed-language content

---

# 12. Test Quality Assessment

The current test suite demonstrates a structured manual QA approach.

### Strengths

* Clear test case identification
* Positive and negative testing
* Functional testing of core user journeys
* Explicit expected results
* Defect traceability
* Separate bug reports
* Regression test planning
* Boundary and edge-case coverage
* Transparent reporting of unrecorded results

### Areas for Further Improvement

The next execution cycle should provide evidence for the currently unexecuted test cases.

Recommended improvements:

1. Execute the expanded test suite.
2. Record exact Actual Results.
3. Capture evidence for failed tests.
4. Link every failure to a Bug ID.
5. Perform retesting after fixes.
6. Perform regression testing around fixed defects.
7. Add browser and responsive execution evidence.
8. Update the final metrics after execution.

---

# 13. Release Readiness Assessment

Based on the currently recorded execution results, the application should **not be considered fully validated for release based solely on this test cycle**.

Reasons include:

* 3 recorded failures
* 20 newly added test cases not yet executed
* 35 historical test cases without reliable recorded results
* A High Severity cart calculation defect
* An open authentication-related defect
* A localization defect

This assessment is based on the available test evidence and does not represent an official production release decision.

---

# 14. QA Recommendation

### Current Recommendation: **Further Testing Required**

Before considering the application sufficiently validated, the following should be completed:

* Fix and retest BUG-001.
* Fix and retest BUG-002.
* Investigate and retest BUG-003.
* Execute all critical-path test cases.
* Execute checkout validation tests.
* Execute cart boundary tests.
* Execute session-related tests.
* Execute localization regression tests.
* Perform cross-browser/responsive checks where applicable.
* Update the final test metrics.

---

# 15. Final QA Summary

The manual testing activity identified functional issues in three important areas:

1. **Authentication**
2. **Shopping Cart**
3. **Localization**

The testing process demonstrates the following QA workflow:

```text
Requirement Analysis
        ↓
Test Scenario Design
        ↓
Test Case Design
        ↓
Manual Test Execution
        ↓
Defect Identification
        ↓
Bug Reporting
        ↓
Retesting
        ↓
Regression Testing
        ↓
Test Summary
```

The portfolio intentionally reports incomplete historical execution data rather than presenting assumed or fabricated results.

The expanded test suite provides a stronger foundation for a future execution cycle, with additional coverage for validation, boundaries, sessions, cart calculations, checkout, localization, and regression testing.

---

## Final Metrics

**Test Cases:** 60
**PASS:** 2
**FAIL:** 3
**BLOCKED:** 0
**NOT RECORDED:** 35
**NOT EXECUTED:** 20
**Defects Identified:** 3
**Current QA Recommendation:** **Further Testing Required**
