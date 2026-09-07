# QA Checklists

## Overview

This checklist summarizes the manual QA checks performed on the AI Writing Workspace in a staging/preview environment.

The checklist covers the main application areas, core workflows, persistence, navigation, AI functionality, state management, and UI/UX behavior.

---

# 1. Board Checklist

- [x] Open Board
- [x] Verify existing Board items are displayed
- [x] Drag and drop an item
- [x] Move an item to another position
- [x] Move an item to another section
- [x] Verify item position after drag and drop
- [x] Refresh after moving an item
- [x] Verify item position persists after refresh
- [x] Delete an existing item
- [x] Verify item disappears after deletion
- [x] Refresh after deleting an item
- [x] Verify deleted item does not return

### Result

**PASS:** Drag and drop, moving items, and position persistence.

**FAIL:** Deleted item remained visible after deletion and refresh.

---

# 2. Draft Checklist

## Draft Opening

- [x] Open a Project / Manuscript
- [x] Navigate to Draft
- [x] Observe initial Draft loading
- [x] Wait for Draft to load
- [x] Navigate from Draft to Plan
- [x] Navigate back to Draft
- [x] Verify Draft loading after returning

### Result

**FAIL:** Draft initially remained in a loading state and loaded correctly only after navigating away and returning.

---

## AI Assistant

- [x] Open Draft
- [x] Wait for AI Assistant
- [x] Verify initial AI question
- [x] Enter a writing topic
- [x] Submit the message
- [x] Observe AI response
- [x] Verify AI Assistant error behavior
- [x] Ask AI Assistant to write content
- [x] Ask AI Assistant to create/update Draft content
- [x] Verify generated content is placed in the Draft
- [x] Verify generated content is editable
- [x] Test a second writing request
- [x] Verify AI Assistant behavior after follow-up prompts

### Result

**PASS:** Initial AI question displayed correctly.

**FAIL:** AI Assistant returned errors and could not reliably create or place content into an editable Draft.

---

## Draft Editor

- [x] Open actual Draft Editor
- [x] Enter text directly into the editor
- [x] Verify lowercase text entry
- [x] Test with Caps Lock turned off
- [x] Test without holding Shift
- [x] Observe text while typing
- [x] Verify capitalization behavior
- [x] Refresh after entering content
- [x] Verify entered content after refresh

### Result

**FAIL:** Lowercase text appeared as uppercase while typing.

**FAIL:** Draft content disappeared after refresh.

---

## New Draft Context

- [x] Open a new Draft
- [x] Observe initial AI question
- [x] Enter an unrelated new topic
- [x] Continue the conversation
- [x] Observe AI context
- [x] Verify previous independent document context is not used

### Result

**FAIL:** The new Draft referenced unrelated information from a previous independent document/conversation.

---

# 3. Plan Checklist

- [x] Open Project / Manuscript
- [x] Navigate to Plan
- [x] Verify Plan page opens
- [x] Verify Assistant input is available
- [x] Enter a planning request
- [x] Submit planning request
- [x] Observe AI-generated planning options
- [x] Verify Assistant indicates Plan will be updated
- [x] Check whether generated content appears on Plan
- [x] Refresh Plan
- [x] Verify Plan content after refresh

### Result

**PASS:** Plan page opened successfully and Assistant accepted the planning request.

**FAIL:** AI-generated planning content was not reflected on the Plan page and remained empty after refresh.

---

# 4. Library Checklist

- [x] Open Library
- [x] Select an existing Project / Manuscript
- [x] Open Project / Manuscript
- [x] Verify Project details
- [x] Verify About information
- [x] Verify Author information
- [x] Verify Category information
- [x] Verify Date information
- [x] Verify Description
- [x] Verify Companion instructions
- [x] Close the details panel by clicking outside

### Result

**PASS:** Project opening and details display.

**UX Recommendation:** Consider adding a visible Close (X) button to the details panel.

---

# 5. Poster / Cover Checklist

- [x] Open Project / Manuscript
- [x] Select Edit
- [x] Open Upload
- [x] Select an image
- [x] Verify selected image
- [x] Click Save Poster
- [x] Observe immediate response
- [x] Wait for poster update
- [x] Verify poster eventually updates
- [x] Open upload dialog again
- [x] Verify displayed poster image

### Result

**PASS:** Image selection/upload worked.

**FAIL:** Save Poster did not respond immediately and the poster update was delayed.

**FAIL:** Upload dialog displayed a previously uploaded image instead of the current poster.

---

# 6. AI Chat Checklist

## New Chat

- [x] Open AI Chat
- [x] Start New Chat
- [x] Observe conversation before entering new text
- [x] Enter new text
- [x] Observe conversation after entering new text
- [x] Verify previous conversation disappears

### Result

**FAIL:** Previous conversation remained visible until new text was entered.

---

## Deleted Project Conversation

- [x] Open Project / Manuscript
- [x] Verify existing AI Chat conversation
- [x] Delete Project / Manuscript
- [x] Open AI Chat dropdown
- [x] Check conversation list
- [x] Verify whether deleted Project conversation remains

### Result

**FAIL / Requires Product Confirmation:** Conversation associated with the deleted Project remained visible.

---

# 7. Templates Checklist

- [x] Open Template
- [x] Locate draggable text element
- [x] Hover over draggable element
- [x] Verify cursor behavior
- [x] Drag element
- [x] Move element to another position
- [x] Release element
- [x] Verify element moved successfully

### Result

**PASS:** Draggable element functionality worked.

