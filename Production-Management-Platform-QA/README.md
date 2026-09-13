# Production Management Platform — QA

## Overview

This project documents manual QA testing performed on an anonymized production management platform.

The testing focused on functional behavior, input validation, business logic, data consistency, and UI usability across different application areas.

The project demonstrates a structured manual QA approach including test execution, exploratory testing, defect identification, bug reporting, retesting, and regression testing.

> **Confidentiality Notice**
>
> All application names, project data, user information, and other identifying details have been anonymized for portfolio purposes.

## QA Role

**Junior Manual QA Tester**

The project was tested using manual testing techniques, with a focus on identifying reproducible issues and documenting them clearly.

## Testing Areas

* Project Management
* Director Availability
* Production Budget
* Invoice Management
* Sales Activities
* File Management
* Cloud Integrations
* UI and Usability

## Testing Approach

The following testing techniques were used:

* Functional Testing
* Exploratory Testing
* Regression Testing
* Retesting
* Negative Testing
* Boundary Testing
* Input Validation
* Data Validation
* Business Logic Validation
* UI / Usability Testing

## Documented Bug Reports

The project contains **6 documented defects** identified during manual testing.

| ID      | Area                  | Defect                                     |
| ------- | --------------------- | ------------------------------------------ |
| BUG-001 | Director Availability | Event cannot be added                      |
| BUG-002 | Project Management    | Project Details fail to load               |
| BUG-003 | Production Budget     | Expense not included in total              |
| BUG-004 | Invoice Management    | Negative amount displays `[object Object]` |
| BUG-005 | Sales Activity        | Meeting view displays Call activities      |
| BUG-006 | UI / Usability        | Button text becomes unreadable on hover    |

### Retesting

Retesting was performed for identified defects where a fix was available.

* **BUG-001** — Fixed and successfully retested
* **BUG-002** — Retested and remained reproducible
* **BUG-003** — Fixed and successfully retested
* **BUG-004** — No retest result documented
* **BUG-005** — No retest result documented
* **BUG-006** — No retest result documented

## Key QA Skills Demonstrated

* Writing clear and reproducible bug reports
* Identifying functional and usability defects
* Validating business logic and calculations
* Testing input validation and error handling
* Performing retesting after fixes
* Checking data consistency
* Performing exploratory testing across multiple modules
* Documenting test findings in a structured format
* Assigning defect severity and priority
* Analyzing user impact

## QA Workflow

The testing workflow followed this general process:

**Application Exploration → Test Scenario Identification → Manual Testing → Defect Identification → Reproduction → Bug Reporting → Retesting → Regression Testing → Final Review**

## Project Documentation

* [Project Overview](Project-Overview.md)
* [Test Plan](Test-Plan.md)
* [Test Scenarios](Test-Scenarios.md)
* [Test Cases](Test-Cases.md)
* [Test Execution](Test-Execution.md)
* [Exploratory Testing](Exploratory-Testing.md)
* [Checklists](Checklists.md)
* [Bug Reports](Bug-Reports/)

## Project Status

**Completed**

Manual testing, defect documentation, retesting, and regression activities included in this portfolio project have been completed.

## Confidentiality

This project intentionally excludes:

* Original application name
* Company name
* Application URL
* User credentials
* Personal information
* Confidential business information
* Identifying screenshots or production data

All project names, data, and identifying information have been anonymized for portfolio purposes.
