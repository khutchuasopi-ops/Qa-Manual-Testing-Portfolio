# Test Cases

## Overview

This document contains the detailed manual test cases executed during testing of the AI Writing Workspace in a staging/preview environment.

The test cases cover functional behavior, user workflows, persistence, application state, AI-assisted features, navigation, UI behavior, and usability.

---

# Board

## TC-001 — Verify Board Item Drag & Drop

**Area:** Board
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Preconditions

* User is logged in.
* Board contains at least one existing item.

### Steps

1. Open the Board.
2. Select an existing item.
3. Drag the item to another position.
4. Release the item.

### Expected Result

The item should move to the selected position.

### Actual Result

The item moved successfully.

---

## TC-002 — Verify Moving an Item to Another Section

**Area:** Board
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Preconditions

* Board contains items.
* Board contains more than one section.

### Steps

1. Open the Board.
2. Select an existing item.
3. Drag the item to another section.
4. Release the item.

### Expected Result

The item should be moved to the selected section.

### Actual Result

The item was moved successfully to another section.

---

## TC-003 — Verify Item Position Persistence

**Area:** Board
**Type:** Persistence
**Priority:** Medium
**Status:** PASS

### Preconditions

* Board contains an existing item.

### Steps

1. Open the Board.
2. Move an item to a different position.
3. Wait for the change to be applied.
4. Refresh the page.
5. Check the item's position.

### Expected Result

The item's new position should remain unchanged after refresh.

### Actual Result

The item's position remained unchanged after refresh.

---

## TC-004 — Verify Board Item Deletion

**Area:** Board
**Type:** Functional / Persistence
**Priority:** High
**Status:** FAIL

### Preconditions

* Board contains an existing item that can be deleted.

### Steps

1. Open the Board.
2. Select an existing item.
3. Delete the item.
4. Observe the Board.
5. Refresh the page.
6. Check whether the deleted item is still visible.

### Expected Result

The deleted item should disappear from the Board and should not return after refresh.

### Actual Result

The deleted item remained visible after deletion and was still displayed after refreshing the page.

### Evidence

Screen recording / screenshot of the deletion and refresh behavior.

---

# Draft

## TC-005 — Verify Draft Initial Loading

**Area:** Draft
**Type:** Functional / State
**Priority:** Medium
**Status:** FAIL

### Preconditions

* User has access to an existing Project / Manuscript.
* Project contains a Draft.

### Steps

1. Open the Project / Manuscript.
2. Navigate to Draft.
3. Observe the Draft loading state.
4. Wait for the Draft to load.

### Expected Result

The Draft should load normally when opened.

### Actual Result

The Draft initially remained in a loading state.

### Additional Verification

1. Navigate from Draft to Plan.
2. Navigate back to Draft.
3. Observe the Draft.

### Result

After navigating to Plan and returning to Draft, the Draft loaded correctly.

---

## TC-006 — Verify AI Initial Draft Interaction

**Area:** Draft / AI Assistant
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Preconditions

* User is inside a Draft.

### Steps

1. Open Draft.
2. Wait for the AI Assistant.
3. Observe the initial AI prompt.

### Expected Result

The AI Assistant should display an initial question asking what the user is writing.

### Actual Result

The AI Assistant displayed the expected initial writing-related question.

---

## TC-007 — Verify AI Assistant User Input

**Area:** Draft / AI Assistant
**Type:** Functional
**Priority:** High
**Status:** FAIL

### Preconditions

* Draft is open.
* AI Assistant is available.

### Steps

1. Open Draft.
2. Enter a writing topic in the AI Assistant.
3. Submit the message.
4. Observe the AI response.

### Expected Result

The message should be submitted successfully and the AI Assistant should process the request.

### Actual Result

The AI Assistant returned an error during the interaction.

### Observed Error

The application displayed an error related to a missing `fs_entries` mirror for the Draft.

---

## TC-008 — Verify Draft Editor Text Entry

**Area:** Draft Editor
**Type:** Functional / UI
**Priority:** High
**Status:** FAIL

### Preconditions

* Draft Editor is open.
* Caps Lock is turned off.
* Shift is not being pressed.

### Steps

1. Click inside the actual Draft Editor.
2. Type lowercase text.
3. Example input:

`once upon a time`

4. Observe the text while entering it.

### Expected Result

The text should appear exactly as typed in lowercase.

### Actual Result

The text appeared immediately in uppercase:

`ONCE UPON A TIME`

The capitalization changed while typing and was not the result of a later refresh or formatting step.

### Evidence

Screen recording while typing lowercase text with Caps Lock off.

---

## TC-009 — Verify Draft Content Persistence After Refresh

