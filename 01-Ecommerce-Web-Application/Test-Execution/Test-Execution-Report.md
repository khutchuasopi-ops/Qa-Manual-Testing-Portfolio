# Test Execution Report

## 1. Test Execution Overview

**Project:** E-commerce Web Application
**Testing Type:** Manual Testing
**Role:** Junior Manual QA Tester
**Execution Status:** Not Started

This document contains the execution results of the manual test cases defined for the E-commerce Web Application.

The purpose of test execution is to verify the actual behavior of the application against the expected results defined in the test cases.

---

## 2. Test Execution Status

| Status       | Description                                                |
| ------------ | ---------------------------------------------------------- |
| PASS         | Actual result matches the expected result                  |
| FAIL         | Actual result does not match the expected result           |
| BLOCKED      | Test cannot be executed because of a blocker or dependency |
| NOT EXECUTED | Test has not been executed yet                             |

---

## 3. Test Execution Results

| Test Case ID | Test Case Title                             | Result       | Actual Result | Bug ID |
| ------------ | ------------------------------------------- | ------------ | ------------- | ------ |
| TC-001       | Login with valid credentials                | Not Executed | Not Executed  | -      |
| TC-002       | Login with invalid username                 | Not Executed | Not Executed  | -      |
| TC-003       | Login with invalid password                 | Not Executed | Not Executed  | -      |
| TC-004       | Login with empty username                   | Not Executed | Not Executed  | -      |
| TC-005       | Login with empty password                   | Not Executed | Not Executed  | -      |
| TC-006       | Login with both fields empty                | Not Executed | Not Executed  | -      |
| TC-007       | Logout functionality                        | Not Executed | Not Executed  | -      |
| TC-008       | Search for an existing product              | Not Executed | Not Executed  | -      |
| TC-009       | Search with invalid keyword                 | Not Executed | Not Executed  | -      |
| TC-010       | Search with empty field                     | Not Executed | Not Executed  | -      |
| TC-011       | Search result relevance                     | Not Executed | Not Executed  | -      |
| TC-012       | Search using partial product name           | Not Executed | Not Executed  | -      |
| TC-013       | Navigate from search result to product page | Not Executed | Not Executed  | -      |
| TC-014       | Product information display                 | Not Executed | Not Executed  | -      |
| TC-015       | Select available product size               | Not Executed | Not Executed  | -      |
| TC-016       | Select unavailable product size             | Not Executed | Not Executed  | -      |
| TC-017       | Selected size retained in cart              | Not Executed | Not Executed  | -      |
| TC-018       | Add product without required size           | Not Executed | Not Executed  | -      |
| TC-019       | Product image and price display             | Not Executed | Not Executed  | -      |
| TC-020       | Add product to cart                         | Not Executed | Not Executed  | -      |
| TC-021       | Product information in cart                 | Not Executed | Not Executed  | -      |
| TC-022       | Increase product quantity                   | Not Executed | Not Executed  | -      |
| TC-023       | Decrease product quantity                   | Not Executed | Not Executed  | -      |
| TC-024       | Cart total calculation                      | Not Executed | Not Executed  | -      |
| TC-025       | Remove product from cart                    | Not Executed | Not Executed  | -      |
| TC-026       | Empty cart behavior                         | Not Executed | Not Executed  | -      |
| TC-027       | Navigate from cart to checkout              | Not Executed | Not Executed  | -      |
| TC-028       | Checkout with valid information             | Not Executed | Not Executed  | -      |
| TC-029       | Checkout with missing required information  | Not Executed | Not Executed  | -      |
| TC-030       | Checkout with invalid input                 | Not Executed | Not Executed  | -      |
| TC-031       | Delivery information                        | Not Executed | Not Executed  | -      |
| TC-032       | Payment method selection                    | Not Executed | Not Executed  | -      |
| TC-033       | Order summary and total                     | Not Executed | Not Executed  | -      |
| TC-034       | Successful order placement                  | Not Executed | Not Executed  | -      |
| TC-035       | Change website language                     | Not Executed | Not Executed  | -      |
| TC-036       | Content displayed in selected language      | Not Executed | Not Executed  | -      |
| TC-037       | Language consistency across pages           | Not Executed | Not Executed  | -      |
| TC-038       | Main navigation                             | Not Executed | Not Executed  | -      |
| TC-039       | Visibility of major UI elements             | Not Executed | Not Executed  | -      |
| TC-040       | Interactive UI elements                     | Not Executed | Not Executed  | -      |

---

## 4. Execution Summary

| Metric           | Count |
| ---------------- | ----: |
| Total Test Cases |    40 |
| Passed           |     0 |
| Failed           |     0 |
| Blocked          |     0 |
| Not Executed     |    40 |
| Pass Rate        |   N/A |

---

## 5. Defect Tracking

When a test case fails, the related Bug ID should be added to the execution results table.

Example:

`TC-024 → FAIL → BUG-002`

The actual result should describe exactly what was observed during test execution.

---

## 6. Retesting

When a defect is fixed, the related test case should be executed again.

Example:

`TC-024 → FAIL → BUG-002 → Retest → PASS`

The retest result should be based on the actual behavior observed after the fix.

---

## 7. Execution Notes

* Test results must be based on actual application behavior.
* Do not mark a test as PASS or FAIL without executing it.
* Actual Result should describe what was observed during execution.
* Failed test cases should be linked to the related Bug ID.
* Screenshots may be attached for failed tests and UI defects.
* Blocked test cases should include the reason why execution could not be completed.
