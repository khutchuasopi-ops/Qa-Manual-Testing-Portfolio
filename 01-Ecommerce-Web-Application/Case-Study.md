# Case Study — E-commerce Web Application

## 1. Project Overview

This project was created as a practical manual QA testing portfolio project for a confidential e-commerce web application.

The main goal was to practice a structured manual testing process and demonstrate the ability to design test scenarios, write test cases, execute available test cases, identify defects, and document testing results.

**Testing Role:** Junior Manual QA Tester
**Testing Type:** Manual Testing
**Application Type:** Web Application

---

## 2. Testing Objective

The main objectives of the testing activity were to:

* Verify important user flows.
* Check expected application behavior.
* Identify functional and UI issues.
* Create clear and reproducible test cases.
* Document defects with steps to reproduce.
* Compare expected and actual results.
* Prepare a clear test summary.

---

## 3. Testing Scope

The main areas covered in the project were:

* Login and authentication
* Product search
* Product selection
* Product size selection
* Product quantity
* Shopping cart
* Cart price calculation
* Checkout
* Delivery information
* Payment information
* Order summary
* Language and localization
* Navigation and basic UI checks

---

## 4. Testing Approach

The testing process followed a basic manual QA workflow.

### Step 1 — Identify Functional Areas

The application was divided into important functional areas such as Login, Search, Product, Cart, Checkout, and Localization.

### Step 2 — Create Test Scenarios

High-level test scenarios were created to describe the functionality that needed to be checked.

The project contains **34 documented test scenarios**.

### Step 3 — Create Test Cases

Detailed test cases were created based on the identified scenarios.

The project contains **40 documented test cases** representing the historical test execution set.

### Step 4 — Manual Test Execution

Available historical execution results were reviewed and documented.

The execution report contains:

* 2 Passed
* 3 Failed
* 0 Blocked
* 35 Not Recorded

Results that were not available were intentionally marked as **NOT RECORDED** instead of being recreated.

### Step 5 — Defect Reporting

Issues found during testing were documented as individual bug reports.

Each report includes:

* Bug title
* Severity
* Priority
* Description
* Steps to reproduce
* Expected result
* Actual result
* Related test case

---

## 5. Main Testing Areas

### Login

Login functionality was checked using valid and invalid input.

The testing included:

* Valid login
* Invalid username/email
* Invalid password
* Empty required fields
* Logout

One defect was identified where an invalid email was accepted during login.

**Related Bug:** BUG-003

---

### Product Search

Search functionality was checked using different search inputs.

The testing included:

* Valid search
* Invalid search
* Empty search
* Partial product names
* Search result relevance
* Navigation from search results

---

### Product Details

Product information and selection behavior were checked.

The testing included:

* Product information
* Product image and price
* Available sizes
* Unavailable sizes
* Selected size behavior
* Adding a product without selecting a required size

---

### Shopping Cart

The shopping cart was checked after adding products.

The testing included:

* Adding products
* Product information in the cart
* Increasing quantity
* Decreasing quantity
* Cart total calculation
* Removing products
* Empty cart behavior

One defect was identified where the cart total did not update correctly after changing the quantity.

**Related Bug:** BUG-002

---

### Checkout

The checkout flow was reviewed from the cart through the order summary.

The documented coverage included:

* Navigation to checkout
* Checkout information
* Required field validation
* Delivery information
* Payment information
* Order summary
* Successful order flow
* Invalid and missing input

---

### Localization

Language selection and visible page content were checked.

One defect was identified where the website content remained in English after another language was selected.

**Related Bug:** BUG-001

---

## 6. Defects Identified

Three defects were documented during the testing activity.

| Bug ID  | Area                   | Severity | Priority |
| ------- | ---------------------- | -------- | -------- |
| BUG-001 | Localization           | Medium   | Medium   |
| BUG-002 | Shopping Cart          | High     | High     |
| BUG-003 | Login / Authentication | Medium   | High     |

Detailed information about each issue is available in the `Bug-Reports` folder.

---

## 7. Challenges

One of the main challenges was maintaining sufficient coverage across several different e-commerce user flows.

To address this, the application was divided into functional areas and separate scenarios, test cases, and checklists were created for each area.

Another challenge was working with incomplete historical execution information.

Instead of assuming missing results, unavailable results were marked as **NOT RECORDED**.

---

## 8. Key Learnings

This project helped strengthen my understanding of:

* Writing structured test scenarios
* Writing detailed test cases
* Creating testing checklists
* Performing positive and negative testing
* Identifying functional defects
* Writing clear bug reports
* Creating reproducible steps
* Understanding expected vs. actual results
* Using severity and priority
* Following basic manual QA workflow
* Documenting testing results
* Thinking from the end-user perspective

---

## 9. Junior QA Perspective

This project represents my practical learning and portfolio work as a **Junior Manual QA Tester**.

The purpose of the project is to demonstrate foundational manual testing and documentation skills rather than advanced or production-level QA experience.

The project demonstrates my ability to approach a web application systematically, organize test coverage, document defects, and communicate testing results clearly.

---

## 10. Areas for Further Testing

Based on the documented testing activity, additional testing could include:

* More negative login scenarios
* Additional checkout validation
* More cart calculation scenarios
* Additional localization checks
* Verification of reported defects after fixes
* Regression testing after changes
* Cross-browser verification
* Additional UI and responsive checks

These items represent recommended future testing and are not claimed as completed execution results.

---

## 11. Conclusion

The project provided practical experience in applying a structured manual QA process to an e-commerce web application.

During the project, I created test scenarios, detailed test cases, checklists, execution documentation, and bug reports.

The testing activity identified issues related to login validation, shopping cart calculations, and localization.

Overall, this case study demonstrates my current foundation in **Manual QA Testing** and my ability to create clear, organized, and useful QA documentation.

