# Test Execution Report

## 1. Test Execution Overview

| Field                  | Details                                                                                      |
| ---------------------- | -------------------------------------------------------------------------------------------- |
| Project                | E-commerce Web Application                                                                   |
| Application Under Test | Confidential E-commerce Web Application                                                      |
| Testing Type           | Manual Testing                                                                               |
| Testing Approach       | Functional, UI, Negative, User Flow, Exploratory                                             |
| QA Role                | Junior Manual QA Tester                                                                      |
| Execution Scope        | Authentication, Product Search, Product Selection, Shopping Cart, Checkout, Localization, UI |

This document summarizes the manual test execution performed for the e-commerce web application.

Testing focused on the main customer journeys and core e-commerce functionality, including authentication, product search, product selection, shopping cart, checkout, localization, and user interface behavior.

> **Confidentiality Note:** The application name, organization name, URL, and confidential business or user information are intentionally excluded from this portfolio.

---

## 2. Test Execution Status

| Status           | Description                                                                  |
| ---------------- | ---------------------------------------------------------------------------- |
| **PASS**         | Actual result matched the expected result                                    |
| **FAIL**         | Actual result differed from the expected result                              |
| **BLOCKED**      | Test execution could not be completed because of a blocker or dependency     |
| **NOT RECORDED** | The historical execution result was not reliably recorded                    |
| **NOT EXECUTED** | The test case exists in the current test suite but has not yet been executed |

### Important distinction

`NOT RECORDED` and `NOT EXECUTED` are intentionally different.

* `NOT RECORDED` applies to historical test cases where an execution result cannot be reliably reconstructed.
* `NOT EXECUTED` applies to newly added test cases that have not yet been run.

No execution result is fabricated for portfolio purposes.

---

# 3. Test Execution Results

## 3.1 Authentication and Login

| Test Case ID | Test Case                              | Result       | Actual Result                                                                         | Bug     |
| ------------ | -------------------------------------- | ------------ | ------------------------------------------------------------------------------------- | ------- |
| TC-001       | Login with valid credentials           | **PASS**     | User successfully logged in with valid credentials.                                   | -       |
| TC-002       | Login with invalid username            | **FAIL**     | Invalid email credentials were accepted and the user was redirected to the home page. | BUG-003 |
| TC-003       | Login with invalid password            | **PASS**     | Login was rejected when an invalid password was entered.                              | -       |
| TC-004       | Login with empty username              | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-005       | Login with empty password              | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-006       | Login with both fields empty           | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-007       | Logout functionality                   | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-041       | Session persistence after page refresh | NOT EXECUTED | Test has not yet been executed.                                                       | -       |
| TC-042       | Access protected page after logout     | NOT EXECUTED | Test has not yet been executed.                                                       | -       |
| TC-043       | Login with leading/trailing spaces     | NOT EXECUTED | Test has not yet been executed.                                                       | -       |
| TC-044       | Login with malformed email             | NOT EXECUTED | Test has not yet been executed.                                                       | -       |

---

## 3.2 Product Search

| Test Case ID | Test Case                                   | Result       | Actual Result                                 | Bug |
| ------------ | ------------------------------------------- | ------------ | --------------------------------------------- | --- |
| TC-008       | Search for an existing product              | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-009       | Search with invalid keyword                 | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-010       | Search with empty field                     | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-011       | Search result relevance                     | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-012       | Search using partial product name           | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-013       | Navigate from search result to product page | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-045       | Search using whitespace only                | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-046       | Search case sensitivity                     | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-047       | Search using special characters             | NOT EXECUTED | Test has not yet been executed.               | -   |

---

## 3.3 Product Details and Selection

| Test Case ID | Test Case                         | Result       | Actual Result                                 | Bug |
| ------------ | --------------------------------- | ------------ | --------------------------------------------- | --- |
| TC-014       | Product information display       | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-015       | Select available product size     | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-016       | Select unavailable product size   | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-017       | Selected size retained in cart    | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-018       | Add product without required size | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-019       | Product image and price display   | NOT RECORDED | Historical execution result was not recorded. | -   |

---

## 3.4 Shopping Cart

