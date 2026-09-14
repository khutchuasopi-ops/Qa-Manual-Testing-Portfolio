# Checklists — AI Writing Workspace QA

## 1. Board

* [ ] Board opens successfully.
* [ ] Existing items are displayed correctly.
* [ ] User can open an existing item.
* [ ] User can create a new item.
* [ ] User can edit an existing item.
* [ ] Changes are saved correctly.
* [ ] Delete action is available for applicable items.
* [ ] Deletion behavior matches the intended product behavior.
* [ ] Deleted items are removed from the expected location.
* [ ] No unexpected errors are displayed during Board operations.

---

## 2. Draft Creation and Loading

* [ ] Draft area opens successfully.
* [ ] User can create a new Draft.
* [ ] User can open an existing Draft.
* [ ] Draft content loads correctly.
* [ ] Initial Draft loading behavior is consistent.
* [ ] Loading does not display unexpected application errors.
* [ ] Draft remains accessible after navigating to another workspace area.
* [ ] Draft can be reopened successfully.

---

## 3. Draft Editor

* [ ] Draft Editor opens correctly.
* [ ] User can enter text.
* [ ] Lowercase characters remain lowercase when entered.
* [ ] Uppercase characters remain uppercase when entered.
* [ ] Mixed-case text is preserved.
* [ ] Text can be edited.
* [ ] Edited content remains visible before leaving the page.
* [ ] Editor does not unexpectedly modify user input.
* [ ] No unexpected errors are displayed while editing.

---

## 4. Draft Persistence

* [ ] New Draft content can be created.
* [ ] Draft changes can be saved.
* [ ] Saved content remains available after navigation.
* [ ] Saved content remains available after reopening the Draft.
* [ ] Saved content remains available after page refresh.
* [ ] Refresh does not unexpectedly remove Draft content.
* [ ] Draft state remains consistent when moving between workspace areas.

---

## 5. AI Assistant

* [ ] AI Assistant opens successfully.
* [ ] User can enter a request.
* [ ] AI Assistant responds to the request.
* [ ] Generated content is displayed correctly.
* [ ] Generated content can be used in the Draft workflow.
* [ ] AI-generated content can be inserted into the editable Draft.
* [ ] Generated content does not replace unrelated Draft content.
* [ ] AI Assistant maintains the correct Draft context.
* [ ] Unexpected errors are not displayed during normal AI interaction.

---

## 6. AI Conversation Context

* [ ] Existing conversations can be opened.
* [ ] New conversations can be started.
* [ ] A new Draft starts with the correct conversation context.
* [ ] Previous independent conversations are not incorrectly reused.
* [ ] Switching between Drafts does not mix unrelated conversations.
* [ ] New Chat does not temporarily display a previous conversation.
* [ ] Conversation state remains consistent after entering a new message.
* [ ] Deleted Project conversation behavior matches the intended product behavior.

---

## 7. Plan

* [ ] Plan page opens successfully.
* [ ] User can access Plan functionality from a Draft.
* [ ] Plan content can be created.
* [ ] Plan content is displayed correctly.
* [ ] AI-generated Plan content is reflected on the Plan page.
* [ ] Plan content remains available after navigation.
* [ ] Plan content remains available after page refresh.
* [ ] Plan state is synchronized with the related Draft.
* [ ] Empty Plan states are handled correctly.
* [ ] No unexpected errors are displayed.

---

## 8. Library

* [ ] Library opens successfully.
* [ ] Available Library content is displayed.
* [ ] User can select an existing item.
* [ ] Selected content opens correctly.
* [ ] Library content remains accessible after navigation.
* [ ] No unexpected errors occur when opening Library items.

---

## 9. Templates

* [ ] Templates area opens successfully.
* [ ] Available Templates are displayed.
* [ ] Template content is visible.
* [ ] Template elements can be interacted with as intended.
* [ ] Draggable elements provide clear visual feedback.
* [ ] Drag-and-drop behavior works as expected.
* [ ] Horizontal Template content follows the intended product behavior.
* [ ] Template layout remains usable at the supported screen size.
* [ ] No unexpected content is missing or duplicated.

---

## 10. Poster / Cover

