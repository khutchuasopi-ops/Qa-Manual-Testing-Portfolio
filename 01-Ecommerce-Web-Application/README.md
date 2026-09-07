# E-commerce Web Application — Manual QA Testing

## Project Overview

This project demonstrates a practical **Junior Manual QA Testing** workflow for an e-commerce web application.

The portfolio project focuses on test design, manual functional testing, negative testing, UI checks, defect identification, bug reporting, and test documentation.

---

## QA Role

**Junior Manual QA Tester**

---

## Testing Type

**Manual Testing**

---

## Testing Scope

The testing covered the following main application areas:

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

## QA Activities

The project includes the following QA activities:

* Test Scenario Design
* Test Case Design
* Functional Testing
* Positive Testing
* Negative Testing
* UI Testing
* Validation Testing
* Manual Test Execution
* Defect Identification
* Bug Reporting
* Severity and Priority Assignment
* Test Summary Reporting

---

## Test Documentation

The project contains:

* [Test Scenarios](Test-Scenarios.md)
* [Test Cases](Test-Cases.md)
* [Checklists](Checklists.md)
* [Test Execution Report](Test-Execution/Test-Execution-Report.md)
* [Test Summary Report](Test-Summary-Report.md)
* [Case Study](Case-Study.md)
* [Bug Reports](Bug-Reports/)

---

## Test Design

A total of:

* **34 Test Scenarios**
* **40 Detailed Test Cases**

were prepared for the project.

The test cases include:

* Preconditions
* Test Data
* Test Steps
* Expected Results
* Actual Results
* Execution Status
* Related Test Scenarios

---

## Test Execution

The current test execution documentation contains recorded results for a limited subset of the available test cases.

| Result             | Count |
| ------------------ | ----: |
| Total Test Cases   |    40 |
| Passed             |     2 |
| Failed             |     3 |
| Blocked            |     0 |
| Not Recorded       |    35 |
| Defects Identified |     3 |

### Recorded Results

| Test Case | Result | Defect  |
| --------- | ------ | ------- |
| TC-001    | PASS   | —       |
| TC-002    | FAIL   | BUG-003 |
| TC-003    | PASS   | —       |
| TC-024    | FAIL   | BUG-002 |
| TC-036    | FAIL   | BUG-001 |

> The 35 test cases marked as **Not Recorded** do not represent failed tests. No execution result was recorded for those cases in the current execution report.

---

## Defects Identified

Three defects were documented during the recorded testing activity:

| Bug ID  | Summary                                                    | Severity | Priority | Status   |
| ------- | ---------------------------------------------------------- | -------- | -------- | -------- |
| BUG-001 | Website content remains in English after changing language | Medium   | Medium   | Reported |
| BUG-002 | Cart total is calculated incorrectly                       | High     | High     | Reported |
| BUG-003 | Invalid email is accepted during login                     | Medium   | High     | Open     |

Detailed defect information is available in the [Bug Reports](Bug-Reports/) section.

---

## Testing Approach

The testing approach included:

1. Reviewing the main application functionality
2. Creating high-level test scenarios
3. Creating detailed test cases
4. Performing manual testing
5. Checking positive and negative user flows
6. Identifying defects
7. Documenting defects with bug reports
8. Assigning severity and priority
9. Recording test execution results
10. Preparing a test summary

---

## Traceability

Traceability was maintained between test scenarios, test cases, and identified defects.

Examples:

* `TC-002` → `BUG-003`
* `TC-024` → `BUG-002`
* `TC-036` → `BUG-001`

This structure helps connect test execution results with the defects identified during testing.

---

## Tools

The project documentation was created and maintained using:

* GitHub
* Markdown
* Google Chrome
* Chrome DevTools

Additional QA tools and technologies may be explored as part of future learning and testing practice.

---

## Skills Demonstrated

This project demonstrates practical knowledge of:

* Manual Testing
* Functional Testing
* Positive Testing
* Negative Testing
* UI Testing
* Validation Testing
* Test Scenario Design
* Test Case Design
* Bug Reporting
* Severity and Priority Assignment
* Test Execution Documentation
* Test Summary Reporting
* Basic QA Traceability
* GitHub-based QA Documentation

---

## Project Limitations

The current project contains recorded execution results for only **5 of the 40 test cases**.

Therefore, the execution results should not be interpreted as complete coverage of the entire test case set.

Additional testing could include:

* Execution of the remaining test cases
* Broader responsive testing
* Cross-browser compatibility testing
* Regression testing after application changes
* Re-testing after defect fixes
* Additional negative and boundary testing

These are identified as areas for further testing and are not presented as completed activities.

---

## Confidentiality

Application-specific credentials, private test data, and other confidential information are intentionally excluded from this public portfolio.

Only non-sensitive testing information and documentation are presented.

---

## Project Structure

```text
01-Ecommerce-Web-Application/
│
├── Bug-Reports/
│   ├── BUG-001/
│   ├── BUG-002/
│   └── BUG-003/
│
├── Test-Execution/
│   └── Test-Execution-Report.md
│
├── Case-Study.md
├── Checklists.md
├── Project-Overview.md
├── README.md
├── Test-Cases.md
├── Test-Scenarios.md
└── Test-Summary-Report.md
```

---

## Junior QA Perspective

This project was created as practical portfolio work for a **Junior Manual QA Tester**.

The main goal was to demonstrate the ability to:

* Understand application functionality
* Design test scenarios
* Write detailed test cases
* Perform manual functional testing
* Perform positive and negative testing
* Identify and report defects
* Assign severity and priority
* Maintain basic traceability
* Document test execution
* Summarize testing results

The project also demonstrates an organized approach to maintaining QA documentation in GitHub.

---

## Conclusion

This project demonstrates a structured manual QA workflow applied to an e-commerce web application.

It includes **34 test scenarios**, **40 detailed test cases**, recorded execution results, and **3 documented defects**.

The project focuses on practical Junior Manual QA skills and provides a clear example of how testing activities and QA documentation can be organized in a GitHub portfolio.
