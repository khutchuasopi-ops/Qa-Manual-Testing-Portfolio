# Case Study — Legal Platform Manual QA Testing

## 1. Project Overview

This project focused on manual testing of a confidential web-based legal technology platform.

The platform includes functionality for managing documents, templates, events, workflows, repositories, search, and AI-assisted features.

The project has been anonymized for portfolio purposes.

### QA Role

**Junior Manual QA Tester**

The main focus was on functional testing, negative testing, boundary values, input validation, exploratory testing, defect reporting, and data consistency.

---

## 2. Testing Objectives

The main objectives were to:

* Verify that the main user flows work as expected.
* Check form fields and user input validation.
* Test document upload and replacement.
* Test Templates and Events.
* Check Search functionality.
* Check basic UI and usability.
* Test invalid and unexpected input.
* Perform exploratory testing.
* Identify reproducible defects.
* Document defects with clear reproduction steps.
* Support retesting and regression checks.

---

## 3. Testing Approach

Both structured and exploratory manual testing were used.

### Structured Testing

Test scenarios and test cases were created to cover the main application functionality.

The testing included:

* Positive testing
* Negative testing
* Boundary Value Testing
* Input Validation
* Functional Testing
* UI and Usability Testing
* File Upload Testing
* Search and Filtering Testing
* Data Consistency Testing

### Exploratory Testing

Exploratory testing was used to investigate areas beyond the predefined test cases.

The testing focused on:

* Unexpected input
* Empty values
* Whitespace-only values
* Very long input
* File replacement
* UI behavior
* Error handling
* Unexpected application behavior

When an unexpected result was found, it was investigated and reproduced where possible before being treated as a confirmed defect.

---

## 4. Areas Tested

| Area                | Testing Focus                                        |
| ------------------- | ---------------------------------------------------- |
| Dashboard           | Navigation and basic functionality                   |
| Repository          | Documents, upload, replacement, and file information |
| Documents           | Document actions and data consistency                |
| Templates           | Creation, editing, deletion, and validation          |
| Events              | Creation, editing, and name validation               |
| Workflows           | Workflow-related controls and validation             |
| Search              | Search input, results, and clear behavior            |
| Recycle Bin         | Deleted and restored items                           |
| AI Assistant        | Basic interaction and response behavior              |
| Playbook Generation | Generation flow and error handling                   |
| UI                  | Buttons, controls, cursor behavior, and usability    |

---

## 5. Test Data

Different types of input were used during testing.

Examples included:

* Valid names
* Empty input
* Whitespace-only input
* Single-character input
* Very long input
* Special characters
* Different document files
* Replacement files
* Search keywords
* Invalid or unexpected values

The purpose was to check how the application handles both normal and invalid user input.

---

## 6. Defects Identified

Five confirmed defects were documented during testing.

| Bug ID  | Area             | Defect                                                 | Severity | Priority | Status |
| ------- | ---------------- | ------------------------------------------------------ | -------- | -------- | ------ |
| BUG-001 | File Replacement | Old file name remains after document replacement       | Medium   | Medium   | Open   |
| BUG-002 | Search           | Clear Search interaction has incorrect cursor behavior | Low      | Medium   | Open   |
| BUG-003 | Events           | Event accepts whitespace-only name                     | Medium   | High     | Open   |
| BUG-004 | Events           | Event accepts an excessively long name                 | Medium   | Medium   | Open   |
| BUG-005 | Templates        | Template accepts an excessively long name              | Medium   | Medium   | Open   |

Detailed reproduction steps, actual results, expected results, severity, priority, environment, and status are documented separately in the `Bug-Reports` folder.

---

## 7. Example Defect Investigation

### BUG-001 — Old File Name Remains After Document Replacement

During exploratory testing of the Repository, an existing document was replaced with another document.

The replacement action completed, but the displayed file name remained unchanged.

The behavior was reproduced and documented as a data consistency defect.

### Expected Result

The newly uploaded document and its corresponding file name should be displayed.

### Actual Result

The new document was uploaded, but the previous file name remained visible.

### Why It Matters

The displayed file information does not match the current document and may confuse the user.

---

## 8. Exploratory Testing Findings

Exploratory testing also produced findings that were reviewed separately from confirmed defects.

One example was an error observed during Playbook generation.

This was recorded as a finding requiring further verification rather than being added to the confirmed bug count.

This distinction was important because an unexpected result should not automatically be treated as a confirmed defect without enough evidence.

---

## 9. Testing Challenges

One of the main challenges was distinguishing between:

* A confirmed defect
* A validation issue
* A usability concern
* An unexpected but potentially intentional behavior
* A finding that needs more verification

For each potential issue, the following questions were considered:

* Can the behavior be reproduced?
* What is the expected result?
* Is there a clear validation rule?
* Does the behavior affect the user?
* Could the behavior be intentional?
* Is there enough evidence to report it as a defect?

This helped keep the bug reports focused on reproducible issues.

---

## 10. QA Techniques Used

The following manual QA techniques were used:

* Functional Testing
* Positive Testing
* Negative Testing
* Exploratory Testing
* Boundary Value Testing
* Input Validation Testing
* UI and Usability Testing
* Data Consistency Testing
* Search Testing
* Defect Reproduction
* Defect Documentation
* Retesting
* Regression Checks

---

## 11. Test Results

The testing identified **5 confirmed defects**.

All five documented defects currently have an **Open** status.

| Metric                             | Result |
| ---------------------------------- | -----: |
| Confirmed Defects                  |      5 |
| Open Defects                       |      5 |
| Resolved Defects                   |      0 |
| Confirmed Defects Requiring Retest |      0 |

Detailed test execution information is maintained in `Test-Execution.md`.

Test case Pass/Fail statistics are not included here because this case study focuses on the overall testing process and findings rather than duplicating the execution report.

---

## 12. Key Findings

The main findings were related to:

* Data consistency after document replacement
* Event name validation
* Template name validation
* Whitespace-only input
* Search interaction behavior
* Error handling during Playbook generation

These findings showed the importance of testing not only the normal user flow but also invalid, boundary, and unexpected input.

---

## 13. QA Workflow

The project followed a practical manual QA workflow:

**Feature Understanding → Test Planning → Test Scenarios → Test Cases → Manual Execution → Exploratory Testing → Defect Reporting → Retesting → Regression Checks**

---

## 14. Conclusion

This project provided practical experience in testing a web application with multiple connected features.

The testing process included:

* Planning test coverage
* Creating test scenarios
* Writing test cases
* Performing manual functional testing
* Performing negative and boundary testing
* Performing exploratory testing
* Investigating unexpected behavior
* Reproducing defects
* Writing bug reports
* Planning retesting and regression checks

The project also reinforced the importance of separating confirmed defects from findings that require additional verification.

The final project documentation includes:

* Project Overview
* Test Plan
* Test Scenarios
* Test Cases
* Checklists
* Exploratory Testing
* Test Execution
* Bug Reports
* Case Study

---

## 15. Confidentiality

The project has been anonymized for portfolio purposes.

No confidential application URLs, credentials, personal information, or sensitive business data are included.
