# Test Scenarios

## Overview

This document contains the main manual QA test scenarios executed during testing of the AI Writing Workspace.

The scenarios cover core user workflows, application state, data persistence, AI functionality, navigation, and UI/UX behavior.

---

# 1. Board

## TS-BOARD-001 — Verify Item Drag & Drop

**Area:** Board  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open the Board.
2. Select an existing item.
3. Drag the item to another position.
4. Release the item.

### Expected Result

The item should be moved to the selected position.

### Actual Result

The item was moved successfully.

### Status

**PASS**

---

## TS-BOARD-002 — Verify Moving an Item to Another Section

**Area:** Board  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open the Board.
2. Select an existing item.
3. Drag the item to another section.
4. Release the item.

### Expected Result

The item should be moved to the selected section.

### Actual Result

The item was moved successfully.

### Status

**PASS**

---

## TS-BOARD-003 — Verify Position Persistence After Drag & Drop

**Area:** Board  
**Priority:** Medium  
**Type:** Persistence

### Steps

1. Open the Board.
2. Move an item to a different position.
3. Refresh the page.
4. Check the item's position.

### Expected Result

The item should remain in its new position after refresh.

### Actual Result

The item position was preserved.

### Status

**PASS**

---

## TS-BOARD-004 — Verify Item Deletion

**Area:** Board  
**Priority:** High  
**Type:** Functional / Persistence

### Steps

1. Open the Board.
2. Select an existing item.
3. Delete the item.
4. Refresh the page.
5. Check whether the deleted item is still displayed.

### Expected Result

The deleted item should be removed and should not appear after refresh.

### Actual Result

The deleted item remained visible after deletion and was still displayed after refresh.

### Status

**FAIL**

**Related Bug:** BUG-001

---

# 2. Draft

## TS-DRAFT-001 — Verify Draft Loading

**Area:** Draft  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open a Project / Manuscript.
2. Navigate to Draft.
3. Observe the initial loading behavior.
4. Navigate to another section.
5. Return to Draft.

### Expected Result

Draft should load correctly when opened.

### Actual Result

Draft initially remained in a loading state. Navigating to another section and returning to Draft caused the content to load correctly.

### Status

**FAIL**

**Related Bug:** BUG-002

---

## TS-DRAFT-002 — Verify AI Initial Interaction

**Area:** Draft  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open a Manuscript.
2. Navigate to Draft.
3. Wait for the AI Assistant to load.
4. Observe the initial question.

### Expected Result

The AI Assistant should display an initial writing-related question.

### Actual Result

The AI Assistant displayed the expected initial question.

### Status

**PASS**

---

## TS-DRAFT-003 — Verify AI Assistant Text Entry

**Area:** Draft / AI Assistant  
**Priority:** High  
**Type:** Functional

### Steps

1. Open a Draft.
2. Interact with the AI Assistant.
3. Enter a writing topic.
4. Send the message.
5. Observe the response.

### Expected Result

The message should be submitted successfully and the AI Assistant should process the request.

### Actual Result

The AI Assistant returned an error during the interaction.

### Status

**FAIL**

**Related Bug:** BUG-005

---

## TS-DRAFT-004 — Verify Draft Editor Text Entry

**Area:** Draft Editor  
**Priority:** High  
**Type:** Functional / UI

### Steps

1. Open the Draft Editor.
2. Make sure Caps Lock is turned off.
3. Do not hold the Shift key.
4. Type lowercase text, for example:
   `once upon a time`
5. Observe the text while typing.

### Expected Result

The entered text should appear in lowercase.

### Actual Result

The text appeared in uppercase while it was being entered.

### Status

**FAIL**

**Related Bug:** BUG-004

---

## TS-DRAFT-005 — Verify Draft Content Persistence

**Area:** Draft Editor  
**Priority:** High  
**Type:** Persistence

### Steps

1. Open a Draft.
2. Enter text directly into the Draft Editor.
3. Leave the page.
4. Refresh the page.
5. Return to the Draft Editor.

### Expected Result

Previously entered Draft content should remain available after refresh.

### Actual Result

The entered text disappeared after refresh.

### Status

**FAIL**

**Related Bug:** BUG-003

---

## TS-DRAFT-006 — Verify AI Assistant Draft Creation

