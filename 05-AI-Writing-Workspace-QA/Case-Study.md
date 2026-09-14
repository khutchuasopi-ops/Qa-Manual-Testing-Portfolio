# Case Study — AI Writing Workspace QA

## 1. Project Overview

The AI Writing Workspace is a web-based application designed to support AI-assisted writing and content creation.

This project focused on manually testing the main user flows and checking whether the application behaved as expected during normal, negative, and exploratory testing.

**Role:** Junior Manual QA Tester  
**Environment:** Staging / Preview  
**Testing Type:** Manual Testing  
**Production Environment:** Not tested

---

## 2. Testing Scope

The following areas were tested:

- Board
- Draft Editor
- AI Assistant
- Plan
- Library
- Project Details
- Poster
- AI Chat
- Templates
- Split View
- Navigation
- UI state
- Data persistence
- AI-generated content workflows
- Conversation and context handling

The main focus was on verifying user actions, expected results, data persistence, application state, and behavior across related user flows.

---

## 3. Testing Approach

The testing included:

- Functional testing
- Exploratory testing
- Smoke testing
- Regression testing
- Negative testing
- User-flow testing
- UI and usability checks
- Data persistence checks
- AI workflow and context checks

Testing was performed using documented test scenarios and test cases, together with exploratory checks of related functionality.

---

## 4. Test Execution

A total of **28 test cases** were executed.

| Result | Count |
|---|---:|
| PASS | 12 |
| FAIL | 11 |
| Requires Product Confirmation | 4 |
| UX Recommendation only | 1 |
| **Total Test Cases** | **28** |

The testing resulted in **9 confirmed bug reports** and **2 UX recommendations**.

One of the UX recommendations was identified during a test case that otherwise passed. Therefore, the UX recommendation is not counted as an additional test execution result.

---

## 5. Key Findings

### Draft and Draft Editor

Testing identified several issues affecting the Draft workflow.

- Draft content could be lost after refreshing the page.
- Lowercase text could automatically be displayed as uppercase.
- The AI Assistant could fail to write generated content into an editable Draft.
- A new Draft could retain context from a previous independent AI conversation.

These issues could affect the reliability of the writing workflow and the user's ability to work with Draft content as expected.

### Plan

The AI Assistant could generate a Plan, but the generated Plan was not correctly reflected on the Plan page.

This was documented as a confirmed defect because the expected result was not achieved.

### Poster

Testing identified issues related to Poster functionality.

- Saving a Poster could be delayed or appear unresponsive.
- The upload dialog could display a previous image instead of the current poster.

These behaviors could make it unclear whether the latest Poster changes or selected image had been successfully processed.

### AI Chat

Testing identified an issue where a newly created chat could temporarily display the previous conversation.

A new independent conversation should not display content from a previous conversation.

### Split View

Testing identified duplicated or reset pagination/page controls in the second pane of Split View.

This could make navigation confusing when working with content in multiple panes.

---

## 6. Confirmed Bug Reports

The testing resulted in **9 confirmed bug reports**.

| Bug ID | Area | Issue |
|---|---|---|
| BUG-001 | Draft | Draft content is lost after refresh |
| BUG-002 | Draft Editor | Lowercase text is automatically displayed as uppercase |
| BUG-003 | AI Assistant / Draft | AI Assistant fails to write content into an editable Draft |
| BUG-004 | AI Assistant / Draft | New Draft retains previous independent conversation context |
| BUG-005 | Plan / AI Assistant | AI-generated Plan is not reflected on the Plan page |
| BUG-006 | Poster | Save Poster action is delayed or unresponsive |
| BUG-007 | Poster | Upload dialog shows a previous image instead of the current poster |
| BUG-008 | AI Chat | New Chat temporarily displays the previous conversation |
| BUG-009 | Split View | Pagination/page controls are duplicated or reset in the second pane |

---

## 7. Product Confirmation Items

Not every unexpected behavior was classified as a confirmed bug.

The following observations require confirmation of the intended product behavior:

- Board deletion behavior
- Initial Draft loading behavior
- Deleted Project conversation behavior
- Horizontal content behavior in Templates

These observations were kept separate from confirmed defects because the expected product behavior was not sufficiently confirmed.

---

## 8. UX Recommendations

Two usability recommendations were identified during testing.

### UX-001 — Grab Cursor

Template elements that can be dragged could benefit from a clearer grab/grabbing cursor.

This would make the draggable interaction more obvious to users.

### UX-002 — Close Button

The Project Details panel could benefit from a clearer and more visible Close/X control.

This would make it easier for users to understand how to close the panel.

---

## 9. Bug Traceability

The confirmed bugs were linked to the relevant test cases.

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

This traceability connects the observed behavior with the related test execution and defect report.

---

## 10. Main Areas of Risk

The main areas where issues were identified were:

- Data persistence
- Draft creation and editing
- AI-generated content
- AI conversation context
- Plan synchronization
- Poster saving and image state
- Chat state
- Split View navigation

These areas are important because unexpected behavior in them can directly affect the user's workflow and the reliability of their work.

---

## 11. What I Learned

This project helped me gain practical experience in testing an AI-assisted web application.

During the project, I practiced:

- Creating and executing manual test cases
- Testing positive and negative scenarios
- Performing exploratory testing
- Performing smoke and regression testing
- Checking data persistence after refresh and navigation
- Testing AI-generated content workflows
- Checking conversation and context behavior
- Identifying and documenting reproducible defects
- Linking bugs to related test cases
- Separating confirmed defects from items requiring product confirmation
- Identifying usability improvements separately from functional defects

The project also reinforced the importance of clear reproduction steps, expected results, and accurate defect documentation.

---

## 12. Conclusion

The AI Writing Workspace QA project provided practical experience in manually testing an AI-assisted web application.

A total of **28 test cases** were executed, resulting in **12 PASS**, **11 FAIL**, **4 cases requiring product confirmation**, and **1 UX recommendation-only case**.

The testing resulted in **9 confirmed bug reports** and **2 UX recommendations**.

The project demonstrates my ability as a **Junior Manual QA Tester** to execute structured tests, perform exploratory checks, identify reproducible issues, document defects clearly, maintain traceability, and distinguish confirmed bugs from behavior that requires further product clarification.