**UX Recommendation:** Consider adding a grab/hand cursor to make draggable behavior clearer.

---

# 8. Split View Checklist

- [x] Open Project / Manuscript
- [x] Open Draft
- [x] Verify Draft contains multiple pages/content
- [x] Open same Draft in Split View
- [x] Observe both panes
- [x] Compare pagination
- [x] Compare page breaks
- [x] Verify pagination consistency
- [x] Repeat the workflow
- [x] Reproduce the issue

### Result

**FAIL — Reproduced:** Pagination/page breaks were duplicated or reset on the second side when the same Draft was opened in Split View.

---

# 9. Navigation Checklist

- [x] Library → Project / Manuscript
- [x] Project → Draft
- [x] Draft → Plan
- [x] Plan → Draft
- [x] Project → AI Chat
- [x] Open same Draft in Split View
- [x] Navigate away from Draft
- [x] Return to Draft
- [x] Verify application remains accessible after navigation

### Result

Core navigation worked.

Navigation between Draft and Plan also provided a workaround for the initial Draft loading issue.

---

# 10. Refresh / Persistence Checklist

- [x] Enter Draft content
- [x] Refresh Draft
- [x] Verify Draft content
- [x] Move Board item
- [x] Refresh Board
- [x] Verify item position
- [x] Delete Board item
- [x] Refresh Board
- [x] Verify deleted item
- [x] Send Plan request
- [x] Refresh Plan
- [x] Verify Plan content
- [x] Save Poster
- [x] Reopen poster workflow
- [x] Verify current poster state

### Result

Several persistence/state issues were identified.

---

# 11. AI Context and State Checklist

- [x] Start AI interaction
- [x] Submit a writing topic
- [x] Continue with follow-up input
- [x] Start a new Draft
- [x] Enter unrelated topic
- [x] Check AI context
- [x] Start New Chat
- [x] Check previous conversation state
- [x] Enter new message
- [x] Verify conversation refresh
- [x] Delete Project
- [x] Check AI Chat dropdown
- [x] Verify related conversation state

### Result

Context and conversation state issues were identified.

---

# 12. UI / UX Checklist

- [x] Verify Project details panel behavior
- [x] Verify panel closing behavior
- [x] Check for visible Close (X) button
- [x] Verify draggable Template cursor
- [x] Check whether drag interaction provides visual feedback
- [x] Observe Save Poster feedback
- [x] Observe Draft loading feedback
- [x] Observe AI Assistant error feedback
- [x] Observe New Chat state transition
- [x] Observe Split View pagination behavior

### UX Findings

- Project details panel could benefit from a visible Close (X) button.
- Draggable Template elements could benefit from a grab/hand cursor.
- Save Poster could provide clearer immediate feedback while the change is being processed.

---

# 13. Regression Checks

The following workflows were repeated after issues were identified:

- [x] Draft → Plan → Draft
- [x] Board drag and drop
- [x] Board refresh after moving an item
- [x] Board refresh after deletion
- [x] Draft refresh after entering content
- [x] AI Assistant writing workflow
- [x] New Draft context behavior
- [x] New Chat behavior
- [x] Poster save behavior
- [x] Poster upload dialog behavior
- [x] Split View behavior

---

# 14. Evidence Checklist

Evidence should be collected and organized for reproducible issues.

## Board

- [ ] Deleted item screenshot
- [ ] Deleted item after refresh screenshot/video

## Draft

- [ ] Draft loading screen recording
- [ ] AI Assistant error screenshot
- [ ] AI Assistant Draft creation evidence
- [ ] Draft uppercase behavior screen recording
- [ ] Draft content disappearing after refresh
- [ ] New Draft context evidence

## Plan

- [ ] AI-generated Plan options screenshot
- [ ] Empty Plan after AI response
- [ ] Empty Plan after refresh

## AI Chat

- [ ] Previous conversation visible in New Chat
- [ ] Deleted Project conversation visible in dropdown

## Poster

- [ ] Save Poster delayed response
- [ ] Poster eventually updated
- [ ] Previous image displayed in upload dialog

## Split View

- [ ] Split View pagination/page break issue
- [ ] Reproduction screen recording

---

# 15. Overall Checklist Result

### Functional Testing

- [x] Core Board functionality tested
- [x] Draft functionality tested
- [x] Plan functionality tested
- [x] AI Chat tested
- [x] Library tested
- [x] Poster functionality tested
- [x] Templates tested
- [x] Split View tested

### State Testing

- [x] Refresh behavior tested
- [x] Navigation state tested
- [x] New Chat state tested
- [x] New Draft context tested
- [x] Deleted Project state tested
- [x] Split View state tested

### Persistence Testing

- [x] Board item position
- [x] Board deletion
- [x] Draft content
- [x] Plan content
- [x] Poster state

### AI Testing

- [x] Initial AI interaction
- [x] AI user input
- [x] AI-generated writing
- [x] AI Draft creation
- [x] AI Plan generation
- [x] New Draft context
- [x] New Chat context

### UX Testing

- [x] Project details panel
- [x] Template drag cursor
- [x] Save Poster feedback
- [x] Draft loading feedback
- [x] AI error feedback
- [x] Split View behavior

---

## Final Checklist Status

**Testing Type:** Manual QA

**Environment:** Staging / Preview

**Primary Focus:** Functional, Exploratory, Persistence, State, AI, UI/UX

**Production:** Not tested

**Result:** Multiple functional and state-related issues identified and documented.
