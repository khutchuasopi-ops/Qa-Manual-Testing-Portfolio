# Case Study — E-commerce Web Application

## 1. Project Overview

This case study describes a practical manual QA testing project performed on an e-commerce web application.

The main purpose of the project was to practice a structured manual testing process, from test design and execution to defect reporting and test result documentation.

**QA Role:** Junior Manual QA Tester
**Testing Type:** Manual Testing
**Application Type:** E-commerce Web Application

---

## 2. Testing Objective

The main objective was to verify important user-facing functionality and identify defects that could negatively affect the user experience.

The testing focused on:

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

## 3. Testing Scope

The project included the creation of:

* 34 Test Scenarios
* 40 Detailed Test Cases
* Functional and negative test coverage
* UI checks
* Validation checks
* Bug Reports
* Test Execution Report
* Test Summary Report
* Testing Checklists

The main user flows were reviewed from an end-user perspective.

---

## 4. Testing Approach

The testing process followed a basic manual QA workflow:

**Test Scenario Design → Test Case Design → Manual Test Execution → Defect Identification → Bug Reporting → Test Summary**

### Test Scenario Design

High-level scenarios were created to identify the main areas and user flows that required testing.

### Test Case Design

Detailed test cases were created from the scenarios.

The test cases included:

* Preconditions
* Test data
* Test steps
* Expected results
* Actual results
* Execution status
* Related test scenarios

### Manual Execution

A subset of the available test cases was executed and the results were documented separately.

The recorded execution included:

* 2 Passed
* 3 Failed
* 0 Blocked
* 35 Not Recorded

The 35 test cases marked as **Not Recorded** were not treated as failed tests.

---

## 5. Main Testing Areas

### Login

Login functionality was checked using valid and invalid input combinations.

Negative testing included:

* Invalid username
* Invalid password
* Empty username
* Empty password
* Empty login fields
* Invalid email format

### Product Search

Search functionality was reviewed using valid, invalid, empty, and partial search input.

### Product Details

Product information and available size selection were checked.

### Shopping Cart

The cart was tested for:

* Adding products
* Product information
* Quantity changes
* Removing products
* Empty cart behavior
* Total price calculation

### Checkout

The checkout flow was reviewed for:

* Navigation from cart to checkout
* Required information
* Invalid input
* Delivery information
* Payment method
* Order summary
* Order placement

### Localization

Language selection and consistency of displayed content were checked.

### UI and Navigation

Main navigation and important interactive UI elements were reviewed from a usability perspective.

---

## 6. Defects Identified

Three defects were identified during the recorded test execution.

### BUG-001 — Website Content Remains in English After Changing Language

**Severity:** Medium
**Priority:** Medium

The application continued to display some content in English after another language was selected.

**Impact:**
Users may see inconsistent language content while using the application.

**Related Test Case:** TC-036

---

### BUG-002 — Cart Total is Calculated Incorrectly

**Severity:** High
**Priority:** High

The shopping cart displayed an incorrect total amount for the selected product quantity.

**Impact:**
Incorrect pricing can affect the purchasing process and may lead to incorrect order information.

**Related Test Case:** TC-024

---

### BUG-003 — Invalid Email Accepted During Login

**Severity:** Medium
**Priority:** High

The login functionality accepted an invalid email format instead of displaying the expected validation.

**Impact:**
This may result in incorrect validation behavior during the login process.

**Related Test Case:** TC-002

---

## 7. Defect Prioritization

Defects were prioritized based on their potential impact on the user and the affected functionality.

The cart calculation defect was classified as **High severity and High priority** because incorrect price information can directly affect the purchasing flow.

The login validation issue was classified as **Medium severity and High priority** because it affects authentication-related input validation.

The localization issue was classified as **Medium severity and Medium priority** because it affects consistency of the user interface but does not prevent the main application flow.

---

## 8. Traceability

Traceability was maintained between test cases and identified defects.

| Test Case | Defect  |
| --------- | ------- |
| TC-002    | BUG-003 |
| TC-024    | BUG-002 |
| TC-036    | BUG-001 |

This relationship makes it easier to understand which test case identified each defect.

---

## 9. Challenges

One of the main challenges was identifying negative and boundary-related scenarios beyond the basic happy path.

Additional attention was given to:

* Empty fields
* Invalid input
* Product quantity changes
* Required checkout information
* Language consistency
* Incorrect calculation results

Another challenge was maintaining consistency between test scenarios, detailed test cases, execution results, and bug reports.

---

## 10. Key Learnings

This project helped develop practical understanding of:

* How to break application functionality into test scenarios
* How to create detailed test cases
* How to write clear test steps
* How to define expected results
* How to perform positive and negative testing
* How to identify and document defects
* How to assign severity and priority
* How to maintain traceability
* How to summarize test execution results
* How to organize QA documentation in GitHub

The project also reinforced the importance of clear and reproducible bug reports.

---

## 11. Junior QA Perspective

As a Junior Manual QA Tester, the main focus of this project was to demonstrate a structured approach to manual testing rather than advanced automation or specialized testing techniques.

The project provided practical experience with the basic QA workflow and helped strengthen skills in:

* Test design
* Manual test execution
* Functional testing
* Negative testing
* UI testing
* Validation testing
* Defect reporting
* Test documentation

The project also highlighted areas where further practical experience would be valuable.

---

## 12. Areas for Further Testing

Additional testing could be performed in the following areas:

1. Execute the remaining test cases that currently have no recorded result.
2. Re-test reported defects after fixes become available.
3. Perform additional responsive layout checks.
4. Perform broader browser compatibility checks.
5. Perform regression testing after significant application changes.
6. Expand negative and boundary-value testing.
7. Verify additional checkout and order scenarios.

These areas are identified as **further testing opportunities** and are not presented as completed testing activities.

---

## 13. Confidentiality

Application-specific credentials, private test data, and other confidential information are intentionally excluded from this public portfolio.

The case study contains only non-sensitive testing information necessary to demonstrate the QA process.

---

## 14. Conclusion

This project demonstrates a practical approach to manual QA testing of an e-commerce web application.

The project includes **34 test scenarios**, **40 detailed test cases**, and **3 documented defects**.

The testing focused on important user-facing functionality including authentication, product search, product selection, shopping cart, checkout, localization, and UI/navigation.

The project demonstrates Junior Manual QA skills in test design, manual execution, defect identification, bug reporting, prioritization, traceability, and QA documentation.
