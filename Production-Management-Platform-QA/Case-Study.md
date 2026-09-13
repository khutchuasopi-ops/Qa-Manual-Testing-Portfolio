# QA Case Study — Production Management Platform

## 1. Project Overview

This case study presents manual QA testing performed on an anonymized production management platform.

The testing covered multiple application modules and focused on identifying functional, business logic, validation, data consistency, and UI usability issues.

The testing process included planned test cases, exploratory testing, defect reporting, retesting, and regression checks.

---

## 2. Testing Approach

Testing was performed using a combination of:

* Functional Testing
* Exploratory Testing
* Negative Testing
* Boundary Testing
* Regression Testing
* Retesting
* Input Validation
* Data Validation
* Business Logic Validation
* UI / Usability Testing

The testing approach combined predefined test cases with exploratory investigation of unexpected application behavior.

---

## 3. Key Defects Identified

### 3.1 Director Availability Event

An issue prevented Availability Events from being added successfully.

The issue was documented as **BUG-001**, fixed, and successfully retested.

**QA focus:** Functional testing and regression testing.

---

### 3.2 Project Details Loading

A specific project failed to load its Project Details while other projects opened successfully.

The issue was documented as **BUG-002** and remained reproducible during retesting.

**QA focus:** Functional testing and data/loading investigation.

---

### 3.3 Production Budget Calculation

An added expense was initially not correctly reflected in the Budget Sub-total and Total Budget.

The issue was documented as **BUG-003**, fixed, and successfully retested.

**QA focus:** Business logic and calculation validation.

---

### 3.4 Invoice Validation

Entering a negative invoice amount resulted in `[object Object]` instead of a readable validation message.

The issue was documented as **BUG-004**.

**QA focus:** Negative testing, input validation, and error handling.

---

### 3.5 Sales Activity Filtering

The Meeting activity view displayed both Meeting and Call activities instead of only the selected activity type.

The issue was documented as **BUG-005**.

**QA focus:** Data filtering and consistency testing.

---

### 3.6 Hover Contrast

A button's hover state changed the background to white while the text remained white, making the text difficult to read.

The issue was documented as **BUG-006**.

**QA focus:** UI, usability, and accessibility.

---

## 4. QA Challenges

During testing, several behaviors initially appeared suspicious but were not confirmed as defects after further investigation.

The investigation included:

* Crew counts and department assignments
* Project stages
* Scheduled follow-ups and task creation
* Invoice display behavior
* Report values and totals
* Similar project records
* Data consistency after refresh
* Cloud integration behavior

Where a behavior could not be confirmed as a defect, it was not reported as a separate bug.

This helped distinguish confirmed defects from expected behavior, configuration-related results, and observations requiring further verification.

---

## 5. Retesting

Previously reported issues were retested when a fix was available.

### Successfully Retested

* **BUG-001** — Director Availability Event creation
* **BUG-003** — Production Budget expense calculation

Both issues were fixed and successfully verified during retesting.

### Still Reproducible

* **BUG-002** — Project Details failed to load for a specific project

The issue remained reproducible during retesting and was kept open.

### No Retest Result Documented

* **BUG-004** — Negative invoice amount validation
* **BUG-005** — Meeting Activity filtering
* **BUG-006** — Button text on hover

These defects remain documented as open because no retest result was recorded.

---

## 6. Key QA Skills Demonstrated

* Defect identification
* Bug reproduction
* Clear bug documentation
* Severity assessment
* Exploratory investigation
* Negative testing
* Input validation
* Business logic validation
* Regression testing
* Retesting
* Data consistency checking
* UI and usability evaluation

---

## 7. Outcome

The testing identified and documented **six defects** across different application areas.

| Status                          | Number |
| ------------------------------- | -----: |
| Fixed and successfully retested |      2 |
| Still reproducible              |      1 |
| Open with no documented retest  |      3 |
| **Total**                       |  **6** |

The documented results provide a record of the main issues found during manual testing and the retesting performed where fixes were available.

---

## 8. Project Status

**Completed**

The documented testing activities for the tested functionality have been completed.

All identified defects are documented in the project's Bug Reports section, together with the available retesting results.

---

> All project names, data, and identifying information have been anonymized for portfolio purposes.
