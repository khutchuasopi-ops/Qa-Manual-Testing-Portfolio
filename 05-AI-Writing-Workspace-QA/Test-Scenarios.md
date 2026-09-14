# Test Scenarios — AI Writing Workspace QA

## 1. Board

### TS-001 — Board Item Management
**Objective:** Verify that Board items can be created, opened, edited, and deleted correctly.

**Related Test Cases:** TC-001, TC-002, TC-003, TC-004

**Expected Result:**
Board items should be displayed correctly and user actions should update the Board as expected.

**Note:**
Deletion behavior observed during testing requires product confirmation and is not counted as a confirmed defect.

---

## 2. Draft

### TS-002 — Draft Creation and Loading
**Objective:** Verify that a new Draft can be created and loaded correctly.

**Related Test Cases:** TC-005, TC-006, TC-007

**Expected Result:**
A new Draft should load correctly and allow the user to work with the editor without unexpected errors or state from another Draft.

**Note:**
Initial Draft loading behavior requires product confirmation where specified in the test cases.

---

### TS-003 — Draft Persistence
**Objective:** Verify that Draft content remains available after refreshing the page.

**Related Test Cases:** TC-009

**Expected Result:**
Previously saved Draft content should remain available after refresh.

**Related Bug:** BUG-001

**Result:** FAIL

---

## 3. Draft Editor

### TS-004 — Text Input Behavior
**Objective:** Verify that text entered into the Draft Editor is displayed as entered by the user.

**Related Test Cases:** TC-008

**Expected Result:**
Lowercase text should remain lowercase unless the user intentionally changes its formatting.

**Related Bug:** BUG-002

**Result:** FAIL

---

## 4. AI Assistant and Draft

### TS-005 — AI Content Insertion
**Objective:** Verify that the AI Assistant can generate content and insert it into the editable Draft.

**Related Test Cases:** TC-010

**Expected Result:**
AI-generated content should be inserted into the editable Draft when the user requests this action.

**Related Bug:** BUG-003

**Result:** FAIL

---

### TS-006 — New Draft Conversation State
**Objective:** Verify that a newly created Draft starts with the correct independent AI conversation state.

**Related Test Cases:** TC-011

**Expected Result:**
A new Draft should not automatically display or use conversation context from another independent Draft.

**Related Bug:** BUG-004

**Result:** FAIL

---

## 5. Plan and AI Assistant

### TS-007 — AI-Generated Plan Synchronization
**Objective:** Verify that AI-generated Plan content is correctly reflected on the Plan page.

**Related Test Cases:** TC-014, TC-015

**Expected Result:**
Content generated or updated through the AI Assistant should be reflected correctly on the corresponding Plan page.

**Related Bug:** BUG-005

**Result:** FAIL

---

## 6. Poster / Cover

### TS-008 — Save Poster Changes
**Objective:** Verify that changes made to a Poster are saved and reflected immediately after the save action.

**Related Test Cases:** TC-020

**Expected Result:**
After saving, the updated Poster should be displayed without an unexpected delay or unresponsive state.

**Related Bug:** BUG-006

**Result:** FAIL

---

### TS-009 — Poster Image Upload
**Objective:** Verify that the Poster upload dialog displays the correct image selected by the user.

**Related Test Cases:** TC-021

**Expected Result:**
The upload dialog should display the currently selected image and should not show an image from a previous interaction.

**Related Bug:** BUG-007

**Result:** FAIL

---

## 7. AI Chat

### TS-010 — New Chat State
**Objective:** Verify that a newly created chat starts without displaying content from a previous conversation.

**Related Test Cases:** TC-022

**Expected Result:**
A new chat should display its own conversation state and should not temporarily show the previous conversation.

**Related Bug:** BUG-008

**Result:** FAIL

---

## 8. Deleted Project Conversation

### TS-011 — Deleted Project Conversation
**Objective:** Verify the behavior of conversations associated with a deleted project.

**Related Test Cases:** TC-023

**Expected Result:**
The application should handle conversations belonging to deleted projects according to the intended product behavior.

**Result:** Requires Product Confirmation

**Note:**
The observed behavior was not classified as a confirmed defect because the intended product behavior requires confirmation.

---

## 9. Templates

### TS-012 — Template Content Display
**Objective:** Verify that Template content is displayed correctly.

**Related Test Cases:** TC-025

**Expected Result:**
Template content should be displayed according to the intended product layout and behavior.

**Result:** Requires Product Confirmation

**Note:**
The observed behavior requires confirmation of the intended product behavior.

---

## 10. Split View

### TS-013 — Split View Pagination and Page Controls
**Objective:** Verify that pagination and page controls work independently and correctly in Split View.

**Related Test Cases:** TC-026

**Expected Result:**
Each pane should display the correct pagination and page controls without duplicated or unexpectedly reset controls.

**Related Bug:** BUG-009

**Result:** FAIL

---

## 11. UX Recommendations

### TS-014 — Grab Cursor Usability
**Objective:** Review the cursor behavior when interacting with draggable elements.

**Related Test Cases:** TC-018

**Expected Result:**
The cursor should provide clear visual feedback when an element can be grabbed or moved.

**Result:** UX Recommendation Only

**Related UX Recommendation:** UX-001

---

### TS-015 — Close Button Usability
**Objective:** Review the usability and discoverability of close controls.

**Related Test Cases:** TC-024

**Expected Result:**
The close control should be easy to identify and use.

**Result:** PASS + UX Recommendation

**Related UX Recommendation:** UX-002

---

## 12. Product Confirmation Items

The following behaviors were separated from confirmed defects because the intended product behavior requires confirmation:

| Test Case | Area | Status |
|---|---|---|
| TC-004 | Board | Requires Product Confirmation |
| TC-005 | Draft | Requires Product Confirmation |
| TC-023 | Deleted Project Conversation | Requires Product Confirmation |
| TC-025 | Templates | Requires Product Confirmation |

These items should not be counted as confirmed bugs until the expected product behavior is confirmed.

---

## 13. Confirmed Defect Traceability

| Bug ID | Related Test Case(s) | Area |
|---|---|---|
| BUG-001 | TC-009 | Draft |
| BUG-002 | TC-008 | Draft Editor |
| BUG-003 | TC-010 | AI Assistant / Draft |
| BUG-004 | TC-011 | AI Assistant / Draft |
| BUG-005 | TC-014, TC-015 | Plan / AI Assistant |
| BUG-006 | TC-020 | Poster |
| BUG-007 | TC-021 | Poster |
| BUG-008 | TC-022 | AI Chat |
| BUG-009 | TC-026 | Split View |

---

## 14. Scenario Summary

| Category | Result |
|---|---:|
| Confirmed Bugs | 9 |
| Product Confirmation Items | 4 |
| UX Recommendations | 2 |

The confirmed defects are limited to the nine documented bug reports in the `Bug-Reports` folder.

Product confirmation items and UX recommendations are kept separate from confirmed functional defects.

---

## 15. Overall Testing Result

The test scenarios cover the main AI Writing Workspace workflows, including:

- Board
- Draft
- Draft Editor
- AI Assistant
- Plan
- Poster / Cover
- AI Chat
- Templates
- Split View
- Product state and persistence
- UX behavior

The scenarios are linked to the corresponding test cases, confirmed defects, product confirmation items, and UX recommendations to maintain clear traceability.