| Test Case ID | Test Case                                      | Result       | Actual Result                                                            | Bug                |
| ------------ | ---------------------------------------------- | ------------ | ------------------------------------------------------------------------ | ------------------ |
| TC-020       | Add product to cart                            | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-021       | Product information in cart                    | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-022       | Increase product quantity                      | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-023       | Decrease product quantity                      | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-024       | Cart total calculation                         | **FAIL**     | Cart total did not update correctly after changing the product quantity. | BUG-002            |
| TC-025       | Remove product from cart                       | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-026       | Empty cart behavior                            | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-048       | Minimum allowed quantity                       | NOT EXECUTED | Test has not yet been executed.                                          | -                  |
| TC-049       | Maximum allowed quantity                       | NOT EXECUTED | Test has not yet been executed.                                          | -                  |
| TC-050       | Invalid quantity input                         | NOT EXECUTED | Test has not yet been executed.                                          | -                  |
| TC-051       | Total calculation for multiple products        | NOT EXECUTED | Test has not yet been executed.                                          | -                  |
| TC-052       | Cart total recalculation after quantity update | NOT EXECUTED | Test has not yet been executed.                                          | BUG-002 regression |
| TC-053       | Cart state after page refresh                  | NOT EXECUTED | Test has not yet been executed.                                          | -                  |

---

## 3.5 Checkout

| Test Case ID | Test Case                                            | Result       | Actual Result                                 | Bug |
| ------------ | ---------------------------------------------------- | ------------ | --------------------------------------------- | --- |
| TC-027       | Navigate from cart to checkout                       | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-028       | Checkout with valid information                      | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-029       | Checkout with missing required information           | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-030       | Checkout with invalid input                          | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-031       | Delivery information                                 | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-032       | Payment method selection                             | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-033       | Order summary and total                              | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-034       | Successful order placement                           | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-054       | Invalid checkout email                               | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-055       | Invalid checkout phone number                        | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-056       | Prevent order submission with incomplete information | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-057       | Prevent duplicate order submission                   | NOT EXECUTED | Test has not yet been executed.               | -   |
| TC-058       | Checkout total matches cart total                    | NOT EXECUTED | Test has not yet been executed.               | -   |

---

## 3.6 Localization

| Test Case ID | Test Case                              | Result       | Actual Result                                                            | Bug                |
| ------------ | -------------------------------------- | ------------ | ------------------------------------------------------------------------ | ------------------ |
| TC-035       | Change website language                | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-036       | Content displayed in selected language | **FAIL**     | Website content remained in English after another language was selected. | BUG-001            |
| TC-037       | Language consistency across pages      | NOT RECORDED | Historical execution result was not recorded.                            | -                  |
| TC-059       | Localization of validation messages    | NOT EXECUTED | Test has not yet been executed.                                          | BUG-001 regression |
| TC-060       | No mixed-language content              | NOT EXECUTED | Test has not yet been executed.                                          | BUG-001 regression |

---

## 3.7 UI and Navigation

| Test Case ID | Test Case                       | Result       | Actual Result                                 | Bug |
| ------------ | ------------------------------- | ------------ | --------------------------------------------- | --- |
| TC-038       | Main navigation                 | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-039       | Visibility of major UI elements | NOT RECORDED | Historical execution result was not recorded. | -   |
| TC-040       | Interactive UI elements         | NOT RECORDED | Historical execution result was not recorded. | -   |

---

# 4. Execution Summary

| Metric           | Result |
| ---------------- | -----: |
| Total Test Cases | **60** |
| Passed           |  **2** |
| Failed           |  **3** |
| Blocked          |  **0** |
| Not Recorded     | **35** |
| Not Executed     | **20** |

### Recorded Execution Rate

Historical execution results were available for **5 of 40 original test cases**.

**Recorded execution rate:** 12.5%

The remaining original historical results are intentionally marked as `NOT RECORDED`.

The additional TC-041–TC-060 test cases are part of the expanded test suite and are currently marked `NOT EXECUTED`.

> These metrics represent the current state of the portfolio documentation and should not be interpreted as complete application test coverage.

---

# 5. Recorded Results

The following execution results were historically recorded and are included without modification:

| Test Case | Result | Observation                                               |
| --------- | ------ | --------------------------------------------------------- |
| TC-001    | PASS   | Valid login completed successfully                        |
| TC-002    | FAIL   | Invalid email credentials were accepted                   |
| TC-003    | PASS   | Invalid password was rejected                             |
| TC-024    | FAIL   | Cart total did not update after quantity change           |
| TC-036    | FAIL   | Website content remained in English after language change |

---

# 6. Defect Tracking

| Bug ID  | Related Test Case | Severity | Priority | Status   | Defect                                                       |
| ------- | ----------------- | -------- | -------- | -------- | ------------------------------------------------------------ |
| BUG-001 | TC-036            | Medium   | Medium   | Reported | Website content remained in English after language selection |
| BUG-002 | TC-024            | High     | High     | Reported | Cart total did not update correctly after quantity change    |
| BUG-003 | TC-002            | Medium   | High     | Open     | Invalid email credentials were accepted during login         |

