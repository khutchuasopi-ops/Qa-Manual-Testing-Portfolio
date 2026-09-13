# QA Checklists

## 1. Purpose

This checklist was used to support manual testing of the AI Writing Workspace.

It covers the main application areas, common user flows, AI features, data persistence, UI behavior, and state-related checks.

**Environment:** Staging / Preview
**Testing Type:** Manual Testing
**Production:** Not Tested

---

# 2. Board Checklist

* [x] Board opens successfully
* [x] Board items are visible
* [x] Board items can be moved
* [x] Board items can be moved between sections
* [x] Item position remains after navigation
* [ ] Board item deletion behavior requires product confirmation

---

# 3. Draft Checklist

* [ ] Draft loads correctly on the initial attempt
* [x] Draft can be opened
* [x] AI Assistant is available from Draft
* [ ] AI Assistant request can be submitted without unexpected errors
* [ ] AI Assistant-generated content can be written into an editable Draft
* [ ] Lowercase text remains in the expected case
* [ ] Draft content remains after page refresh
* [ ] New Draft starts with an independent AI conversation context
* [x] Draft and AI Chat inputs remain separate
* [x] Draft → Plan → Draft navigation works

---

# 4. Plan Checklist

* [x] Plan page opens successfully
* [x] AI Assistant is available on the Plan page
* [x] Plan Assistant accepts user input
* [ ] AI-generated Plan is correctly reflected on the Plan page
* [ ] Plan content remains correctly available after refresh

---

# 5. Library and Project Details Checklist

* [x] Library opens
* [x] Project can be opened from Library
* [x] Project Details information is displayed
* [ ] Project Details close control could be clearer
* [ ] Project deletion and related conversation behavior requires product confirmation

---

# 6. Poster Checklist

* [x] Poster area opens
* [x] Image can be uploaded
* [ ] Save action responds without an unnecessary delay
* [ ] Current poster/image is displayed correctly in the upload dialog
* [ ] Poster state remains consistent after saving

---

# 7. AI Chat Checklist

* [x] AI Chat opens
* [x] User can start a conversation
* [ ] New Chat starts without temporarily displaying the previous conversation
* [ ] Conversation behavior after project deletion requires product confirmation

---

# 8. Templates Checklist

* [x] Templates area opens
* [x] Template elements can be selected
* [x] Template elements can be dragged
* [ ] Dragging could provide a clearer grab/grabbing cursor
* [ ] Horizontal Template content behavior requires product confirmation

---

# 9. Split View Checklist

* [x] Split View can be opened
* [x] Content is displayed in the available panes
* [ ] Pagination works consistently between panes
* [ ] Page numbers or controls do not duplicate unexpectedly
* [ ] Pagination does not reset unexpectedly in the second pane

---

# 10. Data Persistence Checklist

* [ ] Draft content remains after refresh
* [ ] Plan content remains correctly available after refresh
* [x] Board item position remains after navigation
* [ ] Poster saved state remains consistent
* [ ] Application state remains consistent after navigation between related areas

---

# 11. AI Workflow Checklist

* [x] AI Assistant is available in the relevant areas
* [x] User can enter AI requests
* [ ] AI-generated content is correctly transferred to an editable Draft
* [ ] New Draft does not incorrectly reuse previous independent conversation context
* [ ] AI-generated Plan is correctly reflected on the Plan page
* [ ] New AI Chat does not temporarily display the previous conversation

---

# 12. Navigation and State Checklist

* [x] Main application areas can be opened
* [x] Library → Project navigation works
* [x] Draft → Plan → Draft navigation works
* [ ] Draft initial loading behavior requires further confirmation
* [ ] AI Chat state is cleared correctly when starting a new chat
* [ ] Application state remains consistent after refresh
* [ ] Split View state remains consistent between panes

---

# 13. UI and Usability Checklist

* [x] Main UI elements are visible
* [x] Project information is readable
* [x] Template elements can be interacted with
* [ ] Project Details close control could be clearer
* [ ] Draggable Template elements could provide a clearer grab/grabbing cursor
* [ ] Text formatting behavior matches expected user input

---

# 14. Defect-Related Checks

The following confirmed defects were identified during testing:

* [ ] BUG-001 — Draft content lost after refresh
* [ ] BUG-002 — Lowercase text automatically entered/displayed as uppercase
* [ ] BUG-003 — AI Assistant fails to write content into an editable Draft
* [ ] BUG-004 — New Draft retains previous independent conversation context
* [ ] BUG-005 — AI-generated Plan not correctly reflected on Plan page
* [ ] BUG-006 — Save Poster delayed/unresponsive
* [ ] BUG-007 — Upload dialog shows previous image instead of current poster
* [ ] BUG-008 — New Chat temporarily displays previous conversation
* [ ] BUG-009 — Split View pagination/page controls duplicated or reset in second pane

**Total Confirmed Bugs:** 9

---

# 15. Product Confirmation Items

The following findings were observed but were not classified as confirmed defects:

* [ ] Board item deletion behavior
* [ ] Initial Draft loading behavior
* [ ] Conversation state after project deletion
* [ ] Horizontal Template content behavior

These items require confirmation of the intended product behavior before being classified as defects.

---

# 16. UX Recommendations

The following usability improvements were identified:

* [ ] Make the Project Details Close/X control clearer
* [ ] Provide a grab/grabbing cursor for draggable Template elements

These recommendations are not counted as confirmed bugs.

---

# 17. Checklist Result

The checklist supported manual testing across the main areas of the AI Writing Workspace.

Testing identified:

* **28 detailed Test Cases**
* **9 confirmed Bug Reports**
* **4 findings requiring Product Confirmation**
* **2 UX recommendations**

Testing was performed in the **Staging / Preview environment**.

The **Production environment was not tested**.