**Area:** Draft / AI Assistant  
**Priority:** High  
**Type:** Functional

### Steps

1. Open the Draft area.
2. Interact with the AI Assistant.
3. Provide a writing topic.
4. Ask the AI Assistant to write or create Draft content.
5. Observe the generated result.
6. Check whether the content is available as an editable Draft.

### Expected Result

The AI Assistant should create or update the appropriate editable Draft.

### Actual Result

The AI Assistant indicated that it was writing into a Draft, but the generated files were not created as the expected editable Draft content. In some cases, the assistant returned an error indicating that it could not place the edit.

### Status

**FAIL**

**Related Bug:** BUG-005

---

## TS-DRAFT-007 — Verify New Draft Context Isolation

**Area:** Draft / AI Assistant  
**Priority:** High  
**Type:** State / Context

### Steps

1. Open a new Draft.
2. Observe the initial AI Assistant question.
3. Enter a new and unrelated writing topic.
4. Continue the conversation.
5. Observe the information referenced by the AI Assistant.

### Expected Result

The new Draft should use only the context relevant to the new Draft.

### Actual Result

The AI Assistant referenced unrelated content from a previous independent document or conversation.

### Status

**FAIL**

**Related Bug:** BUG-006

---

# 3. Plan

## TS-PLAN-001 — Verify Plan Opens Correctly

**Area:** Plan  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open a Project / Manuscript.
2. Navigate to Plan.
3. Observe the page.

### Expected Result

The Plan page should open and display the available planning interface.

### Actual Result

The Plan page opened successfully.

### Status

**PASS**

---

## TS-PLAN-002 — Verify Assistant Planning Request

**Area:** Plan / AI Assistant  
**Priority:** High  
**Type:** Functional

### Steps

1. Open Plan.
2. Use the Assistant input.
3. Enter a request such as:
   `I want to plan an essay about the ocean.`
4. Submit the request.
5. Observe the AI response.
6. Check the Plan page.

### Expected Result

The AI-generated planning content should be reflected in the Plan interface.

### Actual Result

The Assistant generated planning options and indicated that it would build the outline on Plan, but the Plan page remained empty.

### Status

**FAIL**

**Related Bug:** BUG-007

---

## TS-PLAN-003 — Verify Plan After Refresh

**Area:** Plan  
**Priority:** High  
**Type:** Persistence

### Steps

1. Send a planning request through the Assistant.
2. Observe the generated response.
3. Refresh the Plan page.
4. Check the Plan content.

### Expected Result

Generated planning content should remain available after refresh if the operation was successfully completed.

### Actual Result

The Plan remained empty after refresh.

### Status

**FAIL**

**Related Bug:** BUG-007

---

# 4. Library

## TS-LIBRARY-001 — Verify Project Opening

**Area:** Library  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open Library.
2. Select a Project / Manuscript.
3. Open the Project.

### Expected Result

The selected Project should open successfully.

### Actual Result

The Project opened successfully.

### Status

**PASS**

---

## TS-LIBRARY-002 — Verify Project Details

**Area:** Library / Project  
**Priority:** Low  
**Type:** UI

### Steps

1. Open a Project from Library.
2. Open the Project details panel.
3. Review the displayed information.

### Expected Result

Relevant Project information should be displayed.

### Actual Result

Project information such as About, Author, Category, Date, Description, and Companion instructions was displayed.

### Status

**PASS**

---

# 5. Poster / Cover

## TS-POSTER-001 — Verify Poster Upload and Save

**Area:** Poster / Cover  
**Priority:** High  
**Type:** Functional

### Steps

1. Open a Project / Manuscript.
2. Select Edit.
3. Open the Upload option.
4. Select a new image.
5. Click Save Poster.
6. Observe the result.

### Expected Result

The selected image should be saved and displayed as the new poster immediately after saving.

### Actual Result

The Save Poster action did not respond immediately. After some time, the poster was eventually updated.

### Status

**FAIL**

**Related Bug:** BUG-008

---

## TS-POSTER-002 — Verify Poster Upload Dialog Shows Current Image

**Area:** Poster / Cover  
**Priority:** Medium  
**Type:** Functional / UI State

### Preconditions

A Project already has a poster image that has been changed and saved successfully.

### Steps

1. Open the Project.
2. Open the poster upload dialog.
3. Observe the currently displayed image.