**Area:** Draft Editor
**Type:** Persistence
**Priority:** High
**Status:** FAIL

### Preconditions

* Draft Editor is open.

### Steps

1. Open a Draft.
2. Click inside the actual Draft Editor.
3. Enter text.
4. Observe that the text appears in the editor.
5. Refresh the page.
6. Return to the Draft.

### Expected Result

The entered Draft content should remain available after refresh.

### Actual Result

The entered text disappeared after refreshing the page.

---

## TC-010 — Verify AI Assistant Can Create Editable Draft Content

**Area:** Draft / AI Assistant
**Type:** Functional
**Priority:** High
**Status:** FAIL

### Preconditions

* User is inside the Draft / AI Assistant workflow.

### Steps

1. Open the Draft.
2. Interact with the AI Assistant.
3. Provide a writing topic.
4. Ask the Assistant to write content.
5. Observe the generated content.
6. Check whether the generated content is available in the editable Draft.

### Expected Result

The AI Assistant should create or update content in the appropriate editable Draft.

### Actual Result

The Assistant indicated that it was writing into the Draft, but the generated files were tagged as `[archive_file]` instead of the expected editable `[draft]`.

In another attempt, the Assistant started the writing process but returned an error indicating that it could not place the edit.

### Additional Test

A separate writing request was also tested using a different topic and follow-up answers.

### Result

The AI Assistant still could not reliably create or place the requested content into an editable Draft.

---

## TC-011 — Verify New Draft Uses Independent Context

**Area:** Draft / AI Assistant
**Type:** State / Context Isolation
**Priority:** High
**Status:** FAIL

### Preconditions

* A new Draft is opened.
* There is previous content from a separate independent document or conversation.

### Steps

1. Open a new Draft.
2. Observe the initial AI question.
3. Enter a completely new and unrelated topic.
4. Continue the conversation.
5. Observe the information referenced by the AI Assistant.

### Expected Result

The new Draft should use only information relevant to the new Draft.

### Actual Result

The AI Assistant referenced unrelated information from a previous independent document/conversation.

The previous topic was not part of the new Draft.

---

# Plan

## TC-012 — Verify Plan Page Opens

**Area:** Plan
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Preconditions

* User has access to a Project / Manuscript.

### Steps

1. Open the Project / Manuscript.
2. Navigate to Plan.
3. Observe the page.

### Expected Result

The Plan page should open successfully.

### Actual Result

The Plan page opened successfully.

---

## TC-013 — Verify Plan Assistant Input

**Area:** Plan / AI Assistant
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Preconditions

* Plan page is open.

### Steps

1. Open Plan.
2. Locate the Assistant input.
3. Enter a planning request.
4. Example:

`I want to plan an essay about the ocean.`

5. Submit the request.
6. Observe the Assistant response.

### Expected Result

The Assistant should process the request and provide relevant planning information.

### Actual Result

The Assistant generated several planning options and indicated that it would build the outline on Plan.

---

## TC-014 — Verify AI-Generated Plan Appears on Plan Page

**Area:** Plan / AI Assistant
**Type:** Functional
**Priority:** High
**Status:** FAIL

### Preconditions

* Plan page is open.
* Assistant is available.

### Steps

1. Send a planning request through the Assistant.
2. Wait for the Assistant response.
3. Observe the generated options.
4. Check the Plan page.

### Expected Result

The generated planning content should appear on the Plan page.

### Actual Result

The Assistant generated options and stated that it would build the outline on Plan, but the Plan page remained empty.

---

## TC-015 — Verify Plan Content After Refresh

**Area:** Plan
**Type:** Persistence
**Priority:** High
**Status:** FAIL

### Steps

1. Send a planning request.
2. Wait for the Assistant response.
3. Check the Plan page.
4. Refresh the page.
5. Check the Plan again.

### Expected Result

Successfully generated Plan content should remain available after refresh.

### Actual Result

The Plan remained empty after refresh.

---

# Library

## TC-016 — Verify Project / Manuscript Opens from Library

**Area:** Library
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Steps

1. Open Library.
2. Select an existing Project / Manuscript.
3. Open it.

### Expected Result

The selected Project / Manuscript should open successfully.

### Actual Result

The Project / Manuscript opened successfully.

---

## TC-017 — Verify Project Details Information

**Area:** Library / Project Details
**Type:** UI / Functional
**Priority:** Low
**Status:** PASS

### Steps

1. Open a Project / Manuscript from Library.
2. Open the details panel.
3. Review the displayed information.

### Expected Result

The details panel should display the available Project information.

### Actual Result

The panel displayed information including:

