# QA Case Study — Production Management Platform

## Project Overview

This case study presents manual QA testing performed on an anonymized production management platform.

The testing covered multiple modules and focused on identifying real functional, business logic, validation, data consistency, and UI usability issues.

## Testing Approach

Testing was performed using a combination of:

* Functional Testing
* Exploratory Testing
* Negative Testing
* Boundary Testing
* Regression Testing
* Retesting
* Data Validation
* Business Logic Validation
* UI / Usability Testing

## Key Defects Identified

### 1. Director Availability Event

An issue prevented Availability Events from being added successfully.

The issue was reported, fixed, and successfully retested.

**QA focus:** Functional testing and regression testing.

### 2. Project Details Loading

A specific project failed to load its Project Details while other projects opened successfully.

The issue remained reproducible during retesting.

**QA focus:** Functional testing and data/loading investigation.

### 3. Production Budget Calculation

Expenses were initially not correctly reflected in the Budget Sub-total and Total Budget.

The issue was fixed and successfully retested after valid budget values were entered.

**QA focus:** Business logic and calculation validation.

### 4. Invoice Validation

Entering a negative invoice amount resulted in `[object Object]` instead of a readable validation message.

**QA focus:** Negative testing and error handling.

### 5. Sales Activity Filtering

The Meeting activity view displayed both Meeting and Call activities instead of only the selected activity type.

**QA focus:** Data filtering and consistency testing.

### 6. Hover Contrast

A button's hover state changed the background to white while keeping the text white, making the text practically unreadable.

**QA focus:** UI, usability, and accessibility.

## QA Challenges

During testing, several behaviors initially appeared suspicious but were not confirmed as defects after further investigation.

This included checking:

* Crew counts and department assignments
* Project stages
* Scheduled follow-ups and task creation
* Invoice display states
* Report values
* Similar project records
* Data consistency after refresh

These investigations helped distinguish actual defects from expected application behavior or configuration-related results.

## Retesting

Previously reported issues were retested after fixes where applicable.

Confirmed successful fixes included:

* Director Availability Event creation
* Production Budget expense calculation

Retesting helped verify that fixes resolved the original issues without relying only on developer confirmation.

## Key QA Skills Demonstrated

* Defect identification
* Bug reproduction
* Clear bug documentation
* Severity assessment
* Exploratory investigation
* Negative testing
* Business logic validation
* Regression testing
* Retesting
* Data consistency analysis
* UI and usability evaluation

## Outcome

The testing identified six verified defects across different application areas.

The project remains ongoing, allowing additional verified findings to be added as testing continues.

> All project names, data, and identifying information have been anonymized for portfolio purposes.
