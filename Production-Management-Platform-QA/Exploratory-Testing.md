# Exploratory Testing — Production Management Platform QA

## Objective

Exploratory testing was performed to investigate application behavior beyond predefined test cases and identify unexpected functional, validation, business logic, data consistency, and UI usability issues.

The testing focused on comparing related records, testing invalid inputs, checking boundary-style values, investigating unexpected behavior, and retesting previously reported issues.

## Areas Explored

### 1. Project Management

Explored project opening, Project Details loading, project stages, similar project records, and data consistency after navigation and refresh.

**Finding:**

One specific project failed to load its Project Details while other projects opened successfully.

The issue was documented as **BUG-002**.

---

### 2. Director Availability

Explored Director selection, Availability, Event creation, Event statuses, date ranges, optional fields, and invalid date combinations.

**Finding:**

An issue prevented an Availability Event from being added successfully.

The issue was documented as **BUG-001**, fixed, and successfully retested.

---

### 3. Production Budget

Explored expense categories, expense values, Prep and Days values, Sub-total, Total Budget, saving, and data consistency after refresh.

**Finding:**

An expense was initially not correctly reflected in the Budget Sub-total and Total Budget calculations.

The issue was documented as **BUG-003**, fixed, and successfully retested.

---

### 4. Invoice Management

Explored invoice creation, required fields, negative values, duplicate invoice numbers, decimal precision, and large monetary values.

**Finding:**

Entering a negative invoice amount resulted in `[object Object]` instead of a readable validation message.

The issue was documented as **BUG-004**.

Additional validation checks were performed for duplicate invoice numbers and monetary values. No separate confirmed defect was created for these observations.

---

### 5. Sales Activities

Explored Call and Meeting activities, activity type filtering, activity counters, and consistency between different activity views.

**Finding:**

The Call view displayed only Call activities, while the Meeting view displayed both Meeting and Call activities.

The issue was documented as **BUG-005**.

---

### 6. Files / Cloud Import

Explored Cloud Import navigation, Settings navigation, action buttons, and button interaction states.

**Finding:**

An action button became difficult to read when hovered because the background changed to white while the text remained white.

The issue was documented as **BUG-006**.

---

## Exploratory Testing Techniques

The following exploratory techniques were used:

* Comparing similar records
* Comparing different activity types
* Testing valid and invalid input
* Testing negative values
* Testing boundary-style monetary values
* Checking calculation results
* Checking data after save and refresh
* Investigating unexpected application responses
* Checking UI interaction states
* Verifying validation messages
* Retesting previously reported defects
* Cross-checking related application data

## Unexpected Behaviors Investigated

Several behaviors initially appeared suspicious and were investigated further before deciding whether they represented defects.

These included:

* Crew count and Department assignment behavior
* Project stage display
* Scheduled follow-up and Task creation
* Invoice display state
* Report values and totals
* Similar project records
* Data consistency after refresh
* Cloud integration behavior

Where the behavior could not be confirmed as a defect, it was not reported as a bug.

This approach helped distinguish confirmed defects from expected behavior, configuration-related results, and unverified observations.

## Key Findings

Exploratory testing contributed to the identification of six verified defects:

| ID      | Area                  | Finding                                      |
| ------- | --------------------- | -------------------------------------------- |
| BUG-001 | Director Availability | Event could not be added                     |
| BUG-002 | Project Management    | Project Details failed to load               |
| BUG-003 | Production Budget     | Expense was not included correctly in totals |
| BUG-004 | Invoice Management    | Negative amount displayed `[object Object]`  |
| BUG-005 | Sales Activity        | Meeting view displayed Call activities       |
| BUG-006 | UI / Usability        | Button text became unreadable on hover       |

## Retesting

Previously reported issues were retested after fixes where applicable.

Confirmed successful fixes included:

* Director Availability Event creation
* Production Budget expense calculation

Retesting was used to verify the original issue after the fix rather than relying only on a developer confirmation.

## Exploratory Testing Outcome

Exploratory testing provided additional coverage beyond predefined test cases and helped identify defects across different application modules.

The testing also helped eliminate false positives by investigating suspicious behavior before documenting it as a defect.

## Project Status

This is an ongoing QA project.

Additional exploratory testing, verified findings, and regression scenarios may be added as new functionality becomes available.

> All project names, data, and identifying information have been anonymized for portfolio purposes.