* [ ] Poster/Cover area opens successfully.
* [ ] Existing Poster/Cover content is displayed.
* [ ] User can make changes.
* [ ] Save Poster action is available.
* [ ] Save Poster responds within a reasonable time.
* [ ] Clear feedback is provided after saving.
* [ ] Saved changes remain visible after reopening.
* [ ] Image upload functionality opens correctly.
* [ ] Upload dialog shows the correct current state.
* [ ] Previous images are not incorrectly displayed in a new upload operation.
* [ ] Uploaded images are displayed correctly.

---

## 11. Project / Manuscript Details

* [ ] Project/Manuscript details can be opened.
* [ ] Details content is displayed correctly.
* [ ] Details panel does not hide important information.
* [ ] Panel can be closed successfully.
* [ ] Closing the panel is clear to the user.
* [ ] A visible Close (X) control is available or recommended where appropriate.
* [ ] Opening and closing the panel does not affect unrelated content.

---

## 12. Split View

* [ ] Split View opens successfully.
* [ ] Document content is displayed correctly.
* [ ] Page navigation works.
* [ ] Page numbers correspond to the displayed content.
* [ ] Moving between pages does not duplicate content.
* [ ] Pages do not unexpectedly reset.
* [ ] Pagination remains consistent during repeated navigation.
* [ ] Split View remains usable after several page changes.

---

## 13. Navigation

* [ ] Main workspace areas can be opened.
* [ ] Navigation between areas works correctly.
* [ ] Navigation does not cause unexpected page errors.
* [ ] Returning to a previous area preserves the expected state.
* [ ] Navigation does not incorrectly reuse unrelated content.
* [ ] Browser refresh does not unexpectedly break the current workflow.
* [ ] Main navigation remains usable throughout the workflow.

---

## 14. Data Persistence

* [ ] Newly created content is retained.
* [ ] Edited content is retained.
* [ ] Saved Draft content remains after refresh.
* [ ] Plan content remains after refresh.
* [ ] Changes remain after reopening the relevant area.
* [ ] Data does not unexpectedly disappear after navigation.
* [ ] Data from one Draft does not incorrectly appear in another Draft.
* [ ] Previous conversation data does not incorrectly appear in a new Chat.

---

## 15. UI / UX

* [ ] Buttons are readable in their normal state.
* [ ] Button text remains readable on hover.
* [ ] Interactive elements provide clear visual feedback.
* [ ] Draggable elements indicate that they can be dragged.
* [ ] Close controls are easy to identify.
* [ ] Loading states are understandable.
* [ ] Save actions provide appropriate feedback.
* [ ] Dialogs display the correct current state.
* [ ] No unexpected duplicated content is visible.
* [ ] Layout remains usable during normal interaction.

---

## 16. Error Handling

* [ ] Unexpected application errors are not displayed during normal workflows.
* [ ] Error messages are understandable.
* [ ] Invalid or unsupported actions are handled appropriately.
* [ ] The application does not expose raw technical error messages unnecessarily.
* [ ] Failed actions do not silently remove user data.
* [ ] Failed actions provide appropriate feedback where applicable.
* [ ] The user can continue using the application after a recoverable error.

---

## 17. Smoke Checklist

* [ ] Workspace opens successfully.
* [ ] Board opens.
* [ ] Draft opens.
* [ ] New Draft can be created.
* [ ] Draft Editor is usable.
* [ ] AI Assistant opens.
* [ ] AI Chat opens.
* [ ] Plan opens.
* [ ] Library opens.
* [ ] Templates open.
* [ ] Poster/Cover opens.
* [ ] Project/Manuscript details open.
* [ ] Split View opens.
* [ ] Main navigation works.
* [ ] No blocking error prevents basic workspace usage.

---

## 18. Regression Checklist

After a relevant fix or application update, recheck:

* [ ] Draft content persistence.
* [ ] Draft Editor text case.
* [ ] AI Assistant → Draft content insertion.
* [ ] New Draft conversation context.
* [ ] Plan synchronization.
* [ ] Poster save behavior.
* [ ] Poster image upload state.
* [ ] New Chat conversation state.
* [ ] Split View pagination.
* [ ] Related navigation and persistence behavior.

---

## 19. Testing Notes

* Testing is performed in the staging / preview environment.
* Production is outside the current testing scope.
* Confirmed defects are documented separately in the Bug Reports folder.
* Behaviors that require product clarification are not automatically classified as bugs.
* UX observations are documented separately from functional defects.
* The checklist is intended to support repeatable manual testing and regression checks.
