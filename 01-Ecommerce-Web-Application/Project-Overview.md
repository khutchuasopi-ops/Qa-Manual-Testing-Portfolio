# Project Overview

## 1. Project Information

| Field        | Details                    |
| ------------ | -------------------------- |
| Project Name | E-commerce Web Application |
| Project Type | Web Application            |
| Testing Role | Junior Manual QA Tester    |
| Testing Type | Manual Testing             |

---

## 2. Project Description

This project focuses on the manual testing of a web-based e-commerce application.

The main goal was to check important user flows and core functionality and to identify and document software defects.

The testing approach focused on the application from an end-user perspective.

---

## 3. Testing Objectives

The main testing objectives were:

* Verify login functionality.
* Verify product search and product selection.
* Verify product size and quantity selection.
* Verify shopping cart functionality.
* Verify cart quantity and price calculations.
* Verify the checkout flow.
* Verify language and localization behavior.
* Identify functional and UI defects.
* Document defects with clear reproduction steps.
* Compare expected and actual results.

---

## 4. Testing Scope

### In Scope

The following application areas were included in the documented testing coverage:

* User Login
* Product Search
* Product Selection
* Product Size Selection
* Product Quantity
* Shopping Cart
* Cart Price Calculation
* Checkout Flow
* Language / Localization
* UI Elements and Navigation
* Basic User Flows

### Out of Scope

The following areas were outside the scope of this project:

* Performance Testing
* Load Testing
* Security Testing
* Automated Testing
* Backend Code Testing
* Database Testing

The project focuses on Junior-level Manual QA testing.

---

## 5. QA Activities

The project includes the following documented QA activities:

* Test Scenario Design
* Test Case Design
* Functional Testing
* Positive Testing
* Negative Testing
* UI Testing
* Manual Test Execution
* Defect Identification
* Bug Reporting
* Severity and Priority Assignment
* Test Summary Reporting

---

## 6. Test Types

The documented testing coverage includes:

* Functional Testing
* UI Testing
* Positive Testing
* Negative Testing

Additional checks such as responsive, cross-browser, regression, and retesting may be used as future or supporting coverage, but they are not presented as completed execution results in this project.

---

## 7. Test Coverage

The project contains:

* **34 Test Scenarios**
* **40 Detailed Test Cases**
* **3 Documented Defects**

The test scenarios describe the planned and documented functional coverage.

The 40 test cases represent the documented historical test execution set.

Not every documented test case has a preserved execution result.

---

## 8. Historical Test Execution

The available historical execution results are:

| Result           | Count |
| ---------------- | ----: |
| Total Test Cases |    40 |
| Passed           |     2 |
| Failed           |     3 |
| Blocked          |     0 |
| Not Recorded     |    35 |

The available recorded results are:

* **TC-001 — PASS** — Valid login completed successfully.
* **TC-002 — FAIL** — Invalid email was accepted during login.
* **TC-003 — PASS** — Invalid password was rejected.
* **TC-024 — FAIL** — Cart total did not update correctly after quantity change.
* **TC-036 — FAIL** — Website content remained in English after another language was selected.

Test cases without an available historical result are marked as **NOT RECORDED**.

No missing execution results were recreated or assumed.

---

## 9. Key User Flows

### Login Flow

User opens the application → enters credentials → submits the login form → verifies the result.

### Product Selection Flow

User searches for a product → opens product details → selects required options → adds the product to the cart.

### Shopping Cart Flow

User opens the cart → verifies product information → changes quantity → checks the displayed price information.

### Checkout Flow

User proceeds to checkout → enters required information → reviews the order information.

### Localization Flow

User selects a language → checks the visible application content.

---

## 10. Defects Identified

Three defects were documented during the available testing activity:

1. **BUG-001 — Localization**
   Website content remained in English after another language was selected.

2. **BUG-002 — Shopping Cart**
   Cart total did not update correctly after the product quantity was changed.

3. **BUG-003 — Login / Authentication**
   An invalid email was accepted during login.

Detailed information is available in the `Bug-Reports` folder.

---

## 11. Test Documentation

The project documentation includes:

* Project Overview
* Test Scenarios
* Test Cases
* Test Execution Report
* Test Summary Report
* Checklists
* Bug Reports
* Case Study

---

## 12. Confidentiality

The application used for this project is confidential.

The following information has intentionally been excluded:

* Application name
* Organization name
* Application URL
* Real credentials
* Confidential business information
* Confidential user information
* Sensitive test data

Only non-sensitive information required to demonstrate the QA testing process is included in this portfolio.

---

## 13. Junior QA Perspective

This project demonstrates my practical foundation in Manual QA Testing.

The focus is on:

* Structured test documentation
* Functional testing
* Positive and negative testing
* UI checks
* Manual test execution
* Defect reporting
* Clear communication of testing results

The project does not claim advanced or production-level QA experience.
