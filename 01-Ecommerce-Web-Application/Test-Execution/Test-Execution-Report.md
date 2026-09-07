# Test Execution Report

## 1. Project Information

| Field         | Details                    |
| ------------- | -------------------------- |
| Project       | E-commerce Web Application |
| Testing Type  | Manual Testing             |
| Testing Role  | Junior Manual QA Tester    |
| Application   | Confidential               |
| Execution Set | Historical Test Execution  |

---

## 2. Purpose

This document records the available historical test execution results for the documented test cases.

The report is intended to show which results were available and which historical results were not preserved.

Missing results are marked as **NOT RECORDED** and have not been recreated.

---

## 3. Result Definitions

| Status       | Meaning                                                        |
| ------------ | -------------------------------------------------------------- |
| PASS         | Actual result matched the expected result                      |
| FAIL         | Actual result did not match the expected result                |
| BLOCKED      | Test could not be completed because of a blocker or dependency |
| NOT RECORDED | Historical execution result was not available                  |

---

## 4. Execution Summary

| Result           | Count |
| ---------------- | ----: |
| Total Test Cases |    40 |
| PASS             |     2 |
| FAIL             |     3 |
| BLOCKED          |     0 |
| NOT RECORDED     |    35 |

---

# 5. Test Execution Results

| Test Case | Status       | Actual Result / Notes                                                   |
| --------- | ------------ | ----------------------------------------------------------------------- |
| TC-001    | PASS         | Valid login completed successfully                                      |
| TC-002    | FAIL         | Invalid email was accepted and the user was redirected to the home page |
| TC-003    | PASS         | Invalid password was rejected                                           |
| TC-004    | NOT RECORDED | Historical result not available                                         |
| TC-005    | NOT RECORDED | Historical result not available                                         |
| TC-006    | NOT RECORDED | Historical result not available                                         |
| TC-007    | NOT RECORDED | Historical result not available                                         |
| TC-008    | NOT RECORDED | Historical result not available                                         |
| TC-009    | NOT RECORDED | Historical result not available                                         |
| TC-010    | NOT RECORDED | Historical result not available                                         |
| TC-011    | NOT RECORDED | Historical result not available                                         |
| TC-012    | NOT RECORDED | Historical result not available                                         |
| TC-013    | NOT RECORDED | Historical result not available                                         |
| TC-014    | NOT RECORDED | Historical result not available                                         |
| TC-015    | NOT RECORDED | Historical result not available                                         |
| TC-016    | NOT RECORDED | Historical result not available                                         |
| TC-017    | NOT RECORDED | Historical result not available                                         |
| TC-018    | NOT RECORDED | Historical result not available                                         |
| TC-019    | NOT RECORDED | Historical result not available                                         |
| TC-020    | NOT RECORDED | Historical result not available                                         |
| TC-021    | NOT RECORDED | Historical result not available                                         |
| TC-022    | NOT RECORDED | Historical result not available                                         |
| TC-023    | NOT RECORDED | Historical result not available                                         |
| TC-024    | FAIL         | Cart total did not update correctly after quantity was changed          |
| TC-025    | NOT RECORDED | Historical result not available                                         |
| TC-026    | NOT RECORDED | Historical result not available                                         |
| TC-027    | NOT RECORDED | Historical result not available                                         |
| TC-028    | NOT RECORDED | Historical result not available                                         |
| TC-029    | NOT RECORDED | Historical result not available                                         |
| TC-030    | NOT RECORDED | Historical result not available                                         |
| TC-031    | NOT RECORDED | Historical result not available                                         |
| TC-032    | NOT RECORDED | Historical result not available                                         |
| TC-033    | NOT RECORDED | Historical result not available                                         |
| TC-034    | NOT RECORDED | Historical result not available                                         |
| TC-035    | NOT RECORDED | Historical result not available                                         |
| TC-036    | FAIL         | Website content remained in English after another language was selected |
| TC-037    | NOT RECORDED | Historical result not available                                         |
| TC-038    | NOT RECORDED | Historical result not available                                         |
| TC-039    | NOT RECORDED | Historical result not available                                         |
| TC-040    | NOT RECORDED | Historical result not available                                         |

---

# 6. Failed Test Cases

## TC-002 — Invalid Email Login

**Status:** FAIL

**Actual Result:**
An invalid email was accepted and the user was redirected to the home page.

**Related Defect:** BUG-003

---

## TC-024 — Cart Total After Quantity Change

**Status:** FAIL

**Actual Result:**
The cart total did not update correctly after changing the product quantity.

**Related Defect:** BUG-002

---

## TC-036 — Language Content

**Status:** FAIL

**Actual Result:**
The website content remained in English after another language was selected.

**Related Defect:** BUG-001

---

# 7. Passed Test Cases

## TC-001 — Valid Login

**Status:** PASS

**Actual Result:**
Valid login completed successfully.

---

## TC-003 — Invalid Password

**Status:** PASS

**Actual Result:**
Invalid password was rejected.

---

# 8. Defect Tracking

| Bug ID  | Related Test Case | Area                   | Severity | Priority | Status   |
| ------- | ----------------- | ---------------------- | -------- | -------- | -------- |
| BUG-001 | TC-036            | Localization           | Medium   | Medium   | Reported |
| BUG-002 | TC-024            | Shopping Cart          | High     | High     | Reported |
| BUG-003 | TC-002            | Login / Authentication | Medium   | High     | Open     |

---

# 9. Test Case to Defect Traceability

### BUG-001

* Test Case: TC-036
* Area: Localization
* Issue: Website content remained in English after language selection

### BUG-002

* Test Case: TC-024
* Area: Shopping Cart
* Issue: Cart total did not update correctly after quantity change

### BUG-003

* Test Case: TC-002
* Area: Login / Authentication
* Issue: Invalid email was accepted during login

---

# 10. Retesting Example

A retesting workflow can be used after a defect is reported as fixed:

**Failed Test Case → Bug Report → Fix → Retest → New Result**

For example:

**TC-024 → BUG-002 → Fix → Retest**

The final retest result should only be recorded when the retest has actually been performed.

---

# 11. Execution Notes

* The report contains historical execution information available for this project.
* Missing historical results are marked as **NOT RECORDED**.
* No missing results were recreated or assumed.
* Failed test cases are connected to the relevant bug reports.
* The test case library contains 40 documented test cases.
* The project also contains 34 documented test scenarios.
* Test scenarios and test cases represent documented coverage and should not be interpreted as proof that every item was executed.
* Confidential application information has been excluded from this portfolio.

---

# 12. Confidentiality

The application and test environment used for this project are confidential.

The following information has intentionally been excluded:

* Application name
* Application URL
* Real credentials
* Confidential business information
* Confidential user information
* Sensitive screenshots or test data

---

# 13. Final Result

Based on the available historical execution results:

* **2 test cases passed**
* **3 test cases failed**
* **0 test cases were blocked**
* **35 test cases have no recorded historical result**
* **3 defects were documented**

This report reflects the available testing information and does not claim additional execution results that were not recorded.
