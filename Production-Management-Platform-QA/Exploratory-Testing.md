# Exploratory Testing — Production Management Platform QA

## 1. Objective

Exploratory testing was performed to investigate application behavior beyond predefined test cases and identify unexpected functional, validation, business logic, data consistency, and UI usability issues.

The testing focused on related records, invalid inputs, boundary-style values, unexpected application behavior, and previously reported defects.

---

## 2. Areas Explored

### 2.1 Project Management

Explored:

* Opening projects from the Projects list
* Loading Project Details
* Project stage display
* Comparing similar project records
* Data consistency after navigation and refresh

**Finding:**

One specific project failed to load its Project Details while other projects opened successfully.

The issue was documented as **BUG-002** and remained reproducible during retesting.

---

### 2.2 Director Availability

Explored:

* Director selection
* Availability section
* Event creation
* Event status options
* Valid and invalid date ranges
* Optional fields

**Finding:**

An issue prevented an Availability Event from being added successfully.

The issue was documented as **BUG-001**.

The issue was later fixed and successfully retested.

---

### 2.3 Production Budget

Explored:

* Expense categories
* Expense values
* Prep and Days values
* Sub-total calculation
* Total Budget calculation
* Saving budget data
* Data consistency after refresh

**Finding:**

An added expense was initially not correctly reflected in the Budget Sub-total and Total Budget.

The issue was documented as **BUG-003**.

The issue was later fixed and successfully retested. The expense was correctly reflected in the budget totals after the fix.

---

### 2.4 Invoice Management

Explored:

* Invoice creation
* Required fields
* Negative invoice amounts
* Duplicate invoice numbers
* Decimal values
* Large monetary values

**Finding:**

Entering a negative invoice amount resulted in `[object Object]` instead of a readable validation message.

The issue was documented as **BUG-004**.

Additional checks were performed for duplicate invoice numbers and monetary values. No separate confirmed defect was created for these observations.

---

### 2.5 Sales Activities

Explored:

* Call activities
* Meeting activities
* Activity type filtering
* Activity counters
* Consistency between activity views

**Finding:**

The Call view displayed only Call activities, while the Meeting view displayed both Meeting and Call activities.

The issue was documented as **BUG-005**.

No retest result was documented for this issue.

---

### 2.6 Files / Cloud Import

Explored:

* Cloud Import navigation
* Settings navigation
* Action buttons
* Button normal state
* Button hover state

**Finding:**

An action button became difficult to read when hovered because the background changed to white while the text remained white.

The issue was documented as **BUG-006**.

No retest result was documented for this issue.

---

## 3. Exploratory Testing Techniques

The following techniques were used during exploratory testing:

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

---

## 4. Unexpected Behaviors Investigated

Several behaviors appeared unusual during testing and were investigated before deciding whether they represented confirmed defects.

These included:

* Crew count and Department assignment behavior
* Project stage display
* Scheduled follow-up and Task creation
* Invoice display behavior
* Report values and totals
* Similar project records
* Data consistency after refresh
* Cloud integration behavior

Where the behavior could not be confirmed as a defect, it was not reported as a separate bug.

This helped distinguish confirmed defects from expected behavior, configuration-related results, and observations that required further verification.

---

## 5. Key Findings

Exploratory testing contributed to the identification of six documented defects:

| Bug ID  | Area                  | Finding                                      | Status |
| ------- | --------------------- | -------------------------------------------- | ------ |
| BUG-001 | Director Availability | Event could not be added                     | Fixed  |
| BUG-002 | Project Management    | Project Details failed to load               | Open   |
| BUG-003 | Production Budget     | Expense was not correctly included in totals | Fixed  |
| BUG-004 | Invoice Management    | Negative amount displayed `[object Object]`  | Open   |
| BUG-005 | Sales Activity        | Meeting view displayed Call activities       | Open   |
| BUG-006 | UI / Usability        | Button text became unreadable on hover       | Open   |

---

## 6. Retesting

Previously reported issues were retested when a fix was available.

### Successfully Retested

* **BUG-001** — Director Availability Event creation
* **BUG-003** — Production Budget expense calculation

Both issues were fixed and successfully verified during retesting.

### Retested but Still Reproducible

* **BUG-002** — Project Details failed to load for a specific project

The issue remained reproducible during retesting and was kept open.

### No Retest Result Documented

* **BUG-004** — Negative invoice amount validation
* **BUG-005** — Meeting Activity filtering
* **BUG-006** — Button text on hover

These defects remain documented as open because no retest result was recorded.

---

## 7. Exploratory Testing Outcome

Exploratory testing provided additional coverage beyond the predefined test cases and helped identify defects across several application modules.

It was also used to investigate suspicious behavior before reporting it as a defect.

This helped avoid reporting observations that could not be confirmed as actual application issues.

---

## 8. Project Status

**Completed**

The documented exploratory testing activities and findings have been completed for the tested functionality.

The six identified defects are documented in the project's Bug Reports section, with their available retesting results recorded.

---

> All project names, data, and identifying information have been anonymized for portfolio purposes.
