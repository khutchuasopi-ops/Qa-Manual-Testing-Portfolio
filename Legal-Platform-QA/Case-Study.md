# Case Study – Legal Platform Manual Testing

## 1. Project Overview

This case study covers manual QA testing of a confidential legal technology platform.

The main goal was to verify the functionality, input validation, search behavior, file handling, and data consistency of the platform from a user's perspective.

Testing focused on identifying functional issues, validating expected behavior, and documenting confirmed defects.

---

## 2. Testing Scope

The following areas were included in the testing scope:

- Dashboard
- Repository
- Documents
- File Upload
- File Replacement
- Templates
- Events
- Workflows
- AI Assistant
- Search
- Recycle Bin
- General Input Validation
- Playbook Generation

---

## 3. Testing Approach

The testing was performed manually using documented test scenarios, test cases, checklists, and exploratory testing.

The following testing techniques were used:

- Functional Testing
- Positive Testing
- Negative Testing
- Boundary Value Testing
- Input Validation
- UI Testing
- Exploratory Testing
- Regression Testing
- Error Handling
- Data Consistency Testing
- Search and Filtering Testing

The main focus was on verifying expected user behavior and identifying issues that could affect functionality, data consistency, usability, or validation.

---

## 4. Test Environment

| Item | Details |
|---|---|
| Environment | Staging |
| Browser | Google Chrome |
| Testing Type | Manual QA |
| Documentation | Markdown |
| Repository | GitHub |

---

## 5. Test Documentation

The project contains:

- Test Plan
- Test Scenarios
- Test Cases
- Checklists
- Exploratory Testing Notes
- Test Execution
- Bug Reports
- Case Study
- Project Overview

A total of **60 test cases** were documented and executed.

---

## 6. Test Execution Summary

All 60 documented test cases were executed.

| Result | Count |
|---|---:|
| PASS | 55 |
| FAIL | 5 |
| BLOCKED | 0 |
| Total | 60 |

### Execution Result

- **55 test cases passed**
- **5 test cases failed**
- **0 test cases were blocked**
- **60 test cases were executed in total**

The five failed test cases were associated with the five confirmed defects documented in the project.

---

## 7. Failed Test Cases and Defect Traceability

| Test Case | Result | Related Bug | Area |
|---|---|---|---|
| TC-REP-003 | FAIL | BUG-001 | File Replacement |
| TC-SEARCH-003 | FAIL | BUG-002 | Search |
| TC-EVENT-003 | FAIL | BUG-003 | Events |
| TC-EVENT-005 | FAIL | BUG-004 | Events |
| TC-TEMP-004 | FAIL | BUG-005 | Templates |

---

## 8. Confirmed Defects

During execution, five confirmed defects were documented.

### BUG-001 — File Replacement

After replacing an existing file, the old file name remained visible instead of being updated to the new file name.

**Severity:** Medium  
**Priority:** Medium

This issue can create confusion about which file is currently stored in the system.

---

### BUG-002 — Search

Search cursor and clear behavior were inconsistent during search interaction.

**Severity:** Low  
**Priority:** Medium

The issue affects the usability of the search functionality.

---

### BUG-003 — Events

The Events form accepted a whitespace-only name.

**Severity:** Medium  
**Priority:** High

A whitespace-only value should not be accepted as a valid event name.

---

### BUG-004 — Events

The Events form accepted an excessively long event name.

**Severity:** Medium  
**Priority:** Medium

The input should have an appropriate validation rule or maximum length.

---

### BUG-005 — Templates

The Templates form accepted an excessively long template name.

**Severity:** Medium  
**Priority:** Medium

The input should have an appropriate validation rule or maximum length.

---

## 9. Defect Summary

| Severity | Number of Defects |
|---|---:|
| Critical | 0 |
| High | 0 |
| Medium | 4 |
| Low | 1 |
| **Total** | **5** |

### Priority Summary

| Priority | Number of Defects |
|---|---:|
| High | 1 |
| Medium | 4 |
| Low | 0 |
| **Total** | **5** |

All five documented defects remained open at the time of this test documentation.

---

## 10. Key Testing Findings

The testing identified issues in several different areas of the platform.

The main findings were related to:

- Data consistency after file replacement
- Search interaction and usability
- Input validation
- Boundary value handling
- Event name validation
- Template name validation

The findings show the importance of validating both normal user input and invalid or boundary-value input.

---

## 11. QA Activities Demonstrated

This project demonstrates practical experience with:

- Reviewing application functionality
- Creating test scenarios
- Designing detailed test cases
- Executing manual tests
- Performing positive and negative testing
- Performing boundary value testing
- Performing exploratory testing
- Performing regression testing
- Identifying functional defects
- Documenting bugs with clear reproduction information
- Assigning severity and priority
- Maintaining defect traceability
- Summarizing test execution results

---

## 12. Conclusion

The Legal Platform testing cycle covered **60 documented and executed test cases**.

The final execution result was:

- **55 PASS**
- **5 FAIL**
- **0 BLOCKED**

Five confirmed defects were identified and documented.

The testing provided coverage across core platform functionality, file handling, search, events, templates, validation, and data consistency.

This project demonstrates a practical manual QA workflow from test planning and test case design through execution, defect reporting, and final test summary.
