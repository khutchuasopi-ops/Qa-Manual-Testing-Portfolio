# E-commerce Web Application — Manual QA Testing

## Project Overview

This project is a practical **Manual QA Testing portfolio project** for a confidential e-commerce web application.

The project demonstrates my approach to testing a web application by creating test scenarios, detailed test cases, checklists, documenting available execution results, and reporting identified defects.

**Testing Role:** Junior Manual QA Tester
**Testing Type:** Manual Testing
**Application Type:** Web Application

---

## Testing Scope

The main areas covered in this project are:

* Login and Authentication
* Product Search
* Product Details
* Product Size Selection
* Product Quantity
* Shopping Cart
* Cart Price Calculation
* Checkout
* Delivery Information
* Payment Information
* Order Summary
* Language / Localization
* Navigation
* Basic UI Checks

### Out of Scope

* Performance Testing
* Load Testing
* Security Testing
* Automated Testing
* Backend Code Testing
* Database Testing

---

## QA Activities

The project includes the following manual QA activities:

* Test Scenario Design
* Test Case Design
* Positive Testing
* Negative Testing
* Functional Testing
* UI Testing
* Exploratory Testing
* Manual Test Execution
* Defect Identification
* Bug Reporting
* Severity and Priority Assignment
* Retesting / Defect Verification Concepts
* Test Summary Reporting

---

## Test Documentation

| Document                                                         | Description                                  |
| ---------------------------------------------------------------- | -------------------------------------------- |
| [Project Overview](Project-Overview.md)                          | Project scope, objectives, and testing areas |
| [Test Scenarios](Test-Scenarios.md)                              | High-level testing scenarios                 |
| [Test Cases](Test-Cases.md)                                      | Detailed manual test cases                   |
| [Test Execution Report](Test-Execution/Test-Execution-Report.md) | Available historical execution results       |
| [Test Summary Report](Test-Summary-Report.md)                    | Overall testing summary                      |
| [Checklists](Checklists.md)                                      | Manual QA checklists                         |
| [Case Study](Case-Study.md)                                      | Detailed project description                 |
| Bug Reports                                                      | Documented defects found during testing      |

---

## Test Coverage

The project currently contains:

* **34 Test Scenarios**
* **40 Detailed Test Cases**
* **3 Documented Defects**

The 34 test scenarios describe the documented functional coverage.

The 40 test cases represent the documented historical test execution set.

The documented test cases and scenarios should not be interpreted as proof that every test was executed.

---

## Historical Test Execution

The available historical execution results are:

| Result           | Count |
| ---------------- | ----: |
| Total Test Cases |    40 |
| Passed           |     2 |
| Failed           |     3 |
| Blocked          |     0 |
| Not Recorded     |    35 |

### Recorded Results

* **TC-001 — PASS** — Valid login completed successfully
* **TC-002 — FAIL** — Invalid email was accepted during login
* **TC-003 — PASS** — Invalid password was rejected
* **TC-024 — FAIL** — Cart total did not update correctly after quantity change
* **TC-036 — FAIL** — Website content remained in English after changing language

Historical results that were not available are marked as **NOT RECORDED**.

No missing execution results were recreated or assumed.

---

## Documented Defects

Three defects were identified and documented:

| Bug     | Area                   | Severity | Priority | Status   |
| ------- | ---------------------- | -------- | -------- | -------- |
| BUG-001 | Localization           | Medium   | Medium   | Reported |
| BUG-002 | Shopping Cart          | High     | High     | Reported |
| BUG-003 | Login / Authentication | Medium   | High     | Open     |

Detailed bug reports are available in the `Bug-Reports` folder.

---

## Example User Flows Tested

### Login Flow

Login → Credential Validation → User Access

### Product Flow

Search Product → Open Product → Select Size → Add to Cart

### Shopping Cart Flow

Add Product → Open Cart → Change Quantity → Check Total

### Checkout Flow

Cart → Checkout → Customer Information → Delivery → Payment → Order Summary

### Localization Flow

Select Language → Review Visible Page Content

---

## Testing Approach

The testing process followed a basic manual QA workflow:

**Functional Areas → Test Scenarios → Test Cases → Manual Execution → Defect Reporting → Test Summary**

Testing focused on comparing the application's actual behavior with the expected behavior described in the test cases.

---

## Tools

* Manual Testing
* GitHub
* Markdown
* Google Chrome
* Browser DevTools
* Jira / ClickUp concepts
* Basic SQL knowledge

---

## QA Skills Demonstrated

* Functional Testing
* Positive Testing
* Negative Testing
* UI Testing
* Exploratory Testing
* Test Scenario Design
* Test Case Design
* Manual Test Execution
* Bug Reporting
* Severity and Priority
* Retesting Concepts
* QA Documentation
* GitHub Repository Management

---

## Key Findings

The available execution results identified issues in three areas:

### Login

An invalid email was accepted during login.

**Bug:** BUG-003

### Shopping Cart

The cart total did not update correctly after changing the product quantity.

**Bug:** BUG-002

### Localization

Website content remained in English after another language was selected.

**Bug:** BUG-001

---

## Confidentiality

The application used for this project is confidential.

The following information has intentionally been excluded:

* Application name
* Organization name
* Application URL
* Real credentials
* Confidential business information
* Confidential user information
* Sensitive screenshots or test data

Only non-sensitive information required to demonstrate the QA testing process is included in this portfolio.

---

## Portfolio Note

This project represents my practical learning and portfolio work as a **Junior Manual QA Tester**.

It demonstrates foundational manual testing, test documentation, defect reporting, and structured QA thinking.

The project does not claim advanced or production-level QA experience.
