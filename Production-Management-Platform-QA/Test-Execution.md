# Test Execution

## 1. Overview

This document summarizes the manual test execution performed for the Production Management Platform.

Testing focused on the main functional areas of the platform, including project management, director availability, production budget, invoice management, sales activities, cloud import, and UI behavior.

Testing included functional, negative, validation, exploratory, regression, and retesting activities.

---

## 2. Test Execution Summary

| Area                  |      Test Cases | Result / Finding                                             |
| --------------------- | --------------: | ------------------------------------------------------------ |
| Project Management    | TC-001 – TC-006 | Project details loading issue identified for one project     |
| Director Availability | TC-007 – TC-014 | Availability event creation issue identified and later fixed |
| Production Budget     | TC-015 – TC-023 | Budget calculation issue identified and later fixed          |
| Invoice Management    | TC-024 – TC-030 | Negative amount validation issue identified                  |
| Sales Activities      | TC-031 – TC-035 | Incorrect activity filtering identified in Meeting view      |
| Cloud Import / UI     | TC-036 – TC-039 | Button text visibility issue identified on hover             |
| Data Consistency      |          TC-040 | Save and refresh behavior checked                            |

---

## 3. Defects Identified

During test execution, 6 defects were documented.

| Bug ID  | Area                  | Severity | Status |
| ------- | --------------------- | -------- | ------ |
| BUG-001 | Director Availability | High     | Fixed  |
| BUG-002 | Project Management    | Medium   | Open   |
| BUG-003 | Production Budget     | High     | Fixed  |
| BUG-004 | Invoice Management    | Medium   | Open   |
| BUG-005 | Sales Activity        | Medium   | Open   |
| BUG-006 | UI / Usability        | Medium   | Open   |

### Defect Summary

* **BUG-001:** Event could not be added to Director Availability.
* **BUG-002:** Project Details failed to load for a specific project.
* **BUG-003:** Added expense was not correctly included in the budget total.
* **BUG-004:** Negative invoice amount displayed `[object Object]` instead of a readable validation message.
* **BUG-005:** Meeting Activity view displayed Call activities.
* **BUG-006:** Button text became unreadable on hover because of insufficient contrast.

---

## 4. Retesting Results

Retesting was performed for defects where a fix was available.

### BUG-001 — Director Availability

**Initial Result:** Failed

The event could not be added to Director Availability.

**Retest Result:** Passed

The issue was fixed and the availability event was successfully created during retesting.

---

### BUG-002 — Project Details

**Initial Result:** Failed

Project Details failed to load for one specific project, while other projects opened normally.

**Retest Result:** Failed

The issue remained reproducible during retesting.

**Status:** Open

---

### BUG-003 — Production Budget

**Initial Result:** Failed

An added expense was not correctly reflected in the Sub-total and Total Budget.

**Retest Result:** Passed

The issue was fixed. Valid budget values were calculated correctly and the expense was reflected in the budget totals.

---

### BUG-004 — Negative Invoice Amount

**Initial Result:** Failed

Entering a negative invoice amount resulted in `[object Object]` instead of a readable validation message.

**Retest Result:** Not documented

**Status:** Open

---

### BUG-005 — Meeting Activity Filtering

**Initial Result:** Failed

The Meeting view displayed both Meeting and Call activities instead of only Meeting activities.

**Retest Result:** Not documented

**Status:** Open

---

### BUG-006 — Button Text on Hover

**Initial Result:** Failed

The button text became difficult to read when the button was hovered because the text and background had insufficient contrast.

**Retest Result:** Not documented

**Status:** Open

---

## 5. Regression Testing

Regression testing was used to check that previously tested functionality continued to behave correctly after changes.

The main regression focus included:

* Project details loading
* Director Availability
* Production Budget calculations
* Invoice validation
* Sales Activity filtering
* UI behavior
* Data consistency after saving and refreshing

Issues that remained reproducible during retesting were kept open.

---

## 6. Exploratory Testing

Exploratory testing was also performed alongside the planned test cases.

The exploratory focus included:

* Unexpected input values
* Boundary and validation behavior
* Data consistency
* UI behavior
* Navigation between related areas
* Business logic
* Error messages
* Behavior after saving and refreshing

Exploratory findings were used to identify additional areas that required validation during structured testing.

---

## 7. Overall Execution Result

The execution identified functional, validation, business logic, filtering, and UI issues across several areas of the platform.

Some defects were successfully fixed and verified through retesting, while other defects remained reproducible or had no documented retest result.

### Final Defect Status

* **Total defects:** 6
* **Fixed and successfully retested:** 2
* **Still reproducible:** 1
* **Open with no documented retest:** 3

### Final Status

**Testing completed**

The documented defects and retesting results provide a record of the main issues found during manual testing of the Production Management Platform.

---

## 8. Related Documentation

* [Project Overview](Project-Overview.md)
* [Test Plan](Test-Plan.md)
* [Test Scenarios](Test-Scenarios.md)
* [Test Cases](Test-Cases.md)
* [Exploratory Testing](Exploratory-Testing.md)
* [Checklists](Checklists.md)
* [Bug Reports](Bug-Reports/README.md)
* [Case Study](Case-Study.md)
