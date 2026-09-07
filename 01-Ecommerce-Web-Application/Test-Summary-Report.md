# Test Summary Report — E-commerce Web Application

## 1. Project Information

| Field               | Details                    |
| ------------------- | -------------------------- |
| Project             | E-commerce Web Application |
| Testing Type        | Manual Testing             |
| QA Role             | Junior Manual QA Tester    |
| Test Scenarios      | 34                         |
| Detailed Test Cases | 40                         |
| Identified Defects  | 3                          |
| Documentation       | GitHub / Markdown          |

---

## 2. Testing Objective

The objective of this testing activity was to evaluate the main functionality and user flows of the e-commerce web application through manual testing.

The testing focused on identifying functional, validation, UI, and localization issues in important user-facing areas.

---

## 3. Testing Scope

The following areas were included in the testing scope:

* Login and authentication
* Product search
* Product details
* Product size selection
* Shopping cart
* Product quantity management
* Checkout
* Localization
* UI and navigation

---

## 4. Test Design

The test documentation was prepared using:

* Test Scenarios
* Detailed Test Cases
* Checklists
* Bug Reports
* Test Execution Report
* Test Summary Report

A total of **34 test scenarios** and **40 detailed test cases** were created.

---

## 5. Test Execution Summary

The execution report contains recorded results for a limited subset of the available test cases.

| Result             | Count |
| ------------------ | ----: |
| Total Test Cases   |    40 |
| Passed             |     2 |
| Failed             |     3 |
| Blocked            |     0 |
| Not Recorded       |    35 |
| Defects Identified |     3 |

### Recorded Test Cases

| Test Case | Result | Defect  |
| --------- | ------ | ------- |
| TC-001    | PASS   | —       |
| TC-002    | FAIL   | BUG-003 |
| TC-003    | PASS   | —       |
| TC-024    | FAIL   | BUG-002 |
| TC-036    | FAIL   | BUG-001 |

> **Note:** The 35 "Not Recorded" test cases do not mean that they failed. No execution result was recorded for these cases in the current test execution report.

---

## 6. Defect Summary

Three defects were identified during the recorded testing activity.

| Bug ID  | Summary                                                    | Severity | Priority | Status   |
| ------- | ---------------------------------------------------------- | -------- | -------- | -------- |
| BUG-001 | Website content remains in English after changing language | Medium   | Medium   | Reported |
| BUG-002 | Cart total is calculated incorrectly                       | High     | High     | Reported |
| BUG-003 | Invalid email is accepted during login                     | Medium   | High     | Open     |

---

## 7. Key Findings

### BUG-001 — Localization Issue

The application does not consistently display content in the selected language.

**Impact:**
Users may see mixed-language content after changing the application language.

**Severity:** Medium

**Priority:** Medium

---

### BUG-002 — Incorrect Cart Total

The shopping cart displays an incorrect total amount for the selected product quantity.

**Impact:**
Incorrect price information can directly affect the user's purchasing decision and checkout flow.

**Severity:** High

**Priority:** High

---

### BUG-003 — Invalid Email Accepted During Login

The login functionality accepts an invalid email format and allows the user to continue instead of displaying appropriate validation.

**Impact:**
This may cause incorrect authentication behavior and indicates a validation issue in the login flow.

**Severity:** Medium

**Priority:** High

---

## 8. Testing Approach

The testing approach included:

* Positive test cases for expected user behavior
* Negative test cases for invalid or missing input
* Functional testing of important application features
* UI checks for important user-facing elements
* Validation testing for form inputs
* User flow testing across major application areas
* Manual defect identification and reporting

The testing was performed from a user perspective with focus on the application's visible behavior.

---

## 9. Defect Prioritization

Defects were prioritized based on their potential impact on the user and the affected functionality.

### High Priority

* Incorrect cart total
* Invalid email accepted during login

### Medium Priority

* Inconsistent language display

The cart calculation issue received **High severity and High priority** because incorrect pricing can affect the purchasing process.

---

## 10. Traceability

The project maintains traceability between testing documentation and reported defects.

Examples:

* `TC-002` → `BUG-003`
* `TC-024` → `BUG-002`
* `TC-036` → `BUG-001`

This relationship makes it easier to identify which test case detected a specific defect.

---

## 11. Documentation Quality

The project includes the following QA documentation:

* Project Overview
* Test Scenarios
* Test Cases
* Checklists
* Test Execution Report
* Bug Reports
* Test Summary Report
* Case Study

The documentation is organized so that test design, execution results, and defect information can be reviewed separately.

---

## 12. Limitations

The current execution dataset contains recorded results for only **5 of the 40 test cases**.

Therefore:

* The execution results do not represent complete coverage of all 40 test cases.
* The 35 unrecorded test cases should not be interpreted as passed or failed.
* Additional execution would be required for a complete test assessment.
* Further testing could include broader browser, responsive, regression, and retesting coverage when applicable.

---

## 13. Recommendations

Based on the identified issues, the following areas could receive additional testing:

1. Verify cart calculations with different products and quantities.
2. Perform additional validation testing for login fields.
3. Verify language consistency across all supported pages.
4. Execute the remaining unrecorded test cases.
5. Re-test reported defects after fixes are available.
6. Perform additional responsive and browser compatibility checks if required.

---

## 14. Junior QA Perspective

This project was completed as a practical **Junior Manual QA Testing** exercise.

The main focus was on developing practical skills in:

* Understanding application requirements
* Creating test scenarios
* Writing detailed test cases
* Performing manual functional testing
* Performing positive and negative testing
* Identifying defects
* Writing clear bug reports
* Assigning severity and priority
* Maintaining traceability
* Preparing test documentation
* Summarizing test results

The project also helped develop a structured approach to analyzing application behavior from an end-user perspective.

---

## 15. Overall Assessment

The testing activity identified functional, validation, and localization issues within the tested areas.

The project demonstrates practical knowledge of the basic manual QA workflow:

**Test Scenario Design → Test Case Design → Manual Execution → Defect Identification → Bug Reporting → Test Summary**

The current results provide useful evidence of the testing process, while the unrecorded test cases show that additional execution would be required for full test coverage.

---

## 16. Confidentiality

Application-specific credentials, private test data, and confidential information are intentionally not included in this public portfolio.

Only testing methodology, documentation structure, and non-sensitive defect information are presented.

---

## 17. Final Conclusion

The project demonstrates a structured approach to manual testing of an e-commerce web application.

A total of **34 test scenarios** and **40 detailed test cases** were prepared. During the recorded execution, **3 defects** were identified and documented.

The main issues were related to:

* Localization
* Cart total calculation
* Login input validation

The project provides practical evidence of Junior Manual QA skills in test design, manual execution, defect reporting, prioritization, traceability, and test documentation.
