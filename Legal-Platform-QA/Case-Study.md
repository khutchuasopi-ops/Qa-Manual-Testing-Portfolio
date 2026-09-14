1. Project Overview

The AI Writing Workspace is a web-based platform designed to support AI-assisted writing and content creation workflows.

This project focused on manually testing the main user flows and identifying functional issues, state and data persistence problems, AI workflow issues, and usability concerns.

Role: Junior Manual QA Tester
Environment: Staging / Preview
Testing Type: Manual Testing
Production Environment: Not tested

2. Testing Scope

The testing covered the following areas:

Board
Draft Editor
AI Assistant
Plan
Library
Project Details
Poster
AI Chat
Templates
Split View
Navigation and UI state
Data persistence
AI-generated content workflows
Conversation and context handling

The main focus was on verifying that user actions produced the expected results and that data, content, and application state remained consistent during normal and negative user flows.

3. Testing Approach

The project included several types of manual testing:

Functional testing
Exploratory testing
Smoke testing
Regression testing
Negative testing
User-flow testing
UI and usability checks
Data persistence checks
AI workflow and context checks

Testing was performed by following documented test scenarios and test cases, while also exploring related flows to identify unexpected behavior.

4. Test Execution

A total of 28 test cases were executed.

Results
Result	Count
PASS	12
FAIL	11
Requires Product Confirmation	4
UX Recommendation only	1
Total Test Cases	28

In addition to the test execution results, 9 confirmed bugs were documented.

There were also 2 UX recommendations identified during testing.

One of the UX recommendations was related to a test case that otherwise passed, so UX recommendations are not counted as a separate execution result in addition to the 28 test cases.

5. Key Findings

Several issues were identified during testing of the AI Writing Workspace.

Draft and Editor

Testing identified problems with draft persistence and editor behavior.

Draft content could be lost after refreshing the page.
Lowercase text could automatically appear as uppercase.
The AI Assistant could fail to write generated content into an editable Draft.
A new Draft could retain context from a previous independent AI conversation.

These issues could affect the reliability of the writing workflow and the user's confidence that their work and conversation context are being handled correctly.

Plan

The AI-generated Plan could be created successfully through the AI workflow, but the generated information was not correctly reflected on the Plan page.

This was documented as a confirmed issue because the expected result was not achieved.

Poster

Issues were identified in the Poster workflow:

Saving a Poster could be delayed or appear unresponsive.
The upload dialog could display a previous image instead of the current poster.

These behaviors could make it unclear whether the user's latest changes or selected image were successfully processed.

AI Chat

Testing identified an issue where creating a new chat could temporarily display the previous conversation.

This was documented as a confirmed bug because a new conversation should not display content from a previous independent conversation.

Split View

Testing of Split View identified duplicated or reset pagination controls in the second pane.

This could make navigation confusing when working with content in multiple panes.

6. Confirmed Bug Reports

The testing resulted in 9 confirmed bug reports:

Bug ID	Area	Issue
BUG-001	Draft	Draft content is lost after refresh
BUG-002	Draft Editor	Lowercase text is automatically displayed as uppercase
BUG-003	AI Assistant / Draft	AI Assistant fails to write content into an editable Draft
BUG-004	AI Assistant / Draft	New Draft retains previous independent conversation context
BUG-005	Plan / AI Assistant	AI-generated Plan is not reflected on the Plan page
BUG-006	Poster	Save Poster action is delayed or unresponsive
BUG-007	Poster	Upload dialog shows a previous image instead of the current poster
BUG-008	AI Chat	New Chat temporarily displays the previous conversation
BUG-009	Split View	Pagination/page controls are duplicated or reset in the second pane
7. Product Confirmation Items

Not every unexpected behavior was classified as a confirmed defect.

Some observations required clarification or confirmation of the intended product behavior, including:

Board deletion behavior
Initial Draft loading behavior
Deleted Project conversation behavior
Horizontal content behavior in Templates

These items were kept separate from confirmed bugs to avoid reporting expected product behavior as a defect without sufficient confirmation.

8. UX Recommendations

Two usability recommendations were documented during testing.

UX-001 — Grab Cursor

Template elements that can be dragged could benefit from a clearer grab/grabbing cursor.

This would make the draggable interaction more obvious to the user.

UX-002 — Close Button

The Project Details panel could benefit from a clearer and more visible Close/X control.

This would make it easier for users to understand how to close the panel.

9. Traceability

The documented bugs were linked to the relevant test cases to maintain traceability between testing and reported defects.

Examples include:

BUG-001 → TC-009
BUG-002 → TC-008
BUG-003 → TC-010
BUG-004 → TC-011
BUG-005 → TC-014, TC-015
BUG-006 → TC-020
BUG-007 → TC-021
BUG-008 → TC-022
BUG-009 → TC-026

This helped connect the observed behavior, expected result, test execution, and final defect report.

10. Outcome

The testing identified 9 confirmed functional issues across important parts of the AI Writing Workspace.

The most significant findings were related to:

Data persistence
Draft creation and editing
AI-generated content
AI conversation context
Plan synchronization
Poster state and saving
Chat state
Split View navigation

The testing also identified usability improvements and several behaviors that require product confirmation before being classified as defects.

11. What I Learned

This project helped me improve my understanding of testing AI-assisted applications and the importance of checking not only the visible result, but also application state and data consistency.

I practiced:

Creating and executing manual test cases
Testing positive and negative scenarios
Performing exploratory testing
Checking data persistence after navigation and refresh
Testing independent AI conversations and context
Identifying and documenting reproducible defects
Linking bugs back to test cases
Separating confirmed bugs from product behavior that requires clarification
Identifying usability improvements separately from functional defects

This project also reinforced the importance of clear reproduction steps and expected results when documenting issues for developers and product teams.

12. Conclusion

The AI Writing Workspace QA project provided practical experience in testing a modern AI-assisted web application through manual testing.

I was able to execute 28 test cases, identify 9 confirmed bugs, document 2 UX recommendations, and separate uncertain behaviors that required product confirmation from confirmed defects.

The project demonstrates my ability as a Junior Manual QA Tester to follow structured test cases, explore application behavior, identify issues, document defects clearly, and maintain traceability between test execution and bug reports.
