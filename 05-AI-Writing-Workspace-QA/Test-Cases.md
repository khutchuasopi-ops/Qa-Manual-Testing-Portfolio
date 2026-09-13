# Test Cases

## 1. Purpose

This document contains the detailed manual test cases used for testing the AI Writing Workspace.

The test cases cover the main user flows, AI-assisted writing features, data persistence, navigation, UI behavior, and state handling.

Testing was performed in the Staging/Preview environment.

---

## 2. Test Case Statuses

| Status                        | Meaning                                                                |
| ----------------------------- | ---------------------------------------------------------------------- |
| PASS                          | Expected behavior was observed                                         |
| FAIL                          | Actual behavior did not match the expected result                      |
| Requires Product Confirmation | The behavior needs clarification or confirmation from the product team |
| UX Recommendation             | The functionality works, but a usability improvement was identified    |

---

# 3. Board

## TC-001 — Move a Board Item

**Scenario:** Board item positioning

**Preconditions:**

* User is on the Board page.
* At least one movable item is available.

**Steps:**

1. Open the Board.
2. Select a board item.
3. Drag the item to another position.
4. Release the item.

**Expected Result:**

* The item moves to the selected position.
* No unrelated board items are affected.

**Actual Result:**

* The item was moved successfully.

**Status:** PASS

---

## TC-002 — Move a Board Item to Another Section

**Scenario:** Board section management

**Preconditions:**

* Board contains multiple sections.
* A movable item is available.

**Steps:**

1. Open the Board.
2. Select an item.
3. Drag the item to another section.
4. Release the item.

**Expected Result:**

* The item is moved to the selected section.

**Actual Result:**

* The item was moved successfully.

**Status:** PASS

---

## TC-003 — Verify Board Position Persistence

**Scenario:** Board data persistence

**Preconditions:**

* A board item has been moved.

**Steps:**

1. Move a board item to a different position.
2. Leave the Board.
3. Return to the Board.
4. Check the item's position.

**Expected Result:**

* The item's position remains unchanged after returning to the Board.

**Actual Result:**

* The item position was retained.

**Status:** PASS

---

## TC-004 — Delete a Board Item

**Scenario:** Board item deletion

**Preconditions:**

* A deletable board item is available.

**Steps:**

1. Open the Board.
2. Select a board item.
3. Use the available delete action.
4. Confirm the action if confirmation is displayed.
5. Check the Board.

**Expected Result:**

* The selected item is removed from the Board.
* The behavior is consistent with the expected product behavior.

**Actual Result:**

* The deletion behavior requires product confirmation.

**Status:** Requires Product Confirmation

**Related Bug:** None

---

# 4. Draft

## TC-005 — Open Draft Page

**Scenario:** Draft loading

**Steps:**

1. Open the Draft area.
2. Observe the page during initial loading.
3. Wait for the Draft content to load.
4. Navigate to another relevant area and return to Draft if needed.

**Expected Result:**

* The Draft page loads normally.
* Existing Draft content is available.

**Actual Result:**

* The Draft did not load correctly on the initial attempt.
* After navigating through the Plan flow and returning to Draft, the content became available.

**Status:** Requires Product Confirmation

**Related Bug:** None

---

## TC-006 — Interact with AI Assistant from Draft

**Scenario:** AI Assistant interaction

**Steps:**

1. Open a Draft.
2. Open the AI Assistant.
3. Enter a valid request.
4. Submit the request.

**Expected Result:**

* The request is accepted.
* The AI Assistant processes the request and provides a response.

**Actual Result:**

* The basic interaction flow was available.

**Status:** PASS

---

## TC-007 — Enter a Request in AI Assistant

**Scenario:** AI Assistant text input

**Steps:**

1. Open the Draft.
2. Open the AI Assistant.
3. Enter a request in the input field.
4. Submit the request.

**Expected Result:**

* The entered request is accepted and processed normally.

**Actual Result:**

* An error related to `fs_entries` was observed during the interaction.

**Status:** FAIL

**Related Bug:** None directly assigned

