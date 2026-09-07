# Test Summary Report

## 1. Project Information

| Field          | Details                      |
| -------------- | ---------------------------- |
| Project        | E-commerce Web Application   |
| Project Type   | Web Application              |
| Testing Type   | Manual Testing               |
| Testing Role   | Junior Manual QA Tester      |
| Application    | Confidential                 |
| Test Execution | Historical execution results |

---

## 2. Testing Objective

The main objective of this testing activity was to verify the main functionality and user flows of the e-commerce web application through manual testing.

The testing focused on identifying functional and UI issues and documenting the results in a clear and structured way.

---

## 3. Testing Scope

The following areas were covered in the documented test scenarios and test cases:

* User Login
* Authentication validation
* Product Search
* Product Selection
* Product Size Selection
* Product Quantity
* Shopping Cart
* Cart Price Calculation
* Checkout Flow
* Delivery Information
* Payment Information
* Order Summary
* Language / Localization
* Navigation
* Basic UI checks

### Out of Scope

The following areas were not part of this manual testing activity:

* Performance Testing
* Load Testing
* Security Testing
* Automated Testing
* Backend Code Testing
* Database Testing

---

## 4. Test Coverage

The project contains:

* **34 Test Scenarios**
* **40 Detailed Test Cases**
* **3 Documented Defects**

The test scenarios describe the areas that should be tested, while the 40 test cases represent the documented historical test execution set.

Not all historical execution results were preserved. Therefore, test cases without confirmed historical results are marked as **NOT RECORDED**.

---

## 5. Test Execution Summary

| Result           | Count |
| ---------------- | ----: |
| Total Test Cases |    40 |
| Passed           |     2 |
| Failed           |     3 |
| Blocked          |     0 |
| Not Recorded     |    35 |

### Execution Result Notes

* **PASS** — The actual result matched the expected result.
* **FAIL** — The actual result did not match the expected result.
* **BLOCKED** — Testing could not be completed because of a blocker or dependency.
* **NOT RECORDED** — The original execution result was not available and was not recreated.

No result has been marked as passed or failed unless there was a recorded result for the historical execution.

---

## 6. Recorded Test Results

The following test cases have confirmed historical execution results:

| Test Case | Result | Summary                                                   |
| --------- | ------ | --------------------------------------------------------- |
| TC-001    | PASS   | Valid login completed successfully                        |
| TC-002    | FAIL   | Invalid email was accepted during login                   |
| TC-003    | PASS   | Invalid password was rejected                             |
| TC-024    | FAIL   | Cart total did not update correctly after quantity change |
| TC-036    | FAIL   | Page content remained in English after changing language  |

---

## 7. Defect Summary

Three defects were identified and documented during the testing activity.

| Bug ID  | Area                   | Severity | Priority | Status   |
| ------- | ---------------------- | -------- | -------- | -------- |
| BUG-001 | Localization           | Medium   | Medium   | Reported |
| BUG-002 | Shopping Cart          | High     | High     | Reported |
| BUG-003 | Login / Authentication | Medium   | High     | Open     |

---

## 8. Key Findings

### BUG-001 — Localization

After selecting another language, the website content remained in English.

**Related Test Case:** TC-036

This indicates that the language selection did not correctly update the visible website content.

---

### BUG-002 — Shopping Cart

The cart total price did not update correctly after changing the product quantity.

**Related Test Case:** TC-024

This can result in an incorrect total being displayed to the user.

---

### BUG-003 — Login

An invalid email was accepted during login and the user was redirected to the home page.

**Related Test Case:** TC-002

This indicates an issue with validation of the email input during the login flow.

---

## 9. Testing Approach

The testing activity followed a basic manual QA workflow:

1. Review the main application functionality.
2. Identify important user flows.
3. Create test scenarios.
4. Create detailed test cases.
5. Perform manual testing where execution results were available.
6. Compare actual results with expected results.
7. Document identified defects.
8. Assign severity and priority.
9. Prepare a test summary.

---

## 10. Test Documentation

The project includes the following QA documentation:

* Test Scenarios
* Test Cases
* Test Execution Report
* Test Summary Report
* Checklists
* Bug Reports
* Case Study
* Project Overview

These documents demonstrate the process of organizing test coverage and documenting manual testing results.

---

## 11. Recommendations

Based on the recorded results, the following areas should receive additional verification:

* Login validation, especially invalid email formats
* Shopping cart quantity and total price calculations
* Localization after changing the selected language
* Checkout validation
* Negative testing for required fields
* Verification of fixes for reported defects
* Regression checks after defect fixes
* UI and navigation checks across supported browsers

These recommendations represent suggested follow-up testing and are not additional executed results.

---

## 12. Limitations

The original execution history was not fully preserved.

For this reason:

* 35 test cases are marked **NOT RECORDED**.
* Missing results were not recreated.
* No additional PASS or FAIL results were invented.
* The report represents the available historical execution information.

The documented test cases and scenarios demonstrate planned and documented coverage, but they should not be interpreted as proof that every documented test was executed.

---

## 13. Confidentiality

The application used for this testing activity is confidential.

The following information has intentionally not been included in this portfolio:

* Application name
* Organization name
* Application URL
* Real credentials
* Confidential business information
* Confidential user information
* Sensitive screenshots or data

The portfolio contains only the information necessary to demonstrate the QA testing process and documentation skills.

---

## 14. Junior QA Perspective

This project was completed as a practical manual QA portfolio project to demonstrate foundational testing skills.

The main skills demonstrated include:

* Manual Functional Testing
* Positive and Negative Testing
* UI Testing
* Test Scenario Design
* Test Case Design
* Test Execution
* Defect Reporting
* Severity and Priority
* Test Documentation
* Basic Regression / Retesting Concepts
* GitHub Documentation

The project does not claim production-level or advanced QA experience. It demonstrates a structured approach to learning and applying manual QA testing practices.

---

## 15. Final Assessment

The testing activity identified functional issues in important parts of the application, including login validation, shopping cart calculations, and localization.

The project demonstrates the ability to:

* Break an application into testable areas
* Create structured test scenarios
* Write detailed test cases
* Record available execution results
* Identify and document defects
* Distinguish severity and priority
* Maintain QA documentation
* Communicate testing results clearly

Overall, this project demonstrates a practical foundation in **Junior Manual QA Testing**.

