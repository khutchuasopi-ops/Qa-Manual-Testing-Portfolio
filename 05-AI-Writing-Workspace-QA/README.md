# AI Writing Workspace — Manual QA Testing

## Project Overview

This project covers manual QA testing of an anonymized AI Writing Workspace application.

The testing focused on core writing workflows, AI-assisted features, data persistence, project and library management, poster functionality, chat behavior, templates, split view, and general UI behavior.

## Testing Scope

The following areas were tested:

- Board
- Draft
- Plan
- AI Assistant
- Library / Project Management
- Templates
- Split View
- Poster / Cover
- Navigation and UI
- Data Persistence and State
- AI-assisted writing workflows

## Testing Approach

The application was tested manually using:

- Functional Testing
- Exploratory Testing
- End-to-End User Flow Testing
- Data Persistence and State Testing
- AI Feature Testing
- Negative Testing
- UI and Usability Testing

The testing included normal user flows as well as scenarios involving data persistence, navigation, state changes, AI-generated content, and invalid or unexpected behavior.

## Test Execution Summary

A total of **28 test cases** were executed.

| Result | Count |
|---|---:|
| PASS | 12 |
| FAIL | 11 |
| Requires Product Confirmation | 4 |
| UX Recommendation Only | 1 |
| **Total** | **28** |

In addition to the test case results, **2 UX recommendations** were documented. One of them was associated with a test case that otherwise passed.

## Confirmed Defects

Nine confirmed defects were identified and documented.

| Bug ID | Area | Issue |
|---|---|---|
| BUG-001 | Draft | Draft content is lost after refresh |
| BUG-002 | Draft Editor | Lowercase text is automatically displayed as uppercase |
| BUG-003 | AI Assistant / Draft | AI Assistant fails to write content into the editable Draft |
| BUG-004 | AI Assistant / Draft | New Draft retains the previous independent conversation context |
| BUG-005 | Plan / AI Assistant | AI-generated Plan content is not reflected on the Plan page |
| BUG-006 | Poster | Saving Poster changes is delayed or unresponsive |
| BUG-007 | Poster | Upload dialog shows a previous image instead of the current poster |
| BUG-008 | AI Chat | New Chat temporarily displays the previous conversation |
| BUG-009 | Split View | Pagination and page controls are duplicated or reset in the second pane |

## Bug Traceability

| Bug ID | Related Test Case(s) |
|---|---|
| BUG-001 | TC-009 |
| BUG-002 | TC-008 |
| BUG-003 | TC-010 |
| BUG-004 | TC-011 |
| BUG-005 | TC-014, TC-015 |
| BUG-006 | TC-020 |
| BUG-007 | TC-021 |
| BUG-008 | TC-022 |
| BUG-009 | TC-026 |

## Product Confirmation Items

Four test cases required product confirmation rather than being recorded as confirmed defects:

- **TC-004** — Draft initial loading behavior
- **TC-005** — Initial Draft loading behavior
- **TC-023** — Deleted project conversation behavior
- **TC-025** — Horizontal Template content behavior

These items were kept separate from confirmed bugs because the observed behavior required confirmation of the intended product behavior.

## UX Recommendations

Two UX recommendations were identified during testing:

- **UX-001** — Grab cursor behavior
- **UX-002** — Close button usability

These recommendations are separate from confirmed functional defects.

## Key Findings

The main issues identified during testing were related to:

- Data persistence after page refresh
- Text input behavior
- AI-generated content integration
- Conversation and application state
- Plan synchronization
- Poster saving and image handling
- New chat state
- Split View pagination and page controls

The testing showed that several issues could affect the reliability of user data, consistency between related application areas, and the overall user experience.

## QA Activities Demonstrated

This project demonstrates practical experience with:

- Manual test case execution
- Functional testing
- Exploratory testing
- End-to-end user flow testing
- Data persistence testing
- State behavior testing from a user perspective
- AI feature testing
- Negative testing
- UI and usability testing
- Defect identification
- Bug reporting
- Test result documentation
- Defect traceability

## Conclusion

The AI Writing Workspace testing covered **28 executed test cases** across the main writing, AI, project management, poster, chat, template, and split-view workflows.

The final test execution results were:

- **12 PASS**
- **11 FAIL**
- **4 Requires Product Confirmation**
- **1 UX Recommendation Only**

A total of **9 confirmed bugs** and **2 UX recommendations** were documented.

The project demonstrates a practical manual QA approach to testing an application that combines traditional workspace functionality with AI-assisted features.
