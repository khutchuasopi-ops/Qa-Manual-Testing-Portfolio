# Case Study – Legal Platform Manual Testing

## 1. Project Overview

This project focused on manual testing of a web-based legal platform designed to support organizations and their members with document and contract-related activities.

The platform includes functionality for managing documents, templates, events, workflows, tasks, search, and other collaboration-related features.

The goal of the testing was to evaluate the application's functionality, usability, validation, and consistency from an end-user perspective.

---

## 2. Testing Objectives

The main objectives were to:

- Verify that core features work according to expected behavior.
- Validate form fields and user input.
- Test document upload and replacement functionality.
- Test Templates and Events.
- Verify Search functionality.
- Check navigation and UI behavior.
- Identify invalid or unexpected user inputs.
- Perform exploratory testing to discover issues outside predefined test cases.
- Document and validate reproducible defects.

---

## 3. Testing Approach

A combination of structured and exploratory manual testing was used.

### Structured Testing

Test scenarios and test cases were created before execution to provide consistent coverage of the application's main functionality.

Testing included:

- Positive test cases
- Negative test cases
- Boundary-value testing
- Input validation
- UI and usability checks
- File upload testing
- Navigation testing

### Exploratory Testing

Exploratory testing was also performed by interacting with the application without following predefined test cases.

This helped identify unexpected behaviors such as:

- Invalid input being accepted.
- Incorrect information being displayed after document replacement.
- UI interaction inconsistencies.
- Extremely long input being accepted.

---

## 4. Areas Tested

The following areas were explored during testing:

| Area | Testing Focus |
|---|---|
| Repository | Document upload, replacement and file information |
| Templates | Template creation and input validation |
| Events | Event creation and name validation |
| Search | Search input and clear functionality |
| Workflows | Date and workflow-related controls |
| Dashboard | Activity overview and navigation |
| Tasks | Filters and task-related functionality |
| AI Assistant | Basic interaction and response behavior |
| UI | Buttons, icons, cursor behavior and usability |

---

## 5. Test Data

Different types of input were used to evaluate application validation.

Examples included:

- Valid names
- Empty input
- Whitespace-only input
- Single-character input
- Very long input
- Special characters
- Different document files
- Replacing an existing uploaded document

The purpose was to determine how the application handles both normal and unexpected user input.

---

## 6. Defects Identified

Five confirmed defects were documented during testing.

| ID | Area | Defect | Severity | Status |
|---|---|---|---|---|
| BUG-001 | Repository | Old file name remains after document replacement | Medium | Open |
| BUG-002 | Search | Clear Search icon does not display pointer cursor | Low | Open |
| BUG-003 | Events | Event can be created with whitespace-only name | Medium | Open |
| BUG-004 | Events | Event accepts an excessively long name | Medium | Open |
| BUG-005 | Templates | Template accepts an excessively long name | Medium | Open |

Detailed reproduction steps, expected results, actual results, impact, and severity are documented separately in the `Bug-Reports` folder.

---

## 7. Example Defect Investigation

### BUG-001 – Old File Name Remains After Replacing a Document

During exploratory testing of the Repository, I uploaded a PDF document and then replaced it with a different PDF.

The replacement operation completed successfully, but the displayed file name remained the name of the original document.

I reproduced the behavior and documented it as a functional/data consistency defect.

### Expected

The newly uploaded document and its corresponding file name should be displayed.

### Actual

The new document was uploaded, but the previous file name remained visible.

### Impact

This can cause confusion for users because the displayed file information does not correspond to the current document.

---

## 8. Testing Challenges

One of the main challenges was distinguishing between an actual defect and expected application behavior.

Not every unexpected behavior was immediately classified as a bug.

For each potential issue, I considered:

- Is the behavior reproducible?
- What should the expected behavior be?
- Is there a clear validation rule?
- Does the behavior affect the user?
- Could the behavior be intentional?
- Can the issue be supported by the available requirements or application behavior?

This helped avoid reporting issues that could not be confirmed as genuine defects.

---

## 9. QA Techniques Used

The following manual testing techniques were applied:

- Functional Testing
- Exploratory Testing
- Positive Testing
- Negative Testing
- Boundary Value Analysis
- Input Validation Testing
- UI/Usability Testing
- Regression-oriented checks
- Defect Reproduction
- Defect Documentation

---

## 10. Test Results

Testing resulted in five confirmed defects.

The final execution statistics will be updated after completing execution of the full test suite.

| Metric | Result |
|---|---:|
| Confirmed Defects | 5 |
| Open Defects | 5 |
| Resolved Defects | 0 |
| Needs Validation | 0 |
| Test Cases Executed | TBD |
| Passed | TBD |
| Failed | TBD |
| Blocked | TBD |

---

## 11. Key Findings

The testing demonstrated several areas where input validation and UI consistency could be improved.

The most significant findings involved:

- Data consistency after document replacement.
- Input validation for Event names.
- Input validation for Template names.
- Handling of whitespace-only input.
- UI feedback for interactive controls.

These findings demonstrate the importance of testing not only the expected user flow but also invalid, boundary, and unexpected input.

---

## 12. Conclusion

This project provided practical experience in testing a complex web application with multiple interconnected features.

The testing process included planning test coverage, creating test cases, executing tests, performing exploratory testing, investigating unexpected behavior, reproducing defects, and documenting findings.

The project also reinforced the importance of distinguishing confirmed defects from expected behavior and requirement-dependent observations.

The final deliverables include:

- Test Plan
- Test Scenarios
- Test Cases
- Checklists
- Exploratory Testing Notes
- Test Execution Results
- Bug Reports
- Case Study
