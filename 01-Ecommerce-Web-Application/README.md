# E-commerce Web Application — Manual QA Testing

## Project Overview

This project demonstrates practical **Manual QA Testing** of an e-commerce web application.

The goal of the project is to practice and demonstrate core software testing activities, including test design, manual execution, exploratory testing, smoke testing, regression testing, defect identification, bug reporting, and test reporting.

**QA Role:** Junior Manual QA Tester
**Testing Type:** Manual Testing
**Application Type:** E-commerce Web Application

---

## Testing Scope

The main application areas covered in this project are:

* Login and Authentication
* Product Search
* Product Details
* Size Selection
* Shopping Cart
* Checkout
* Localization
* UI and Navigation

---

## QA Activities

The project includes the following testing activities:

* Test Scenario Design
* Test Case Design
* Functional Testing
* Positive Testing
* Negative Testing
* UI Testing
* Exploratory Testing
* Smoke Testing
* Regression Testing
* Manual Test Execution
* Defect Identification
* Bug Reporting
* Severity and Priority Assignment
* Test Summary Reporting

---

## Test Design

The project contains:

* **34 Test Scenarios**
* **40 Detailed Test Cases**
* Positive and negative test coverage
* User-flow based testing
* Localization testing
* UI and navigation checks

The test cases are documented separately from execution results so that test design and test execution can be clearly distinguished.

---

## Test Execution Summary

The current execution record contains **40 test cases**.

| Result       |  Count |
| ------------ | -----: |
| PASS         |      2 |
| FAIL         |      3 |
| BLOCKED      |      0 |
| Not Recorded |     35 |
| **Total**    | **40** |

### Recorded Test Cases

| Test Case | Result |
| --------- | ------ |
| TC-001    | PASS   |
| TC-002    | FAIL   |
| TC-003    | PASS   |
| TC-024    | FAIL   |
| TC-036    | FAIL   |

The remaining test cases are marked as **Not Recorded** because no execution result was recorded for them.

This distinction is maintained to avoid presenting unexecuted or undocumented tests as completed testing results.

---

## Defects Identified

Three defects are documented in the project.

| Bug ID  | Severity | Priority | Status   |
| ------- | -------- | -------- | -------- |
| BUG-001 | Medium   | Medium   | Reported |
| BUG-002 | High     | High     | Reported |
| BUG-003 | Medium   | High     | Open     |

### Defect Areas

The documented defects relate to:

* Localization
* Shopping Cart
* Login / Authentication

Each defect report contains:

* Bug description
* Steps to reproduce
* Expected result
* Actual result
* Impact
* Severity
* Priority
* Related test case
* Related test scenario

---

## Testing Approach

### Functional Testing

The main application functions and user flows were checked to identify whether they behaved as expected.

### Positive Testing

Valid input and expected user actions were used to verify normal application behavior.

### Negative Testing

Invalid input and unexpected user actions were considered to identify validation and error-handling issues.

### Exploratory Testing

The application was explored beyond predefined test cases to identify additional unexpected behavior and usability issues.

### Smoke Testing

Basic checks of important application functionality were performed to verify that the main flows were available for testing.

### Regression Testing

Relevant functionality was re-checked to verify that existing behavior continued to work as expected.

### UI Testing

Important interface elements, navigation, visibility, and user interaction were checked manually.

---

## Traceability

The project demonstrates traceability between testing artifacts:

**Test Scenario → Test Case → Test Execution → Bug Report**

Example:

`TS-002 → TC-002 → FAIL → BUG-003`

This structure helps connect identified defects to the related testing scenario and test case.

---

## Project Documentation

### Test Planning & Design

* [Project Overview](Project-Overview.md)
* [Test Scenarios](Test-Scenarios.md)
* [Test Cases](Test-Cases.md)
* [Checklists](Checklists.md)

### Test Execution & Reporting

* [Test Execution Report](Test-Execution/Test-Execution-Report.md)
* [Test Summary Report](Test-Summary-Report.md)

### Defect Reports

* [BUG-001](Bug-Reports/BUG-001.md)
* [BUG-002](Bug-Reports/BUG-002.md)
* [BUG-003](Bug-Reports/BUG-003.md)

### Case Study

* [Case Study](Case-Study.md)

---

## Tools

Tools used for this project include:

* GitHub
* Markdown
* Google Chrome
* Chrome DevTools

---

## Skills Demonstrated

### Test Design

* Test Scenario Design
* Test Case Design
* Positive Test Design
* Negative Test Design
* User Flow Coverage

### Manual Testing

* Functional Testing
* Exploratory Testing
* Smoke Testing
* Regression Testing
* UI Testing
* Localization Testing

### Defect Management

* Defect Identification
* Bug Reporting
* Severity Assignment
* Priority Assignment
* Defect Traceability

### Documentation

* Test Cases
* Test Scenarios
* Checklists
* Test Execution Reports
* Test Summary Reports
* Case Study Documentation

---

## Limitations

This project represents a practical learning portfolio project and should not be considered production-level QA experience.

The execution report contains only recorded results. Test cases without recorded results are intentionally shown as **Not Recorded**.

Additional testing areas such as API testing, database testing, cross-browser testing, and responsive testing may require separate environments, tools, or test data.

---

## Confidentiality

Application-specific credentials, private test data, and other confidential information are intentionally excluded from this public portfolio.

Only non-sensitive testing documentation and examples are included.

---

## Junior QA Perspective

This project reflects my current level as a **Junior Manual QA Tester**.

It demonstrates my ability to structure testing activities, design test cases, perform manual testing, explore application behavior, document defects, and communicate testing results clearly.

My goal is to continue improving my practical QA skills through hands-on testing and further learning.
