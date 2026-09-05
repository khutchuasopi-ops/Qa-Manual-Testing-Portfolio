# Test Execution Report

## 1. Test Execution Overview

**Project:** E-commerce Web Application
**Application Under Test:** Confidential E-commerce Web Application
**Testing Type:** Manual Testing
**Testing Approach:** Functional, UI, Negative, User Flow, Exploratory
**Role:** Junior Manual QA Tester

This document summarizes the manual test execution performed on the web application.

The testing focused on the main customer journeys and core e-commerce functionality, including authentication, product search, product selection, shopping cart, checkout, localization, and user interface behavior.

> **Confidentiality Note:** The application name, organization name, URL, and confidential business or user information are intentionally excluded from this portfolio.

---

## 2. Test Execution Status

| Status       | Description                                                              |
| ------------ | ------------------------------------------------------------------------ |
| PASS         | Actual result matched the expected result                                |
| FAIL         | Actual result differed from the expected result                          |
| BLOCKED      | Test execution could not be completed because of a blocker or dependency |
| NOT RECORDED | The exact historical execution result was not recorded                   |

---

## 3. Test Execution Results

| Test Case ID | Test Case Title                             | Result       | Actual Result                                                                         | Bug ID  |
| ------------ | ------------------------------------------- | ------------ | ------------------------------------------------------------------------------------- | ------- |
| TC-001       | Login with valid credentials                | PASS         | User successfully logged in with valid credentials.                                   | -       |
| TC-002       | Login with invalid username                 | FAIL         | Invalid email credentials were accepted and the user was redirected to the home page. | BUG-003 |
| TC-003       | Login with invalid password                 | PASS         | Login was rejected when an invalid password was entered.                              | -       |
| TC-004       | Login with empty username                   | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-005       | Login with empty password                   | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-006       | Login with both fields empty                | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-007       | Logout functionality                        | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-008       | Search for an existing product              | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-009       | Search with invalid keyword                 | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-010       | Search with empty field                     | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-011       | Search result relevance                     | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-012       | Search using partial product name           | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-013       | Navigate from search result to product page | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-014       | Product information display                 | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-015       | Select available product size               | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-016       | Select unavailable product size             | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-017       | Selected size retained in cart              | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-018       | Add product without required size           | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-019       | Product image and price display             | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-020       | Add product to cart                         | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-021       | Product information in cart                 | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-022       | Increase product quantity                   | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-023       | Decrease product quantity                   | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-024       | Cart total calculation                      | FAIL         | Cart total did not update correctly after changing the product quantity.              | BUG-002 |
| TC-025       | Remove product from cart                    | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-026       | Empty cart behavior                         | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-027       | Navigate from cart to checkout              | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-028       | Checkout with valid information             | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-029       | Checkout with missing required information  | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-030       | Checkout with invalid input                 | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-031       | Delivery information                        | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-032       | Payment method selection                    | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-033       | Order summary and total                     | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-034       | Successful order placement                  | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-035       | Change website language                     | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-036       | Content displayed in selected language      | FAIL         | Website content remained in English after another language was selected.              | BUG-001 |
| TC-037       | Language consistency across pages           | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-038       | Main navigation                             | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-039       | Visibility of major UI elements             | NOT RECORDED | Historical execution result was not recorded.                                         | -       |
| TC-040       | Interactive UI elements                     | NOT RECORDED | Historical execution result was not recorded.                                         | -       |

---

## 4. Execution Summary

| Metric           | Result |
| ---------------- | -----: |
| Total Test Cases |     40 |
| Passed           |      2 |
| Failed           |      3 |
| Blocked          |      0 |
| Not Recorded     |     35 |

### Recorded Results

* **TC-001:** PASS — Valid login
* **TC-002:** FAIL — Invalid email accepted
* **TC-003:** PASS — Invalid password rejected
* **TC-024:** FAIL — Cart total did not update correctly
* **TC-036:** FAIL — Localization content remained in English

---

## 5. Defect Tracking

| Bug ID  | Related Test Case | Defect                                                            |
| ------- | ----------------- | ----------------------------------------------------------------- |
| BUG-001 | TC-036            | Selected language was not applied consistently to website content |
| BUG-002 | TC-024            | Cart total did not update correctly after quantity change         |
| BUG-003 | TC-002            | Invalid email credentials were accepted during login              |

Detailed defect information is documented in the `Bug-Reports` directory.

---

## 6. Retesting

When a defect is fixed, the related test case should be executed again to verify the fix.

Example:

**TC-024**

`FAIL → BUG-002 → Fix → Retest → PASS`

The retest result should be based on the actual behavior observed after the fix.

---

## 7. Test Execution Notes

* Test results are based on manual testing observations.
* Confidential organization and user information is excluded.
* Real personal data and credentials are not included in the portfolio.
* Historical results that could not be reliably reconstructed are marked as `NOT RECORDED`.
* Failed test cases are linked to the corresponding Bug Report.
* Screenshots should only be included if they do not expose confidential information.
* This portfolio does not represent the official QA process or internal records of the application owner.

---

## 8. Conclusion

The manual testing activities covered the main functional areas of the e-commerce application.

During testing, defects related to authentication, shopping cart calculation, and localization were identified and documented.

The project demonstrates the following QA workflow:

**Test Design → Test Execution → Defect Identification → Bug Reporting → Retesting → Test Summary**

