# Exploratory Testing — Legal Platform

## 1. Overview

Exploratory testing was used to check the application beyond the predefined test cases.

The main focus was on user behavior, invalid input, boundary values, file replacement, template creation, and Playbook generation.

During the sessions, unexpected behavior was investigated and the findings were checked to determine whether they were defects or expected behavior.

---

## 2. QA Role

**Role:** Junior Manual QA Tester

Exploratory testing was performed manually by using the application and following realistic user flows.

The testing focused on:

* Trying different inputs
* Checking invalid and empty values
* Testing long names
* Changing uploaded files
* Checking the result after actions
* Looking for inconsistencies between the expected and actual behavior
* Rechecking unexpected results

---

## 3. Exploratory Session 01 — Templates and File Upload

### Objective

Explore template creation and document upload functionality.

### Focus Areas

* Template creation
* File upload
* File replacement
* Input validation
* Long names
* Empty input
* Playbook generation

### Session Notes

During the session, the main user flows were explored first.

Additional negative and boundary cases were then tested to check how the application handles unexpected or invalid input.

---

## 4. File Replacement

### Action

An existing document was selected and replaced with another file.

### Observation

The file replacement action completed, but the displayed file name did not update correctly.

The stored file changed, while the old file name remained visible.

### Result

This behavior was treated as a defect because the displayed information did not match the replaced file.

### Related Bug

**BUG-001 — Old File Name Remains After Replacement**

**Severity:** Medium
**Priority:** Medium
**Status:** Open

---

## 5. Playbook Generation

### Action

A Playbook generation process was started using the available functionality.

### Observation

The generation process started, but an error was returned after the action was initiated.

### Result

The behavior was recorded as an issue because the expected Playbook generation process did not complete successfully.

### Finding

Further verification is required to determine the exact conditions under which the error occurs.

---

## 6. Long Template Names

### Action

A very long name was entered when creating a template.

### Observation

The application accepted the long template name.

### Result

The behavior was considered a validation issue because there was no clear maximum length restriction.

### Related Bug

**BUG-005 — Excessively Long Template Name Accepted**

**Severity:** Medium
**Priority:** Medium
**Status:** Open

---

## 7. Empty Template Name

### Action

A template was created without entering a name.

### Observation

The application allowed template creation without a name.

### Result

This behavior was treated as a validation issue because a template should have a valid name before it is created.

### Finding

The name field should validate empty input and prevent creation when the required value is missing.

---

## 8. Additional Negative Testing

During the exploratory session, attention was also given to invalid and unexpected input.

The following areas were checked:

* Empty values
* Very long values
* File replacement
* Missing template name
* Unexpected results after actions
* Error handling during Playbook generation

The purpose was to find issues that may not be visible during the normal happy path.

---

## 9. Findings

The exploratory session resulted in the following findings:

| Area                | Finding                                          | Result           |
| ------------------- | ------------------------------------------------ | ---------------- |
| File Replacement    | Old file name remained visible after replacement | Confirmed defect |
| Playbook Generation | Error appeared after starting generation         | Issue identified |
| Template Name       | Very long name was accepted                      | Confirmed defect |
| Template Creation   | Template could be created without a name         | Validation issue |

---

## 10. Defect Validation

Each unexpected behavior was reviewed before being treated as a defect.

The following points were considered:

* Could the issue be reproduced?
* Was the behavior different from the expected result?
* Was the behavior related to input validation?
* Could the issue affect the user flow?
* Was the behavior a defect or only a usability concern?

Only validated findings were included in the Bug Reports section.

---

## 11. Exploratory Testing Approach

The exploratory testing process was:

**Explore → Observe → Investigate → Reproduce → Validate → Report**

This approach helped identify issues that were not limited to the normal successful user flow.

---

## 12. Main Findings

The main issues identified during exploratory testing were related to:

* File replacement and displayed data
* Input validation
* Empty required fields
* Long input values
* Playbook generation error handling

These findings were then used to create or support the related bug reports.

---

## 13. Limitations

The exploratory testing was performed manually within the available application environment.

The following areas were outside the scope of this testing:

* Source code review
* Automated testing
* API testing
* Database testing
* Performance and load testing
* Security penetration testing
* Internal AI/model implementation

---

## 14. Conclusion

Exploratory testing helped identify several issues that could affect normal user interaction with the platform.

The session focused on realistic user actions, invalid input, boundary values, file replacement, template creation, and Playbook generation.

The identified findings were validated and documented where appropriate.

This demonstrates practical use of exploratory testing as part of a Junior Manual QA workflow.

