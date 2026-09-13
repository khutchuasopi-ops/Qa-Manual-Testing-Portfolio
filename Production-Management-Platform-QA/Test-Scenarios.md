# Test Scenarios — Production Management Platform QA

## 1. Project Management

| ID     | Test Scenario                                                                 |
| ------ | ----------------------------------------------------------------------------- |
| TS-001 | Verify that available projects can be opened successfully.                    |
| TS-002 | Verify that Project Details load correctly for a valid project.               |
| TS-003 | Verify that project stage information is displayed correctly.                 |
| TS-004 | Verify that project-related information is displayed consistently.            |
| TS-005 | Verify that a project with valid data can be accessed without loading errors. |

## 2. Director Availability

| ID     | Test Scenario                                                                |
| ------ | ---------------------------------------------------------------------------- |
| TS-006 | Verify that a Director Availability event can be created with valid data.    |
| TS-007 | Verify that available event statuses can be selected correctly.              |
| TS-008 | Verify that valid start and end dates are accepted.                          |
| TS-009 | Verify that invalid date ranges are rejected.                                |
| TS-010 | Verify that optional project and notes fields can be used correctly.         |
| TS-011 | Verify that an existing Director Availability event can be viewed correctly. |
| TS-012 | Retest previously reported Director Availability event creation issues.      |

## 3. Production Budget

| ID     | Test Scenario                                                                   |
| ------ | ------------------------------------------------------------------------------- |
| TS-013 | Verify that expense items can be added to a production budget.                  |
| TS-014 | Verify that valid expense values are accepted.                                  |
| TS-015 | Verify that Prep and Days values are processed correctly.                       |
| TS-016 | Verify that Sub-total is calculated correctly after adding expenses.            |
| TS-017 | Verify that Total Budget is calculated correctly.                               |
| TS-018 | Verify that added expense values are reflected in the overall budget.           |
| TS-019 | Verify that budget values remain correct after saving and reopening the budget. |

## 4. Invoice Management

| ID     | Test Scenario                                                                |
| ------ | ---------------------------------------------------------------------------- |
| TS-020 | Verify that an invoice can be created with valid data.                       |
| TS-021 | Verify that required invoice fields are validated.                           |
| TS-022 | Verify that negative invoice amounts are rejected.                           |
| TS-023 | Verify that validation errors are displayed as readable messages.            |
| TS-024 | Verify that duplicate invoice numbers are handled correctly.                 |
| TS-025 | Verify that valid invoice data is saved correctly.                           |
| TS-026 | Verify that invoice information remains correct after reopening the invoice. |

## 5. Sales Activities

| ID     | Test Scenario                                                                               |
| ------ | ------------------------------------------------------------------------------------------- |
| TS-027 | Verify that Call activities are displayed correctly.                                        |
| TS-028 | Verify that Meeting activities are displayed correctly.                                     |
| TS-029 | Verify that activity type filtering works correctly.                                        |
| TS-030 | Verify that the selected activity type displays only relevant activities.                   |
| TS-031 | Verify that activity counters match the displayed records.                                  |
| TS-032 | Verify that activity information remains consistent when navigating between activity views. |

## 6. File Management / Cloud Import

| ID     | Test Scenario                                                              |
| ------ | -------------------------------------------------------------------------- |
| TS-033 | Verify that the Cloud Import functionality can be accessed.                |
| TS-034 | Verify that the user can navigate to Cloud integration settings.           |
| TS-035 | Verify that the relevant action button is displayed correctly.             |
| TS-036 | Verify that the action button behaves correctly during normal interaction. |
| TS-037 | Verify that the button displays an appropriate hover state.                |
| TS-038 | Verify that button text remains readable in the hover state.               |
| TS-039 | Verify that UI elements provide clear visual feedback during interaction.  |

## 7. Cross-Module Validation

| ID     | Test Scenario                                                                              |
| ------ | ------------------------------------------------------------------------------------------ |
| TS-040 | Verify that related data remains consistent between application modules.                   |
| TS-041 | Verify that calculated values remain synchronized with displayed data.                     |
| TS-042 | Verify that saved changes are reflected after refreshing or reopening the relevant page.   |
| TS-043 | Verify that related module data is not incorrectly changed by an action in another module. |
| TS-044 | Verify that validation and error handling behave consistently across different modules.    |

## 8. Regression Scenarios

| ID     | Test Scenario                                                                       |
| ------ | ----------------------------------------------------------------------------------- |
| TS-045 | Retest the Director Availability event creation functionality after a fix.          |
| TS-046 | Retest Production Budget calculations after a fix.                                  |
| TS-047 | Verify that previously fixed functionality remains working after related changes.   |
| TS-048 | Verify that changes in one module do not introduce issues in related functionality. |

## 9. Exploratory Scenarios

| ID     | Test Scenario                                                              |
| ------ | -------------------------------------------------------------------------- |
| TS-049 | Explore boundary values in fields that accept numeric or text input.       |
| TS-050 | Test invalid and unexpected input in relevant forms.                       |
| TS-051 | Check UI behavior during hover and other interaction states.               |
| TS-052 | Compare similar records or views for inconsistent behavior.                |
| TS-053 | Investigate unexpected validation or error responses.                      |
| TS-054 | Explore application behavior after saving, refreshing, and reopening data. |
| TS-055 | Check whether displayed data remains consistent after common user actions. |

## Scenario Coverage

The scenarios cover:

* Project Management
* Director Availability
* Production Budget
* Invoice Management
* Sales Activities
* File Management
* Cloud Integrations
* UI / Usability
* Cross-Module Validation
* Regression Testing
* Exploratory Testing
