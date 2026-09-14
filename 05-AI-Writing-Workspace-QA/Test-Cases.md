```markdown
# Test Cases — AI Writing Workspace QA

## 1. Test Case Summary

| Status | Count |
|---|---:|
| PASS | 12 |
| FAIL | 11 |
| Requires Product Confirmation | 4 |
| UX Recommendation Only | 1 |
| **Total** | **28** |

---

## 2. Test Cases

### TC-001 — Board: Open Existing Item

**Priority:** Medium  
**Status:** PASS

**Precondition:** Existing items are available on the Board.

**Steps:**
1. Open the AI Writing Workspace.
2. Navigate to the Board.
3. Select an existing item.
4. Open the item.

**Expected Result:**  
The selected item opens successfully and displays its available content and controls.

**Actual Result:**  
The item opened successfully.

---

### TC-002 — Board: Create New Item

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the Board.
2. Click the option to create a new item.
3. Enter the required information.
4. Save the item.

**Expected Result:**  
A new item is created and appears on the Board.

**Actual Result:**  
The new item was created successfully and appeared on the Board.

---

### TC-003 — Board: Edit Existing Item

**Priority:** Medium  
**Status:** PASS

**Precondition:** An existing Board item is available.

**Steps:**
1. Open the Board.
2. Select an existing item.
3. Edit the available information.
4. Save the changes.

**Expected Result:**  
The changes are saved and remain visible after reopening the item.

**Actual Result:**  
The changes were saved successfully.

---

### TC-004 — Board: Delete Item

**Priority:** High  
**Status:** Requires Product Confirmation

**Steps:**
1. Open the Board.
2. Select an existing item.
3. Choose the delete option.
4. Confirm the deletion if prompted.

**Expected Result:**  
The item should be removed from the Board according to the product's intended deletion behavior.

**Actual Result:**  
The observed deletion behavior requires confirmation of the intended product behavior.

**Note:**  
Product confirmation is required before classifying this behavior as a confirmed defect.

---

### TC-005 — Draft: Initial Loading

**Priority:** Medium  
**Status:** Requires Product Confirmation

**Steps:**
1. Open the AI Writing Workspace.
2. Create or open a Draft.
3. Observe the Draft page while it is loading.
4. Navigate to another relevant page, such as Plan.
5. Return to the Draft.

**Expected Result:**  
The Draft should load correctly when opened.

**Actual Result:**  
The Draft did not initially load as expected. After navigating from Draft to Plan and returning to Draft, the content loaded.

**Note:**  
The expected initial-loading behavior should be confirmed with the product team before treating this as a confirmed defect.

---

### TC-006 — Draft: Create New Draft

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the Draft area.
2. Select the option to create a new Draft.
3. Enter the required information.
4. Create the Draft.

**Expected Result:**  
A new Draft is created successfully.

**Actual Result:**  
The new Draft was created successfully.

---

### TC-007 — Draft: Load Content Without Errors

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open the Draft area.
2. Open an available Draft.
3. Observe the page while the Draft content loads.

**Expected Result:**  
The Draft should load without displaying application errors.

**Actual Result:**  
An `fs_entries` error was displayed while loading the Draft.

**Related Bug Report:**  
No confirmed bug report was created for this observation.

**Note:**  
This is recorded as an observed failure, but it is not included in the confirmed 9-bug set.

---

### TC-008 — Draft Editor: Preserve Text Case

**Priority:** Medium  
**Status:** FAIL

**Steps:**
1. Open a Draft.
2. Click inside the Draft Editor.
3. Enter text using lowercase letters.
4. Observe the entered text.

**Expected Result:**  
The entered text should remain in the same letter case used by the user.

**Actual Result:**  
Lowercase text was automatically converted to uppercase.

**Related Bug Report:**  
BUG-002 — Draft Editor lowercase automatically uppercase

---

### TC-009 — Draft: Preserve Content After Refresh

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open an existing Draft.
2. Add or edit content.
3. Save the Draft if a save action is available.
4. Refresh the page.
5. Check the Draft content.

**Expected Result:**  
Previously saved Draft content should remain available after refreshing the page.

**Actual Result:**  
Draft content was lost after refreshing the page.

**Related Bug Report:**  
BUG-001 — Draft content lost after refresh

---

### TC-010 — AI Assistant: Insert Generated Content Into Draft

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open a Draft.
2. Open the AI Assistant.
3. Enter a request for content.
4. Generate the content.
5. Use the available action to add or write the generated content into the Draft.

**Expected Result:**  
The generated content should be inserted into the editable Draft.

**Actual Result:**  
The AI Assistant failed to write the generated content into the editable Draft.

**Related Bug Report:**  
BUG-003 — AI Assistant fails to write into editable Draft

---

### TC-011 — New Draft: Conversation Context

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open an existing Draft and use an independent AI conversation.
2. Create a new Draft.
3. Open the AI conversation for the new Draft.
4. Observe the conversation context.

**Expected Result:**  
A new Draft should start with its own conversation context and should not use unrelated context from a previous independent conversation.

**Actual Result:**  
The new Draft retained the previous independent conversation context.

**Related Bug Report:**  
BUG-004 — New Draft retains previous independent conversation context

---

### TC-012 — Plan: Open Plan Page

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open a Draft.
2. Navigate to the Plan page.
3. Observe the page.

**Expected Result:**  
The Plan page opens successfully.

**Actual Result:**  
The Plan page opened successfully.

---

### TC-013 — Plan: Create Plan Content

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the Plan page.
2. Create or generate Plan content.
3. Save the content.

**Expected Result:**  
The Plan content is created and saved successfully.

**Actual Result:**  
Plan content was created successfully.

---

### TC-014 — Plan: Display AI-Generated Content

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open a Draft.
2. Generate Plan content using the available AI functionality.
3. Open the Plan page.
4. Observe the generated content.

**Expected Result:**  
AI-generated Plan content should be reflected on the Plan page.

**Actual Result:**  
The AI-generated Plan content was not reflected on the Plan page.

**Related Bug Report:**  
BUG-005 — AI-generated Plan content not reflected on Plan page

---

### TC-015 — Plan: Preserve Generated Content After Refresh

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Generate Plan content.
2. Open the Plan page.
3. Refresh the page.
4. Check the Plan content.

**Expected Result:**  
Previously generated or saved Plan content should remain visible after refreshing the page.

**Actual Result:**  
The Plan page was empty after the refresh.

**Related Bug Report:**  
BUG-005 — AI-generated Plan content not reflected on Plan page

---

### TC-016 — Library: Open Library

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the AI Writing Workspace.
2. Navigate to Library.
3. Observe the available content.

**Expected Result:**  
The Library opens and available content is displayed.

**Actual Result:**  
The Library opened successfully.

---

### TC-017 — Library: Open Existing Content

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open Library.
2. Select an existing item.
3. Open the item.

**Expected Result:**  
The selected Library item opens successfully.

**Actual Result:**  
The item opened successfully.

---

### TC-018 — Templates: Drag-and-Drop Element

**Priority:** Low  
**Status:** UX Recommendation Only

**Steps:**
1. Open the Templates area.
2. Select a Template containing draggable elements.
3. Attempt to drag an element to another position.

**Expected Result:**  
The interface should clearly indicate which elements can be dragged.

**Actual Result:**  
The draggable behavior was available, but the cursor did not clearly communicate that the element could be dragged.

**UX Recommendation:**  
Use a grab cursor for draggable Template elements to make the interaction more understandable.

**Related UX Recommendation:**  
UX-001 — Grab cursor for draggable Template elements

---

### TC-019 — Poster: Open Poster/Cover

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open a relevant Project or Draft.
2. Navigate to Poster/Cover.
3. Open the Poster/Cover area.

**Expected Result:**  
The Poster/Cover area opens successfully.

**Actual Result:**  
The Poster/Cover area opened successfully.

---

### TC-020 — Poster: Save Changes

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open Poster/Cover.
2. Make a change.
3. Click the Save Poster action.
4. Observe the response.

**Expected Result:**  
The changes should be saved immediately or within a reasonable response time, with clear feedback that the save was completed.

**Actual Result:**  
The Save Poster action was delayed or appeared unresponsive.

**Related Bug Report:**  
BUG-006 — Save Poster action delayed/unresponsive

---

### TC-021 — Poster: Upload Image

**Priority:** Medium  
**Status:** FAIL

**Steps:**
1. Open Poster/Cover.
2. Select the option to upload an image.
3. Open the upload dialog.
4. Observe the image displayed in the dialog.

**Expected Result:**  
The upload dialog should display the current upload state and should not show an unrelated image from a previous operation.

**Actual Result:**  
The upload dialog displayed the previous image.

**Related Bug Report:**  
BUG-007 — Upload dialog shows previous image

---

### TC-022 — AI Chat: Start New Chat

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open AI Chat.
2. Start a new chat.
3. Observe the conversation before entering new text.
4. Enter a new message.

**Expected Result:**  
A new chat should start with a clean conversation state and should not temporarily display messages from a previous conversation.

**Actual Result:**  
The previous conversation was temporarily displayed until new text was entered.

**Related Bug Report:**  
BUG-008 — New Chat temporarily shows previous conversation

---

### TC-023 — Deleted Project: Conversation Availability

**Priority:** High  
**Status:** Requires Product Confirmation

**Steps:**
1. Open a Project with an existing conversation.
2. Delete the Project.
3. Navigate to the relevant conversation or AI Chat area.
4. Check whether the deleted Project's conversation is still accessible.

**Expected Result:**  
The conversation availability after Project deletion should follow the product's intended behavior.

**Actual Result:**  
The observed behavior requires confirmation of the expected product behavior.

**Note:**  
Product confirmation is required before classifying this as a confirmed defect.

---

### TC-024 — Project/Manuscript Details: Close Panel

**Priority:** Low  
**Status:** PASS

**Steps:**
1. Open a Project or Manuscript.
2. Open the details panel.
3. Observe the available controls for closing the panel.

**Expected Result:**  
The details panel should provide a clear and convenient way to close it.

**Actual Result:**  
The panel could be closed, but the interface would be clearer with a dedicated Close (X) button.

**UX Recommendation:**  
Add a visible Close (X) button to the Project/Manuscript details panel.

**Related UX Recommendation:**  
UX-002 — Close X for Project/Manuscript details panel

---

### TC-025 — Templates: Horizontal Content

**Priority:** Medium  
**Status:** Requires Product Confirmation

**Steps:**
1. Open the Templates area.
2. Open a Template containing the observed horizontal content.
3. Review the content layout.
4. Check whether the content can be accessed or displayed as intended.

**Expected Result:**  
Template content should follow the intended product layout and interaction behavior.

**Actual Result:**  
Horizontal Template content was observed, but the expected product behavior is not sufficiently clear to classify it as a confirmed defect.

**Note:**  
Product confirmation is required.

---

### TC-026 — Split View: Pagination

**Priority:** High  
**Status:** FAIL

**Steps:**
1. Open a document in Split View.
2. Navigate between pages.
3. Observe the page numbers and displayed content.
4. Continue navigating through the available pages.

**Expected Result:**  
Pagination should remain consistent, with the correct page number and corresponding content displayed.

**Actual Result:**  
Split View pagination broke and pages were duplicated or reset during navigation.

**Related Bug Report:**  
BUG-009 — Split View pagination/page breaks duplicated/reset

---

### TC-027 — Navigation: Move Between Main Areas

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the AI Writing Workspace.
2. Navigate between the main available areas.
3. Open each selected area.

**Expected Result:**  
Navigation between the main areas should work without unexpected errors.

**Actual Result:**  
Navigation worked successfully.

---

### TC-028 — UI: General Workspace Interaction

**Priority:** Medium  
**Status:** PASS

**Steps:**
1. Open the AI Writing Workspace.
2. Navigate through the main interface.
3. Interact with available controls.
4. Observe the general UI behavior.

**Expected Result:**  
The interface should remain usable and responsive during normal interaction.

**Actual Result:**  
The general interface was usable during normal interaction.

---

# 3. Confirmed Bug Traceability

| Bug ID | Bug | Related Test Case(s) |
|---|---|---|
| BUG-001 | Draft content lost after refresh | TC-009 |
| BUG-002 | Draft Editor lowercase automatically uppercase | TC-008 |
| BUG-003 | AI Assistant fails to write into editable Draft | TC-010 |
| BUG-004 | New Draft retains previous independent conversation context | TC-011 |
| BUG-005 | AI-generated Plan content not reflected on Plan page | TC-014, TC-015 |
| BUG-006 | Save Poster action delayed/unresponsive | TC-020 |
| BUG-007 | Upload dialog shows previous image | TC-021 |
| BUG-008 | New Chat temporarily shows previous conversation | TC-022 |
| BUG-009 | Split View pagination/page breaks duplicated/reset | TC-026 |

**Total Confirmed Bugs:** 9

---

# 4. Product Confirmation Items

The following observations were recorded during testing but should not be counted as confirmed defects until the intended product behavior is confirmed:

| Test Case | Observation |
|---|---|
| TC-004 | Board item deletion behavior |
| TC-005 | Draft initial loading behavior |
| TC-023 | Conversation availability after Project deletion |
| TC-025 | Horizontal Template content behavior |

**Total:** 4

---

# 5. UX Recommendations

| ID | Recommendation | Related Test Case |
|---|---|---|
| UX-001 | Add a grab cursor for draggable Template elements | TC-018 |
| UX-002 | Add a visible Close (X) button to the Project/Manuscript details panel | TC-024 |

**Total UX Recommendations:** 2

---

# 6. Final Execution Summary

| Category | Count |
|---|---:|
| PASS | 12 |
| FAIL | 11 |
| Requires Product Confirmation | 4 |
| UX Recommendation Only | 1 |
| **Total Test Cases** | **28** |
| Confirmed Bugs | **9** |
| UX Recommendations | **2** |

## Notes

- TC-007 is recorded as a failed test because the `fs_entries` error was observed, but no separate confirmed bug report is included for it.
- TC-004, TC-005, TC-023 and TC-025 require product confirmation and are therefore not counted as confirmed defects.
- TC-018 is recorded as a UX Recommendation Only because the observed behavior did not prevent the workflow from being completed.
- TC-024 passed functionally but resulted in a UX recommendation for a clearer close control.
- The project was tested in the staging/preview environment. Production was not included in the testing scope.
```
