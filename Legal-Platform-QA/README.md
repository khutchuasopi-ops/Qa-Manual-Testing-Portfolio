# Legal Platform — Manual QA Testing

## Project Overview

This project contains manual QA testing work for a confidential legal technology platform.

The platform includes features for managing legal documents, templates, events, workflows, repositories, search, and AI-assisted functionality.

The project has been anonymized for portfolio purposes.

---

## QA Role

**Junior Manual QA Tester**

The testing work included planning, test design, manual execution, exploratory testing, defect reporting, and validation of identified issues.

---

## Testing Scope

The main areas covered were:

* Dashboard
* Repository
* Documents
* File Upload and Replacement
* Templates
* Events
* Workflows
* AI Assistant
* Search and Filtering
* Recycle Bin
* Playbook Generation
* UI and Usability
* Data Consistency

---

## Testing Types

The following manual testing approaches were used:

* Functional Testing
* Negative Testing
* Boundary Value Testing
* Input Validation
* Exploratory Testing
* Regression Testing
* UI Testing
* Error Handling
* Data Consistency Testing
* Search and Filtering Testing

---

## QA Process

The testing process followed these main steps:

**Feature Understanding → Test Planning → Test Scenarios → Test Cases → Manual Execution → Exploratory Testing → Defect Reporting → Retesting → Regression Testing**

---

## Test Documentation

| Document                                      | Description                                         |
| --------------------------------------------- | --------------------------------------------------- |
| [Project Overview](Project-Overview.md)       | Project scope, objectives, and testing information  |
| [Test Plan](Test-Plan.md)                     | Testing scope, approach, environment, and criteria  |
| [Test Scenarios](Test-Scenarios.md)           | High-level scenarios covering the main features     |
| [Test Cases](Test-Cases.md)                   | Detailed manual test cases                          |
| [Test Execution](Test-Execution.md)           | Manual execution results and testing findings       |
| [Exploratory Testing](Exploratory-Testing.md) | Exploratory testing approach and findings           |
| [Checklists](Checklists.md)                   | Reusable checks for functional and negative testing |
| [Bug Reports](Bug-Reports/)                   | Documented defects with reproduction steps          |

---

## Main Testing Areas

### Documents and Files

Testing included:

* File upload
* File replacement
* File names
* File actions
* Data consistency after replacement
* Invalid file input

### Templates

Testing included:

* Template creation
* Template editing
* Template deletion
* Template name validation
* Empty input
* Long input values

### Events

Testing included:

* Event creation
* Event editing
* Event deletion
* Event name validation
* Boundary values
* Invalid input

### Search

Testing included:

* Valid search terms
* Partial search
* No results
* Empty search
* Clearing search
* Search result consistency

### AI Assistant

Testing included:

* User questions
* Follow-up questions
* Context handling
* Invalid or unclear requests
* Response behavior
* Error handling

### Playbook Generation

Testing included:

* Starting generation
* Generation flow
* Loading behavior
* Generated result
* Error handling

---

## Documented Defects

Five defects were documented during the testing work.

| Bug ID  | Area             | Summary                                        | Severity | Priority | Status |
| ------- | ---------------- | ---------------------------------------------- | -------- | -------- | ------ |
| BUG-001 | File Replacement | Old file name remains after replacement        | Medium   | Medium   | Open   |
| BUG-002 | Search           | Search cursor / clear behavior is inconsistent | Low      | Medium   | Open   |
| BUG-003 | Events           | Whitespace-only event name is accepted         | Medium   | High     | Open   |
| BUG-004 | Events           | Excessively long event name is accepted        | Medium   | Medium   | Open   |
| BUG-005 | Templates        | Excessively long template name is accepted     | Medium   | Medium   | Open   |

---

## Exploratory Testing Findings

Exploratory testing also identified findings that required additional investigation.

One example was an error observed during Playbook generation.

This was kept as an exploratory finding rather than being counted as a confirmed defect because further verification was needed.

This distinction was used to avoid treating every unexpected observation as a confirmed bug.

---

## Test Environment

| Item            | Details                                |
| --------------- | -------------------------------------- |
| Application     | Confidential Legal Technology Platform |
| Environment     | Staging                                |
| Platform        | Web                                    |
| Testing         | Manual QA                              |
| Browser         | Chrome                                 |
| Documentation   | Markdown                               |
| Version Control | GitHub                                 |

Exact browser versions and test dates were not recorded in the portfolio where they were not available.

---

## Out of Scope

The following areas were not part of this manual testing project:

* Source code testing
* Automated testing
* API testing
* Database testing
* Performance testing
* Load testing
* Security penetration testing
* Internal AI/model implementation

---

## QA Perspective

This project demonstrates practical experience with manual QA activities at a Junior level, including:

* Understanding application functionality
* Creating test scenarios
* Writing detailed test cases
* Performing functional testing
* Performing negative and boundary testing
* Exploratory testing
* Identifying reproducible defects
* Writing clear bug reports
* Retesting reported issues
* Planning regression checks
* Checking data consistency and usability

The focus is on practical manual testing and clear QA documentation rather than advanced automation or technical testing.

---

## Project Status

**Completed**

The project documentation contains the testing scope, test scenarios, test cases, execution information, exploratory findings, checklists, and documented defects.

---

## Confidentiality

The project has been anonymized for portfolio purposes.

No confidential application URLs, credentials, personal information, or sensitive business data are included.


