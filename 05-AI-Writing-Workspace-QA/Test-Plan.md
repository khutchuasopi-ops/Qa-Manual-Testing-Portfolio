# Test Plan

## 1. Test Plan Overview

This test plan defines the manual QA approach used to evaluate the AI Writing Workspace in a staging/preview environment.

The testing focuses on the application's main user workflows, including writing, planning, AI-assisted features, project management, and document interaction.

The goal is to identify functional defects, state and persistence issues, AI workflow problems, and usability improvements.

---

## 2. Test Objectives

The main testing objectives are:

- Verify that core application features work as expected.
- Verify complete user workflows from start to finish.
- Identify reproducible functional defects.
- Verify data persistence after page refresh.
- Verify application state after navigation.
- Test AI Assistant workflows.
- Verify Draft Editor behavior.
- Verify Board interactions.
- Verify Plan functionality.
- Verify Project and Manuscript management.
- Verify Poster upload and save behavior.
- Verify Template interactions.
- Verify Split View behavior.
- Test conversation and context isolation.
- Identify usability and UX issues.
- Collect evidence for reproducible issues.

---

## 3. Test Scope

### In Scope

The following areas are included in testing:

- Board
- Draft
- Draft Editor
- Plan
- AI Chat
- Library
- Projects / Manuscripts
- Templates
- Poster / Cover management
- Split View
- Navigation
- Data persistence
- Page refresh behavior
- Conversation state
- AI Assistant workflows
- UI and UX behavior

### Out of Scope

The following areas are outside the scope of this testing:

- Production environment
- Performance testing
- Load testing
- Security testing
- API testing
- Automated testing
- Backend infrastructure testing
- Database-level testing

---

## 4. Test Environment

### Environment

Staging / Preview

### Testing Type

Manual QA

### Testing Methods

- Functional Testing
- Exploratory Testing
- Regression Testing
- End-to-End Testing
- UI/UX Testing
- State Testing
- Persistence Testing
- AI Feature Testing

### Production

Production was not tested.

---

## 5. Testing Strategy

Testing was performed using realistic end-user workflows.

Instead of testing only individual elements, the application was tested across multiple states and interactions.

The testing strategy included:

### Functional Testing

Verify that application features behave according to their intended functionality.

### Exploratory Testing

Explore the application using realistic user actions to identify unexpected behavior.

### End-to-End Testing

Verify complete workflows across multiple application sections.

### Regression Testing

Repeat previously tested workflows after encountering issues to verify whether behavior was consistent.

### Persistence Testing

Refresh pages and reopen content to verify whether user data and changes were preserved.

### State Testing

Check whether the application maintained the correct state after navigation, refresh, deletion, and switching between views.

### AI Feature Testing

Test AI Assistant interactions, generated content, Draft creation, planning, and conversation context.

### UI/UX Testing

Evaluate whether interactive elements provide clear feedback and whether the interface behaves intuitively.

---

## 6. Test Areas

### 6.1 Board

Test the following:

- Item drag and drop
- Moving items between sections
- Item position persistence
- Item deletion
- Deleted item behavior after refresh

### 6.2 Draft

Test the following:

- Draft opening
- Initial Draft loading
- AI Assistant interaction
- Draft Editor text entry
- Text behavior
- Draft content persistence
- Refresh behavior
- AI-generated Draft content
- New Draft behavior
- Conversation context

### 6.3 Plan

Test the following:

- Opening Plan
- Assistant planning request
- AI-generated planning options
- Plan content update
- Plan persistence after refresh

### 6.4 AI Chat

Test the following:

- Sending messages
- AI responses
- New Chat behavior
- Conversation state
- Context isolation
- Project-related conversations
- Deleted Project conversation behavior

### 6.5 Library

Test the following:

- Opening Projects / Manuscripts
- Project details
- Navigation
- Details panel behavior

### 6.6 Templates

Test the following:

- Template interaction
- Draggable elements
- Cursor behavior
- Horizontal content behavior

### 6.7 Poster / Cover

Test the following:

- Uploading images
- Saving poster changes
- Poster update behavior
- Upload dialog behavior
- Previously uploaded image behavior

### 6.8 Split View

Test the following:

- Opening the same Draft in Split View
- Multiple Draft panes
- Pagination behavior
- Page break behavior
- Consistency between panes

---

## 7. Data Persistence Checks

Persistence testing is an important part of this project.

The following actions were checked:

- Enter content
- Save content
- Refresh the page
- Reopen the content
- Navigate away and return
- Delete an item
- Refresh after deletion
- Change a poster
- Reopen the upload dialog
- Create a new conversation
- Switch between different application sections

The expected behavior was that saved changes should remain available and deleted content should no longer appear where applicable.

---

## 8. AI Assistant Testing

AI-related functionality was tested using realistic prompts and follow-up responses.

The testing included:

- Starting an AI interaction
- Providing a writing topic
- Providing additional information
- Asking the AI to generate content
- Asking the AI to create or update Draft content
- Asking the AI to create planning content
- Starting a new Draft
- Starting a new Chat
- Checking whether previous conversation context remained
- Verifying whether AI-generated content appeared in the expected application area

Special attention was given to cases where the AI indicated that content had been created or updated but the corresponding UI did not reflect the change.

---

## 9. Navigation and State Testing

Navigation was tested between major application areas.

Examples included:

- Library → Project / Manuscript
- Project → Draft
- Draft → Plan
- Plan → Draft
- Project → AI Chat
- Opening the same Draft in Split View
- Returning to previously opened content

The application was also checked after navigation to determine whether the expected state was preserved.

---

## 10. Refresh Testing

Page refreshes were intentionally performed after important actions.

Examples included:

- Entering Draft content
- Deleting Board items
- Creating Plan content
- Changing poster images
- Navigating between Draft and Plan
- Starting new conversations

The purpose was to identify issues that might not be visible during the initial interaction.

---

## 11. Expected Quality Criteria

The application should:

- Respond correctly to user actions.
- Save user changes successfully.
- Preserve saved content after refresh.
- Remove deleted content where deletion is expected.
- Maintain consistent application state.
- Display generated content in the correct location.
- Keep independent conversations isolated.
- Provide clear feedback after user actions.
- Maintain consistent behavior between different views.
- Avoid unexpected data or context from unrelated workflows.

---

## 12. Defect Documentation

Each confirmed defect will be documented separately.

Bug reports will contain:

- Bug ID
- Title
- Preconditions
- Steps to Reproduce
- Expected Result
- Actual Result
- Priority
- Environment
- Evidence

UX recommendations will be documented separately when the current functionality works but the user experience could be improved.

---

## 13. Evidence

Supporting screenshots and screen recordings will be organized by application area.

Evidence categories include:

- Board
- Draft
- Plan
- AI Chat
- Library
- Poster
- Split View

Evidence will be referenced from the relevant bug report or UX recommendation.

---

## 14. Test Completion Criteria

Testing for this project is considered complete when:

- Core workflows have been tested.
- Important application areas have been covered.
- Reproducible defects have been documented.
- Regression checks have been performed where appropriate.
- UX recommendations have been identified.
- Supporting evidence has been collected where available.
- Test documentation has been organized in the portfolio.

---

## 15. Test Result

Overall testing identified multiple functional, state, persistence, AI workflow, and usability issues.

The detailed results are documented in the Test Scenarios, Test Cases, Checklists, Bug Reports, and UX Recommendations sections of this project.
