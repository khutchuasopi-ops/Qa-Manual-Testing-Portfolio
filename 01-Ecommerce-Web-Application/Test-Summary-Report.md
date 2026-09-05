# Test Summary Report

## 1. Project Overview

**Project:** E-commerce Web Application
**Application Under Test:** Confidential E-commerce Web Application
**Testing Type:** Manual Testing
**Role:** Junior Manual QA Tester

This report summarizes the manual testing activities performed for the web application.

The testing covered the main customer-facing functionality, including authentication, product search, product selection, shopping cart, checkout, localization, and user interface behavior.

> **Confidentiality Note:** The application name, organization name, URL, credentials, and confidential business or user information are intentionally excluded from this portfolio.

---

## 2. Testing Scope

The following areas were included in the testing scope:

* Login and authentication
* Product search
* Product information and size selection
* Shopping cart
* Product quantity management
* Checkout flow
* Delivery and payment-related functionality
* Localization
* Main navigation and UI behavior

---

## 3. Testing Types

The following testing approaches were applied:

* Functional Testing
* UI Testing
* Positive Testing
* Negative Testing
* User Flow Testing
* Exploratory Testing
* Regression / Retesting of reported defects

---

## 4. Test Execution Summary

| Metric             | Result |
| ------------------ | -----: |
| Total Test Cases   |     40 |
| Passed             |      2 |
| Failed             |      3 |
| Blocked            |      0 |
| Not Recorded       |     35 |
| Defects Identified |      3 |

The execution report contains the detailed status of each test case.

---

## 5. Identified Defects

Three defects were documented during manual testing.

| Bug ID  | Area          | Related Test Case | Severity | Status |
| ------- | ------------- | ----------------- | -------- | ------ |
| BUG-001 | Localization  | TC-036            | Medium   | Open   |
| BUG-002 | Shopping Cart | TC-024            | Medium   | Open   |
| BUG-003 | Login         | TC-002            | Medium   | Open   |

Detailed defect information is available in the `Bug-Reports` folder.

---

## 6. Key Findings

The testing identified issues affecting several important areas of the application:

* Localization content did not consistently change after language selection.
* Shopping cart totals did not update correctly after changing product quantity.
* Invalid email credentials were accepted during the login process.

These issues were documented using structured bug reports with reproduction steps, expected results, actual results, severity, priority, and related test cases.

---

## 7. QA Workflow Demonstrated

The project demonstrates the following manual QA workflow:

**Test Planning → Test Scenario Design → Test Case Design → Test Execution → Defect Identification → Bug Reporting → Retesting → Test Summary**

This workflow reflects a practical approach to documenting and communicating software quality issues.

---

## 8. Recommendations

Based on the testing results, the following areas should receive additional verification:

1. Authentication validation and negative login scenarios.
2. Shopping cart calculation and quantity updates.
3. Localization consistency across the application.
4. Regression testing after defect fixes.
5. Additional negative testing for checkout and user input validation.
6. Cross-browser verification for critical customer journeys.

---

## 9. Conclusion

The manual testing activities covered the main customer journeys of the e-commerce application and demonstrated the identification and documentation of functional and UI-related defects.

The project demonstrates practical Junior QA Manual Testing skills, including:

* Test scenario creation
* Test case design
* Manual test execution
* Positive and negative testing
* Defect reporting
* Severity and priority assessment
* Test-to-bug traceability
* Retesting concepts
* QA documentation
* GitHub-based portfolio organization

> **Portfolio Note:** This project is presented for professional portfolio purposes. Confidential application, organization, user, and business information has been intentionally excluded.