* About
* Author
* Category
* Date
* Description
* Companion instructions

---

## TC-018 — Verify Project Details Panel Closing

**Area:** Library / Project Details
**Type:** UX
**Priority:** Low
**Status:** UX Recommendation

### Steps

1. Open a Project / Manuscript.
2. Open the details panel.
3. Try to close the panel.

### Expected Result

The panel should provide an obvious and intuitive way to close it.

### Actual Result

The panel could be closed by clicking outside of it, but there was no visible Close (X) button.

### Recommendation

Consider adding a Close (X) button to make the panel easier to close.

---

# Poster / Cover

## TC-019 — Verify Poster Image Upload

**Area:** Poster / Cover
**Type:** Functional
**Priority:** Medium
**Status:** PASS

### Steps

1. Open a Project / Manuscript.
2. Select Edit.
3. Open the Upload option.
4. Select an image.
5. Observe the upload behavior.

### Expected Result

The selected image should be accepted and prepared for saving.

### Actual Result

The image was selected successfully.

---

## TC-020 — Verify Save Poster Action

**Area:** Poster / Cover
**Type:** Functional / State
**Priority:** High
**Status:** FAIL

### Steps

1. Open a Project / Manuscript.
2. Select Edit.
3. Open Upload.
4. Select a new image.
5. Click Save Poster.
6. Observe the result immediately.
7. Wait and observe again.

### Expected Result

The new poster should be saved and displayed immediately after clicking Save Poster.

### Actual Result

The Save Poster action did not respond immediately despite multiple clicks.

After some time, the poster was eventually updated.

### Note

The poster image was eventually updated, but the change was not applied immediately after clicking Save Poster.

---

## TC-021 — Verify Upload Dialog Displays Current Poster

**Area:** Poster / Cover
**Type:** UI State
**Priority:** Medium
**Status:** FAIL

### Preconditions

* A Project already has a poster.
* The poster has previously been changed and saved successfully.

### Steps

1. Open the Project.
2. Open the poster upload dialog again.
3. Observe the image displayed in the dialog.

### Expected Result

The upload dialog should display the current poster image.

### Actual Result

The upload dialog displayed the previously uploaded image instead of the current poster.

---

# AI Chat

## TC-022 — Verify New Chat Clears Previous Conversation

**Area:** AI Chat
**Type:** State
**Priority:** Medium
**Status:** FAIL

### Steps

1. Open AI Chat.
2. Select New Chat.
3. Observe the conversation area before entering a new message.
4. Enter new text.
5. Observe the conversation again.

### Expected Result

The new Chat should start with a clean conversation state and should not display the previous conversation.

### Actual Result

The previous conversation remained visible until new text was entered.

After entering new text, the conversation refreshed and the previous content disappeared.

---

## TC-023 — Verify Deleted Project Conversation in AI Chat

**Area:** AI Chat / Project
**Type:** State
**Priority:** Medium
**Status:** FAIL / Requires Product Confirmation

### Preconditions

* A Project / Manuscript has an existing AI Chat conversation.

### Steps

1. Open the Project / Manuscript.
2. Delete the Project / Manuscript.
3. Open the AI Chat dropdown.
4. Review the available conversation titles.

### Expected Result

If deleting a Project is expected to remove its related conversation, the deleted Project's conversation should no longer appear.

### Actual Result

The conversation title associated with the deleted Project remained visible in the AI Chat dropdown.

### Note

This behavior should be confirmed against the intended product behavior because AI Chat history may potentially be designed to remain independent from Project deletion.

---

# Templates

## TC-024 — Verify Template Element Dragging

**Area:** Templates
**Type:** Functional / UX
**Priority:** Medium
**Status:** PASS — UX Recommendation

### Steps

1. Open a Template.
2. Locate a draggable text element.
3. Move the cursor over the element.
4. Drag the element to another position.

### Expected Result

The element should be draggable.

The cursor should also provide a clear indication that the element can be moved.

### Actual Result

The element could be dragged successfully.

However, the cursor remained a regular arrow instead of changing to a hand/grab cursor.

### Recommendation

Consider adding a grab/hand cursor when hovering over draggable Template elements.

---

## TC-025 — Verify Horizontal Template Content Behavior

**Area:** Templates
**Type:** UI
**Priority:** Medium
**Status:** To Be Confirmed

### Steps

1. Open a Template.
2. Observe the Template content area.
3. Check whether content extends beyond the visible horizontal area.
4. Check whether horizontal navigation is available.

### Expected Result

If Template content exceeds the available horizontal space, users should have an intuitive way to access the hidden content.

### Actual Result

Horizontal scrolling behavior was identified as an area requiring verification.