**Note:** The observed behavior was recorded during testing. The confirmed defect related to AI-generated editable Draft creation is documented separately as BUG-003.

---

## TC-008 — Verify Draft Editor Text Case

**Scenario:** Draft Editor text formatting

**Steps:**

1. Open the Draft Editor.
2. Enter text using lowercase characters.
3. Observe the entered text.

**Expected Result:**

* The entered text remains in the same case used by the user.

**Actual Result:**

* Lowercase text was automatically entered/displayed as uppercase.

**Status:** FAIL

**Related Bug:** BUG-002

---

## TC-009 — Verify Draft Content Persistence After Refresh

**Scenario:** Draft persistence

**Steps:**

1. Open a Draft.
2. Enter or modify Draft content.
3. Save the content if a save action is available.
4. Refresh the page.
5. Check the Draft content.

**Expected Result:**

* Previously saved Draft content remains available after refresh.

**Actual Result:**

* Draft content was lost after refresh.

**Status:** FAIL

**Related Bug:** BUG-001

---

## TC-010 — Create an Editable Draft Using AI Assistant

**Scenario:** AI-generated Draft creation

**Steps:**

1. Open the AI Assistant.
2. Submit a request to generate Draft content.
3. Wait for the AI response.
4. Check whether the generated content is placed into an editable Draft.

**Expected Result:**

* AI-generated content is written into a Draft that the user can edit.

**Actual Result:**

* The AI Assistant failed to write the generated content into an editable Draft.

**Status:** FAIL

**Related Bug:** BUG-003

---

## TC-011 — Verify New Draft Conversation Context

**Scenario:** AI context isolation

**Steps:**

1. Open an existing Draft and interact with the AI Assistant.
2. Create a new Draft.
3. Start a new AI Assistant interaction in the new Draft.
4. Check whether information from the previous independent conversation is used.

**Expected Result:**

* The new Draft starts with an independent AI conversation context.

**Actual Result:**

* The new Draft retained context from the previous independent conversation.

**Status:** FAIL

**Related Bug:** BUG-004

---

# 5. Plan

## TC-012 — Open Plan Page

**Scenario:** Plan page access

**Steps:**

1. Open the project.
2. Navigate to the Plan page.
3. Observe the page.

**Expected Result:**

* The Plan page opens successfully.
* Existing Plan information is displayed.

**Actual Result:**

* The Plan page opened successfully.

**Status:** PASS

---

## TC-013 — Enter a Request in Plan Assistant

**Scenario:** Plan AI Assistant

**Steps:**

1. Open the Plan page.
2. Open the AI Assistant.
3. Enter a valid request.
4. Submit the request.

**Expected Result:**

* The request is accepted.
* The AI Assistant provides a response.

**Actual Result:**

* The request was accepted and the assistant interaction was available.

**Status:** PASS

---

## TC-014 — Verify AI-Generated Plan Appears on Plan Page

**Scenario:** AI-generated Plan

**Steps:**

1. Open the Plan page.
2. Use the AI Assistant to generate a Plan.
3. Wait for the generation to complete.
4. Return to the Plan page content.

**Expected Result:**

* The generated Plan is reflected on the Plan page.

**Actual Result:**

* The AI-generated Plan was not correctly reflected on the Plan page.

**Status:** FAIL

**Related Bug:** BUG-005

---

## TC-015 — Verify Plan Content After Refresh

**Scenario:** Plan persistence

**Steps:**

1. Generate or update Plan content.
2. Confirm the Plan content is displayed.
3. Refresh the page.
4. Check the Plan content again.

**Expected Result:**

* The generated Plan content remains available after refresh.

**Actual Result:**

* The Plan content was not correctly retained/reflected after refresh.

**Status:** FAIL

**Related Bug:** BUG-005

---

# 6. Library and Project Details

## TC-016 — Open a Project from Library

**Scenario:** Library project access

**Steps:**

1. Open the Library.
2. Select an available project.
3. Open the project.

**Expected Result:**

* The selected project opens successfully.

**Actual Result:**

* The project opened successfully.

**Status:** PASS

---

## TC-017 — Verify Project Details Information