Detailed defect information is documented in the `Bug-Reports` directory.

---

# 7. Defect-to-Test Traceability

| Defect  | Detection Test | Related Area                | Regression Coverage |
| ------- | -------------- | --------------------------- | ------------------- |
| BUG-001 | TC-036         | Localization                | TC-059, TC-060      |
| BUG-002 | TC-024         | Shopping Cart / Calculation | TC-052              |
| BUG-003 | TC-002         | Authentication              | TC-044              |

This traceability provides a clear connection between:

**Test Case → Failed Result → Bug Report → Regression Test**

---

# 8. Retesting Strategy

When a defect is fixed, the original failed test case should be executed again.

The related regression test cases should also be executed to verify that the fix did not introduce new issues.

### BUG-001 — Localization

```text
TC-036 FAIL
      ↓
BUG-001
      ↓
Developer Fix
      ↓
TC-036 Retest
      ↓
TC-059 / TC-060 Regression
      ↓
PASS / FAIL
```

### BUG-002 — Cart Total

```text
TC-024 FAIL
      ↓
BUG-002
      ↓
Developer Fix
      ↓
TC-024 Retest
      ↓
TC-052 Regression
      ↓
PASS / FAIL
```

### BUG-003 — Invalid Email Authentication

```text
TC-002 FAIL
      ↓
BUG-003
      ↓
Developer Fix
      ↓
TC-002 Retest
      ↓
TC-044 Regression
      ↓
PASS / FAIL
```

> Retest results should only be marked `PASS` or `FAIL` after the application has actually been tested again.

---

# 9. Risk-Based Execution Priority

If a new execution cycle is performed, the recommended order is:

| Priority | Area                          | Reason                                    |
| -------- | ----------------------------- | ----------------------------------------- |
| P0       | Authentication                | Core access and account security behavior |
| P0       | Shopping Cart Calculation     | Direct impact on customer pricing         |
| P0       | Checkout                      | Critical revenue/customer journey         |
| P1       | Product Selection             | Core purchasing functionality             |
| P1       | Localization                  | User-facing functional consistency        |
| P1       | Search                        | Product discoverability                   |
| P2       | UI / Navigation               | Usability and navigation quality          |
| P2       | Responsive / Browser Coverage | Compatibility and user experience         |

---

# 10. Recommended Next Execution Cycle

The next manual execution cycle should prioritize:

1. Re-execute all currently failed test cases.
2. Execute the new critical cart and checkout cases.
3. Execute authentication/session edge cases.
4. Execute localization regression cases.
5. Record exact Actual Results.
6. Attach Bug IDs when failures are identified.
7. Update defect status after retesting.
8. Update the Test Summary Report after execution is complete.

Recommended critical test cases for the next cycle:

* TC-002 — Invalid email credentials
* TC-024 — Cart total calculation
* TC-036 — Selected language content
* TC-042 — Protected page after logout
* TC-050 — Invalid quantity input
* TC-052 — Cart total recalculation
* TC-056 — Incomplete checkout
* TC-058 — Checkout total vs cart total
* TC-059 — Localization validation messages
* TC-060 — Mixed-language content

---

# 11. Execution Notes

* Test results are based on manual testing observations.
* No historical result has been invented or inferred.
* Historical results that could not be reliably reconstructed are marked `NOT RECORDED`.
* Newly added test cases that have not yet been executed are marked `NOT EXECUTED`.
* Failed test cases are linked to the corresponding Bug Report.
* Regression test cases are explicitly linked to existing defects.
* Confidential organization, application, user, and business information is excluded.
* Real personal data and credentials are not included in the portfolio.
* Screenshots should only be included when they do not expose confidential information.
* This portfolio does not represent the official QA process or internal records of the application owner.

---

# 12. Conclusion

The current test execution documentation demonstrates a structured manual QA workflow covering the core e-commerce customer journey.

The recorded execution identified defects in:

* Authentication
* Shopping cart calculation
* Localization

The expanded test suite increases coverage in:

* Session management
* Input validation
* Boundary testing
* Cart state management
* Checkout validation
* Duplicate submission prevention
* Localization regression
* Defect traceability

The current execution status remains intentionally transparent:

**2 PASS · 3 FAIL · 0 BLOCKED · 35 NOT RECORDED · 20 NOT EXECUTED**

The next quality improvement step is to perform a fresh execution cycle for the expanded test suite and replace `NOT EXECUTED` with actual evidence-based results.

### QA Workflow

```text
Test Planning
     ↓
Test Scenario Design
     ↓
Test Case Design
     ↓
Test Execution
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
