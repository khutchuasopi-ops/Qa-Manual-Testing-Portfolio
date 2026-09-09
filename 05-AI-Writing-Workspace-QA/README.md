# AI Writing Workspace — Manual QA Testing

## Project Overview

This project presents a manual QA testing case study for an AI-powered writing and planning workspace.

The product name has been anonymized for portfolio purposes.

Testing was performed only in the **Staging / Preview environment**. Production was not tested.

---

## Testing Scope

The testing covered the following areas:

- Board
- Draft Editor
- Plan
- AI Assistant
- AI Chat
- Library
- Templates
- Poster / Cover
- Split View
- Project / Manuscript management
- Navigation
- UI / UX
- Data persistence
- AI workflows and context handling

---

## Testing Approach

The main testing approaches used were:

- Functional testing
- Exploratory testing
- Smoke testing
- Regression testing
- Negative testing
- User-flow testing
- UI testing
- Data persistence testing
- AI workflow testing
- Context and state validation

---

## Key QA Findings

The testing identified issues related to:

- Draft content persistence
- Draft Editor text formatting
- AI-generated Draft content
- AI context isolation
- AI-generated Plan persistence
- Poster saving and image state
- AI Chat state handling
- Split View pagination

The project contains documented bug reports for confirmed issues and separate UX recommendations for usability improvements.

---

## Confirmed Bug Reports

| ID | Area | Issue |
|---|---|---|
| BUG-001 | Draft | Draft content is lost after refresh |
| BUG-002 | Draft Editor | Lowercase text is automatically entered in uppercase |
| BUG-003 | AI Assistant / Draft | AI Assistant fails to write content into an editable Draft |
| BUG-004 | AI Assistant / Draft | New Draft retains context from a previous independent conversation |
| BUG-005 | Plan / AI Assistant | AI-generated Plan content is not reflected on the Plan page |
| BUG-006 | Poster | Save Poster action is delayed or unresponsive |
| BUG-007 | Poster | Upload dialog shows the previous image instead of the current poster |
| BUG-008 | AI Chat | New Chat temporarily displays the previous conversation |
| BUG-009 | Split View | Pagination/page breaks are duplicated or reset in the second pane |

---

## UX Recommendations

The project also includes separate UX recommendations for usability improvements, including:

- Adding a grab cursor for draggable Template elements
- Adding a Close (X) button to the Project / Manuscript details panel

These recommendations are documented separately from confirmed functional bugs.

---

## Environment

**Environment:** Staging / Preview

**Production:** Out of scope

---

## QA Deliverables

This project includes:

- Project Overview
- Test Plan
- Test Scenarios
- Test Cases
- Checklists
- Bug Reports
- UX Recommendations

---

## QA Skills Demonstrated

- Manual Testing
- Functional Testing
- Exploratory Testing
- Regression Testing
- Smoke Testing
- Negative Testing
- UI / UX Testing
- User Flow Testing
- Data Persistence Testing
- AI Workflow Testing
- Bug Reporting
- Test Case Design
- Test Scenario Design
- Test Documentation
- GitHub-based QA Documentation