**Scenario:** Project details

**Steps:**

1. Open a project.
2. Open the Project Details panel.
3. Review the displayed project information.

**Expected Result:**

* The Project Details panel displays the relevant project information correctly.

**Actual Result:**

* The expected project information was displayed.

**Status:** PASS

---

## TC-018 — Close Project Details Panel

**Scenario:** Project Details usability

**Steps:**

1. Open a project.
2. Open the Project Details panel.
3. Review the available controls for closing the panel.

**Expected Result:**

* The panel can be closed easily using a clear and visible control.

**Actual Result:**

* The panel can be closed, but a clearer Close/X control would improve usability.

**Status:** UX Recommendation

**Related Bug:** None

---

# 7. Poster

## TC-019 — Upload an Image for Poster

**Scenario:** Poster image upload

**Steps:**

1. Open the Poster area.
2. Select the image upload option.
3. Choose a valid image.
4. Confirm the upload.

**Expected Result:**

* The selected image is uploaded and displayed correctly.

**Actual Result:**

* The image upload completed successfully.

**Status:** PASS

---

## TC-020 — Save Poster

**Scenario:** Poster saving

**Steps:**

1. Open the Poster area.
2. Create or update a poster.
3. Select the Save action.
4. Observe the result.

**Expected Result:**

* The poster is saved without an unnecessary delay.
* The saved state is reflected immediately or within the expected time.

**Actual Result:**

* The Save action was delayed/unresponsive before the updated state appeared.

**Status:** FAIL

**Related Bug:** BUG-006

---

## TC-021 — Verify Current Poster in Upload Dialog

**Scenario:** Poster image state

**Steps:**

1. Open the Poster area.
2. Create or update the current poster.
3. Open the upload dialog.
4. Observe the displayed image.

**Expected Result:**

* The upload dialog displays the current poster/image state.

**Actual Result:**

* The dialog displayed the previous image instead of the current poster.

**Status:** FAIL

**Related Bug:** BUG-007

---

# 8. AI Chat

## TC-022 — Verify New Chat Starts Without Previous Conversation

**Scenario:** New AI Chat

**Steps:**

1. Open AI Chat.
2. Start a conversation.
3. Create a New Chat.
4. Observe the conversation displayed in the new chat.

**Expected Result:**

* The new chat starts without displaying the previous conversation.

**Actual Result:**

* The previous conversation was temporarily displayed in the new chat.

**Status:** FAIL

**Related Bug:** BUG-008

---

## TC-023 — Verify Conversation State After Project Deletion

**Scenario:** Deleted project conversation

**Steps:**

1. Open a project with an AI conversation.
2. Delete the project or perform the relevant deletion action.
3. Open AI Chat.
4. Check whether the deleted project's conversation is still available.

**Expected Result:**

* Conversation availability after project deletion should follow the defined product behavior.

**Actual Result:**

* The observed behavior requires product confirmation.

**Status:** Requires Product Confirmation

**Related Bug:** None

---

# 9. Templates

## TC-024 — Drag Template Element

**Scenario:** Template element positioning

**Steps:**

1. Open the Templates area.
2. Select a draggable template element.
3. Drag the element to another position.
4. Release it.

**Expected Result:**

* The element can be moved as expected.
* The interaction is clear to the user.

**Actual Result:**

* The element could be dragged successfully.

**Status:** PASS

**Related Bug:** None

**UX Recommendation:** A grab/grabbing cursor could make the draggable behavior clearer.

---

## TC-025 — Verify Horizontal Template Content

**Scenario:** Template content layout

**Steps:**

1. Open a template containing horizontal content.
2. Review the content and its layout.
3. Check whether all relevant content is accessible.

**Expected Result:**

* The content is displayed and accessible according to the intended design.

**Actual Result:**

* The behavior requires confirmation of the intended product design.

**Status:** Requires Product Confirmation

**Related Bug:** None

---

# 10. Split View

## TC-026 — Verify Split View Pagination

**Scenario:** Split View pagination

**Steps:**