### Expected Result

The upload dialog should display the current poster image.

### Actual Result

The dialog displayed the previously uploaded image instead of the current poster.

### Status

**FAIL**

**Related Bug:** BUG-009

---

# 6. AI Chat

## TS-AICHAT-001 — Verify New Chat State

**Area:** AI Chat  
**Priority:** Medium  
**Type:** State

### Steps

1. Open AI Chat.
2. Start a new Chat.
3. Observe the conversation area.
4. Enter a new message.

### Expected Result

A new Chat should start with a clean conversation state.

### Actual Result

The previous conversation remained visible until new text was entered. After entering new text, the conversation area refreshed and the previous content disappeared.

### Status

**FAIL**

**Related Bug:** BUG-011

---

## TS-AICHAT-002 — Verify Deleted Project Conversation Behavior

**Area:** AI Chat / Project  
**Priority:** Medium  
**Type:** State

### Steps

1. Open a Project / Manuscript with an existing AI Chat conversation.
2. Delete the Project / Manuscript.
3. Open the AI Chat conversation dropdown.
4. Check whether the deleted Project conversation is still listed.

### Expected Result

If Project deletion is expected to remove related conversations, the deleted Project conversation should no longer appear.

### Actual Result

The conversation title associated with the deleted Project remained visible in the AI Chat dropdown.

### Status

**FAIL / Requires Product Confirmation**

**Related Bug:** BUG-010

---

# 7. Templates

## TS-TEMPLATE-001 — Verify Draggable Template Elements

**Area:** Templates  
**Priority:** Medium  
**Type:** Functional

### Steps

1. Open a Template.
2. Hover over a draggable text element.
3. Drag the element to another position.
4. Release the mouse button.

### Expected Result

The element should be draggable and the interface should clearly indicate that it can be moved.

### Actual Result

The element could be dragged successfully, but the cursor remained a regular arrow instead of providing a clear drag/grab indication.

### Status

**PASS — UX Recommendation**

**Related UX:** UX-001

---

# 8. Split View

## TS-SPLIT-001 — Verify Pagination and Page Breaks in Split View

**Area:** Split View / Draft  
**Priority:** High  
**Type:** Functional / UI State

### Steps

1. Open a Project / Manuscript.
2. Open a Draft containing enough content for multiple pages.
3. Open the same Draft in Split View.
4. Observe the pagination and page breaks in both panes.
5. Compare the pagination behavior between the two sides.

### Expected Result

Pagination and page breaks should remain consistent and correctly positioned in both panes.

### Actual Result

Pagination/page breaks were duplicated or reset on the second side when the same Draft was opened in Split View.

### Status

**FAIL — Reproduced**

**Related Bug:** BUG-012

---

# 9. UX Recommendations

## TS-UX-001 — Project Details Close Button

**Area:** Library / Project Details  
**Type:** UX Recommendation

### Current Behavior

The Project / Manuscript details panel does not provide a visible Close (X) button. The panel can be closed by clicking outside of it.

### Recommendation

Consider adding a visible Close (X) button to make closing the panel easier and more intuitive.

### Status

**UX Recommendation**

**Related UX:** UX-002

---

# 10. Test Scenario Summary

| Area | Scenarios Tested | Pass | Fail | UX |
|------|------------------:|-----:|-----:|----:|
| Board | 4 | 3 | 1 | 0 |
| Draft | 7 | 1 | 6 | 0 |
| Plan | 3 | 1 | 2 | 0 |
| Library | 2 | 2 | 0 | 0 |
| Poster / Cover | 2 | 0 | 2 | 0 |
| AI Chat | 2 | 0 | 2 | 0 |
| Templates | 1 | 1 | 0 | 1 |
| Split View | 1 | 0 | 1 | 0 |
| UX Recommendations | 1 | 0 | 0 | 1 |

---

## Overall Result

The testing identified multiple functional and state-related issues across the application.

The most significant findings were related to:

- Draft content persistence
- AI-generated Draft content
- Draft loading
- AI conversation context
- Plan content updates
- Poster saving
- Split View pagination
- Deleted content state
- New Chat state

Additional usability improvements were identified for draggable Template elements and the Project / Manuscript details panel.

Detailed reproduction steps and evidence are documented separately in the Bug Reports and UX Recommendations sections.
