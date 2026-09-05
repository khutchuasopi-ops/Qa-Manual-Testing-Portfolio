# Test Scenarios — Production Management Platform QA

## 1. Project Management

* Verify that projects can be opened successfully.
* Verify that project details load correctly.
* Verify project stage information.
* Verify that project-related information is displayed consistently.

## 2. Director Availability

* Verify that a Director Availability event can be created.
* Verify available event statuses.
* Verify start and end date validation.
* Verify that invalid date ranges are rejected.
* Verify optional project and notes fields.
* Retest previously reported event creation issues.

## 3. Production Budget

* Verify that expense items can be added.
* Verify that Prep and Days values are processed correctly.
* Verify Sub-total calculations.
* Verify Total Budget calculations.
* Verify that expense values are reflected in the overall budget.

## 4. Invoice Management

* Verify invoice creation with valid data.
* Verify required field validation.
* Verify negative amount validation.
* Verify that validation errors are displayed as readable messages.
* Verify duplicate invoice number validation.
* Verify invoice data is saved correctly.

## 5. Sales Activities

* Verify Call activities.
* Verify Meeting activities.
* Verify activity type filtering.
* Verify that the selected activity type displays the correct activities.
* Verify activity counters and displayed records.

## 6. File Management / Cloud Import

* Verify access to Cloud Import.
* Verify navigation to Cloud integration settings.
* Verify action button behavior.
* Verify normal and hover states.
* Verify text readability and visual contrast.

## 7. Cross-Module Validation

* Verify consistency of data between related modules.
* Verify that calculations and displayed values remain synchronized.
* Verify that changes are reflected after saving and refreshing.
* Verify error handling across different modules.

## 8. Regression Scenarios

* Retest previously fixed Director Availability functionality.
* Retest Production Budget calculations after changes.
* Verify that fixes do not introduce new issues in related functionality.

## 9. Exploratory Scenarios

* Explore boundary values.
* Test invalid and unexpected input.
* Check UI behavior during hover and interaction states.
* Compare similar records for inconsistent behavior.
* Investigate unexpected application responses.