1. Open Split View.
2. Display content in both panes.
3. Navigate between pages.
4. Observe the pagination controls and page content.
5. Repeat the navigation to confirm the behavior.

**Expected Result:**

* Pagination works independently and consistently in the relevant pane.
* Page numbers and controls do not duplicate or reset unexpectedly.

**Actual Result:**

* Pagination/page controls were duplicated or reset in the second pane.
* The behavior was reproduced during testing.

**Status:** FAIL

**Related Bug:** BUG-009

---

# 11. Cross-Flow

## TC-027 — Navigate from Draft to Plan and Back to Draft

**Scenario:** Draft → Plan → Draft workflow

**Steps:**

1. Open a Draft.
2. Navigate to Plan.
3. Perform the available Plan interaction.
4. Navigate back to Draft.
5. Check the Draft state.

**Expected Result:**

* Navigation between Draft and Plan works normally.
* The user can return to Draft without losing the expected state.

**Actual Result:**

* The Draft → Plan → Draft flow completed successfully.

**Status:** PASS

---

## TC-028 — Verify Draft Editor and AI Chat Inputs Are Separate

**Scenario:** Input separation

**Steps:**

1. Open a Draft.
2. Enter text in the Draft Editor.
3. Open AI Chat.
4. Enter a separate message in the AI Chat input.
5. Compare the two inputs.

**Expected Result:**

* Draft Editor content and AI Chat input remain separate.
* Text entered in one input does not unexpectedly appear in the other.

**Actual Result:**

* The Draft Editor and AI Chat inputs remained separate.

**Status:** PASS

---

# 12. Confirmed Bug Traceability

Only confirmed defects documented in the project's Bug Reports are included in this table.

| Bug ID  | Related Test Case(s) | Area                          |
| ------- | -------------------- | ----------------------------- |
| BUG-001 | TC-009               | Draft persistence             |
| BUG-002 | TC-008               | Draft Editor text case        |
| BUG-003 | TC-010               | AI Assistant / Draft creation |
| BUG-004 | TC-011               | New Draft / AI context        |
| BUG-005 | TC-014, TC-015       | Plan / AI-generated content   |
| BUG-006 | TC-020               | Poster saving                 |
| BUG-007 | TC-021               | Poster image state            |
| BUG-008 | TC-022               | AI Chat state                 |
| BUG-009 | TC-026               | Split View pagination         |

---

# 13. Findings Requiring Product Confirmation

The following observations were recorded during testing but are **not counted as confirmed defects** until the expected product behavior is confirmed.

| Test Case | Finding                                                             |
| --------- | ------------------------------------------------------------------- |
| TC-004    | Board item deletion behavior requires product confirmation          |
| TC-005    | Draft initial loading behavior requires product confirmation        |
| TC-023    | Deleted project conversation behavior requires product confirmation |
| TC-025    | Horizontal Template content behavior requires product confirmation  |

---

# 14. UX Recommendations

The following observations are usability recommendations and are not counted as defects.

| Test Case | Recommendation                                             |
| --------- | ---------------------------------------------------------- |
| TC-018    | Add or make the Project Details Close/X control clearer    |
| TC-024    | Use a grab/grabbing cursor for draggable Template elements |

---

# 15. Test Case Summary

| Area                      | Test Cases |
| ------------------------- | ---------: |
| Board                     |          4 |
| Draft                     |          7 |
| Plan                      |          4 |
| Library / Project Details |          3 |
| Poster                    |          3 |
| AI Chat                   |          2 |
| Templates                 |          2 |
| Split View                |          1 |
| Cross-Flow                |          2 |
| **Total**                 |     **28** |

---

## 16. Confirmed Defect Summary

| Bug ID  | Related Test Case(s) |
| ------- | -------------------- |
| BUG-001 | TC-009               |
| BUG-002 | TC-008               |
| BUG-003 | TC-010               |
| BUG-004 | TC-011               |
| BUG-005 | TC-014, TC-015       |
| BUG-006 | TC-020               |
| BUG-007 | TC-021               |
| BUG-008 | TC-022               |
| BUG-009 | TC-026               |

**Total Confirmed Bugs:** 9