### Status

**To Be Confirmed**

---

# Split View

## TC-026 — Verify Same Draft in Split View

**Area:** Split View / Draft
**Type:** Functional
**Priority:** High
**Status:** FAIL — Reproduced

### Preconditions

* A Project / Manuscript contains a Draft.
* The Draft contains enough content for multiple pages.

### Steps

1. Open the Project / Manuscript.
2. Open the Draft.
3. Open the same Draft in Split View.
4. Observe both panes.
5. Compare pagination and page breaks.

### Expected Result

Pagination and page breaks should remain consistent when the same Draft is displayed in Split View.

### Actual Result

Pagination/page breaks were duplicated or reset on the second side when the same Draft was opened in Split View.

### Reproduction Status

**Reproduced**

### Evidence

Screen recording available in the Split View evidence folder.

---

# Additional Workflow Checks

## TC-027 — Verify Draft → Plan → Draft Navigation

**Area:** Draft / Plan
**Type:** Navigation / State
**Priority:** Medium
**Status:** PASS

### Steps

1. Open a Project / Manuscript.
2. Open Draft.
3. Navigate to Plan.
4. Navigate back to Draft.
5. Observe the Draft.

### Expected Result

Navigation between Draft and Plan should work without preventing access to the Draft.

### Actual Result

Navigation worked, and returning to Draft caused the previously loading Draft to load correctly.

### Note

This workflow also helped reproduce the Draft initial loading issue documented in TC-005.

---

## TC-028 — Verify Draft Editor Is Different from AI Chat Input

**Area:** Draft
**Type:** Functional / Workflow
**Priority:** Medium
**Status:** PASS

### Steps

1. Open a Draft.
2. Interact with the AI Assistant.
3. Provide a writing request.
4. Observe the AI conversation area.
5. Locate the actual Draft Editor.
6. Enter text directly into the Draft Editor.

### Expected Result

AI Assistant input and the actual editable Draft Editor should function as separate areas.

### Actual Result

The AI conversation area and Draft Editor were separate.

Direct text entered into the Draft Editor could be observed there, allowing the uppercase behavior and persistence issue to be reproduced.

---

# Test Case Summary

| ID     | Area         | Type                     | Status              |
| ------ | ------------ | ------------------------ | ------------------- |
| TC-001 | Board        | Functional               | PASS                |
| TC-002 | Board        | Functional               | PASS                |
| TC-003 | Board        | Persistence              | PASS                |
| TC-004 | Board        | Functional / Persistence | FAIL                |
| TC-005 | Draft        | Functional / State       | FAIL                |
| TC-006 | Draft / AI   | Functional               | PASS                |
| TC-007 | Draft / AI   | Functional               | FAIL                |
| TC-008 | Draft Editor | Functional / UI          | FAIL                |
| TC-009 | Draft Editor | Persistence              | FAIL                |
| TC-010 | Draft / AI   | Functional               | FAIL                |
| TC-011 | Draft / AI   | State / Context          | FAIL                |
| TC-012 | Plan         | Functional               | PASS                |
| TC-013 | Plan / AI    | Functional               | PASS                |
| TC-014 | Plan / AI    | Functional               | FAIL                |
| TC-015 | Plan         | Persistence              | FAIL                |
| TC-016 | Library      | Functional               | PASS                |
| TC-017 | Library      | UI / Functional          | PASS                |
| TC-018 | Library      | UX                       | UX Recommendation   |
| TC-019 | Poster       | Functional               | PASS                |
| TC-020 | Poster       | Functional / State       | FAIL                |
| TC-021 | Poster       | UI State                 | FAIL                |
| TC-022 | AI Chat      | State                    | FAIL                |
| TC-023 | AI Chat      | State                    | FAIL / Confirmation |
| TC-024 | Templates    | Functional / UX          | PASS / UX           |
| TC-025 | Templates    | UI                       | To Be Confirmed     |
| TC-026 | Split View   | Functional               | FAIL / Reproduced   |
| TC-027 | Draft / Plan | Navigation               | PASS                |
| TC-028 | Draft        | Functional / Workflow    | PASS                |

---

## Test Execution Summary

The test cases above represent the manual testing performed across the main application workflows.

Testing identified issues related to:

* Data persistence
* Draft loading
* Draft Editor behavior
* AI Assistant functionality
* AI-generated content placement
* Conversation context
* Plan content synchronization
* Poster saving
* Poster state
* AI Chat state
* Split View pagination
* UI/UX feedback

Several core workflows passed successfully, including Board drag and drop, Board position persistence, Project opening, Project details display, basic Plan navigation, and Template element dragging.
