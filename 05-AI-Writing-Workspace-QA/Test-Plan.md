# Test Plan — AI Writing Workspace QA

## 1. Document Overview

**Project:** AI Writing Workspace
**Testing Type:** Manual QA Testing
**Tester Level:** Junior Manual QA Tester
**Environment:** Staging / Preview
**Production Testing:** Not included

---

## 2. Objective

The objective of this testing is to verify the main functionality of the AI Writing Workspace and identify functional, usability, persistence, navigation, and AI workflow issues.

The testing focuses on how the application behaves during normal user workflows, as well as selected negative and exploratory scenarios.

---

## 3. Scope

The following areas are included in the testing scope:

* Board
* Draft creation and editing
* Draft persistence
* Draft Editor text input
* AI Assistant
* AI Chat
* Plan
* Library
* Templates
* Poster / Cover
* Split View
* Project / Manuscript details
* Navigation
* UI / UX
* Data persistence
* AI workflows
* AI context and conversation state

---

## 4. Testing Approach

The following manual testing approaches were used:

### Functional Testing

Verify that the main features work according to their expected behavior.

Examples include:

* Creating and opening Drafts
* Editing Draft content
* Creating Plan content
* Using AI Assistant functionality
* Working with Posters / Covers
* Navigating between workspace areas

### Exploratory Testing

Explore the application beyond predefined test steps to identify unexpected behavior, inconsistent states, and usability problems.

### Smoke Testing

Perform basic checks of the main workspace areas to confirm that the application is usable before deeper testing.

### Regression Testing

Recheck relevant functionality after changes or fixes where applicable.

### Negative Testing

Test invalid, unexpected, or problematic user actions and observe how the application responds.

### User-Flow Testing

Test complete workflows from the user's perspective, including navigation between related workspace areas.

### UI / UX Testing

Check interface behavior, visibility, usability, and interaction feedback.

### Persistence Testing

Check whether created or edited content remains available after actions such as refreshing or navigating between pages.

### AI Workflow Testing

Check AI-related workflows, including:

* AI-generated content
* AI Assistant interaction
* AI Chat
* Writing AI-generated content into Drafts
* Plan generation and synchronization

### Context / State Testing

Check whether the application maintains the correct state and conversation context when switching between Drafts, Projects, Chats, and other workspace areas.

---

## 5. Test Environment

Testing was performed in the **staging / preview environment**.

Production was not included in the testing scope.

Testing was performed through a web browser using the available AI Writing Workspace interface.

---

## 6. Test Data

Test data included:

* New and existing Drafts
* Project / Manuscript content
* AI-generated content
* AI Chat conversations
* Plan content
* Template elements
* Poster / Cover images
* Workspace navigation states

Where applicable, existing test data was reused to verify persistence and context behavior.

---

## 7. Entry Criteria

Testing can begin when:

* The staging / preview environment is accessible.
* The main workspace can be opened.
* Required test areas are available.
* Test data can be created or accessed.
* The application is sufficiently stable for manual testing.

---

## 8. Exit Criteria

Testing can be considered complete when:

* The planned test cases have been executed.
* Observed failures have been documented.
* Confirmed defects have been recorded as bug reports.
* Behaviors requiring product clarification have been identified separately.
* UX recommendations have been documented where appropriate.
* The final test documentation reflects the actual testing results.

---

## 9. Test Case Coverage

A total of **28 test cases** are included in the project test suite.

| Area                    | Covered Test Cases |
| ----------------------- | ------------------ |
| Board                   | TC-001 – TC-004    |
| Draft                   | TC-005 – TC-011    |
| Plan                    | TC-012 – TC-015    |
| Library                 | TC-016 – TC-017    |
| Templates               | TC-018, TC-025     |
| Poster / Cover          | TC-019 – TC-021    |
| AI Chat                 | TC-022             |
| Project / Manuscript    | TC-023 – TC-024    |
| Split View              | TC-026             |
| Navigation / General UI | TC-027 – TC-028    |

---

## 10. Test Results Summary

The current test execution contains:

| Result                        |  Count |
| ----------------------------- | -----: |
| PASS                          |     12 |
| FAIL                          |     11 |
| Requires Product Confirmation |      4 |
| UX Recommendation Only        |      1 |
| **Total**                     | **28** |

The test results identified **9 confirmed bugs** and **2 UX recommendations**.

Four observations were separated from confirmed defects because the expected product behavior requires clarification.

---

## 11. Defect Categories

The identified issues cover several areas:

* Data persistence
* Draft editing
* AI-generated content
* AI conversation context
* Plan synchronization
* Poster saving
* Image upload state
* Chat state
* Split View pagination
* UI / UX

---

## 12. Product Confirmation Items

The following behaviors require product clarification before being classified as confirmed defects:

* **TC-004** — Board item deletion behavior
* **TC-005** — Draft initial loading behavior
* **TC-023** — Conversation availability after Project deletion
* **TC-025** — Horizontal Template content behavior

These observations are intentionally kept separate from the confirmed bug count.

---

## 13. Confirmed Defects

The project contains the following confirmed defects:

| Bug ID  | Description                                                 | Related Test Case(s) |
| ------- | ----------------------------------------------------------- | -------------------- |
| BUG-001 | Draft content lost after refresh                            | TC-009               |
| BUG-002 | Draft Editor lowercase automatically uppercase              | TC-008               |
| BUG-003 | AI Assistant fails to write into editable Draft             | TC-010               |
| BUG-004 | New Draft retains previous independent conversation context | TC-011               |
| BUG-005 | AI-generated Plan content not reflected on Plan page        | TC-014, TC-015       |
| BUG-006 | Save Poster action delayed/unresponsive                     | TC-020               |
| BUG-007 | Upload dialog shows previous image                          | TC-021               |
| BUG-008 | New Chat temporarily shows previous conversation            | TC-022               |
| BUG-009 | Split View pagination/page breaks duplicated/reset          | TC-026               |

---

## 14. UX Recommendations

Two UX recommendations were identified:

### UX-001 — Grab Cursor for Draggable Template Elements

A grab cursor would provide clearer visual feedback that Template elements can be dragged.

### UX-002 — Close Button for Project / Manuscript Details

A visible Close (X) button would make closing the details panel clearer and more convenient.

---

## 15. Risks and Limitations

The following limitations apply to this test cycle:

* Testing was performed in the staging / preview environment.
* Production behavior was not tested.
* Some observed behaviors require product clarification before they can be considered defects.
* AI-generated results can vary depending on context and input.
* Not every observed issue has a corresponding confirmed bug report.
* No assumptions are made about undocumented product behavior.

---

## 16. Deliverables

The project testing documentation includes:

* Project Overview
* Test Plan
* Test Scenarios
* Test Cases
* Checklists
* Bug Reports
* UX Recommendations

---

## 17. Final Status

**Testing Status:** Completed

**Total Test Cases:** 28
**PASS:** 12
**FAIL:** 11
**Requires Product Confirmation:** 4
**UX Recommendation Only:** 1
**Confirmed Bugs:** 9
**UX Recommendations:** 2

The test documentation records the observed application behavior and separates confirmed defects from behaviors that require product clarification.
