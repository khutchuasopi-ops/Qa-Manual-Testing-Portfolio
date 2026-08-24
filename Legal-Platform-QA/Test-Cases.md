# Test Cases

This document contains manual test cases created to verify the main functionality of the application.

The test cases cover positive scenarios, negative scenarios, input validation, file management, UI behavior, search, filtering, and error handling.

---

## 1. Dashboard

### TC-DASH-001 – Verify Dashboard Loads Successfully

**Priority:** High

**Preconditions:**
- User is logged in.

**Steps:**
1. Open the Dashboard.
2. Wait for the page to finish loading.

**Expected Result:**
The Dashboard loads successfully and all available sections are displayed correctly.

**Status:** Not Executed

---

### TC-DASH-002 – Verify Activity Overview Date Filters

**Priority:** Medium

**Preconditions:**
- User is on the Dashboard.

**Steps:**
1. Locate the Activity Overview section.
2. Select the 5-day period.
3. Check the displayed data.
4. Repeat the test for 10, 14, 30, and 90 days.

**Expected Result:**
The Activity Overview updates according to the selected time period.

**Status:** Not Executed

---

### TC-DASH-003 – Verify Dashboard Refresh

**Priority:** Medium

**Preconditions:**
- User is on the Dashboard.

**Steps:**
1. Refresh the browser page.
2. Wait for the Dashboard to load.

**Expected Result:**
The Dashboard loads normally and previously available data remains consistent.

**Status:** Not Executed

---

### TC-DASH-004 – Verify Dashboard Navigation

**Priority:** Medium

**Preconditions:**
- User is logged in.

**Steps:**
1. Open the Dashboard.
2. Navigate to another section.
3. Return to the Dashboard.

**Expected Result:**
The Dashboard opens correctly and its data is displayed without unexpected changes.

**Status:** Not Executed

---

# 2. Repository / Documents

### TC-REP-001 – Upload a PDF Document

**Priority:** High

**Preconditions:**
- User has access to the Repository.

**Steps:**
1. Open the Repository.
2. Click the upload button.
3. Select a valid PDF file.
4. Confirm the upload.

**Expected Result:**
The document is uploaded successfully and the correct file name is displayed.

**Status:** Not Executed

---

### TC-REP-002 – Upload a Different Supported File

**Priority:** High

**Preconditions:**
- User is on the Repository page.

**Steps:**
1. Click Upload.
2. Select a supported document format.
3. Complete the upload.

**Expected Result:**
The selected document is uploaded successfully.

**Status:** Not Executed

---

### TC-REP-003 – Replace an Existing Document

**Priority:** High

**Preconditions:**
- A document already exists in the Repository.

**Steps:**
1. Open the existing document.
2. Select the option to replace the file.
3. Choose a different document.
4. Save the changes.

**Expected Result:**
The original document is replaced with the newly selected document, and the displayed file name is updated accordingly.

**Status:** Not Executed

---

### TC-REP-004 – Cancel Document Upload

**Priority:** Medium

**Preconditions:**
- User is on the document upload form.

**Steps:**
1. Start uploading a document.
2. Select a file.
3. Click Cancel.

**Expected Result:**
The upload is cancelled and the document is not added or changed.

**Status:** Not Executed

---

### TC-REP-005 – Delete a Document

**Priority:** High

**Preconditions:**
- A document exists in the Repository.

**Steps:**
1. Select the document.
2. Choose Delete.
3. Confirm the deletion.

**Expected Result:**
The document is removed from the active Repository and moved to the Recycle Bin.

**Status:** Not Executed

---

### TC-REP-006 – Download a Document

**Priority:** Medium

**Preconditions:**
- A document is available in the Repository.

**Steps:**
1. Select the document.
2. Click Download.

**Expected Result:**
The document downloads successfully and can be opened.

**Status:** Not Executed

---

### TC-REP-007 – Upload a Document With a Long File Name

**Priority:** Low

**Preconditions:**
- User is on the Repository page.

**Steps:**
1. Select a document with a very long file name.
2. Upload the document.

**Expected Result:**
The document is uploaded successfully and the file name is displayed without breaking the layout.

**Status:** Not Executed

---

### TC-REP-008 – Upload a Document With Special Characters

**Priority:** Medium

**Preconditions:**
- User is on the Repository page.

**Steps:**
1. Select a file containing special characters in its name.
2. Upload the file.

**Expected Result:**
The file is uploaded successfully and its name is displayed correctly.

**Status:** Not Executed

---

### TC-REP-009 – Verify File Name After Replacement

**Priority:** High

**Preconditions:**
- An existing document is available.
- A second document is available for replacement.

**Steps:**
1. Open the existing document.
2. Replace it with the second document.
3. Save the changes.
4. Check the displayed file name.

**Expected Result:**
The displayed file name matches the newly uploaded document.

**Status:** Not Executed

---

# 3. Templates

### TC-TEMP-001 – Create a New Template

**Priority:** High

**Preconditions:**
- User has permission to create templates.

**Steps:**
1. Open Templates.
2. Select New Template.
3. Enter a valid template name.
4. Upload a document if required.
5. Save the template.

**Expected Result:**
The template is created successfully and appears in the Templates list.

**Status:** Not Executed

---

### TC-TEMP-002 – Create Template With a Valid Document

**Priority:** High

**Preconditions:**
- User is on the New Template page.

**Steps:**
1. Enter a valid template name.
2. Upload a supported document.
3. Save the template.

**Expected Result:**
The template is created and the uploaded document is correctly associated with it.

**Status:** Not Executed

---

### TC-TEMP-003 – Create Template Without a Name

**Priority:** Medium

**Preconditions:**
- User is on the New Template page.

**Steps:**
1. Leave the template name empty.
2. Upload a valid document.
3. Attempt to save the template.

**Expected Result:**
If the template name is required, the system should prevent saving and display a validation message.

**Status:** Not Executed

---

### TC-TEMP-004 – Create Template With a Very Long Name

**Priority:** Medium

**Preconditions:**
- User is on the New Template page.

**Steps:**
1. Enter a very long template name.
2. Upload a valid document.
3. Save the template.

**Expected Result:**
The system should either accept the name within the supported limit or display an appropriate validation message. The interface should not break.

**Status:** Not Executed

---

### TC-TEMP-005 – Edit an Existing Template

**Priority:** High

**Preconditions:**
- An existing template is available.

**Steps:**
1. Open the template.
2. Change one of its editable fields.
3. Save the changes.
4. Reopen the template.

**Expected Result:**
The changes are saved and remain available after reopening the template.

**Status:** Not Executed

---

### TC-TEMP-006 – Delete a Template

**Priority:** High

**Preconditions:**
- An existing template is available.

**Steps:**
1. Select the template.
2. Click Delete.
3. Confirm the deletion.

**Expected Result:**
The template is removed from the active list and moved to the Recycle Bin if that functionality applies.

**Status:** Not Executed

---

### TC-TEMP-007 – Generate a Playbook From a Template

**Priority:** High

**Preconditions:**
- A valid document is available for Playbook generation.

**Steps:**
1. Open the New Template flow.
2. Upload a valid document.
3. Select the option to generate a Playbook.
4. Confirm the action.
5. Wait for the generation process to complete.

**Expected Result:**
The Playbook is generated successfully and the user receives confirmation or access to the generated file.

**Status:** Not Executed

---

### TC-TEMP-008 – Cancel Playbook Generation

**Priority:** Medium

**Preconditions:**
- A valid document is available.
- The Playbook generation confirmation is displayed.

**Steps:**
1. Start the Playbook generation flow.
2. When prompted, choose No or Cancel.

**Expected Result:**
Playbook generation is cancelled and no Playbook is created.

**Status:** Not Executed

---

# 4. Events

### TC-EVENT-001 – Create Event With Valid Information

**Priority:** High

**Preconditions:**
- User has permission to create Events.

**Steps:**
1. Open the Events section.
2. Select Create Event.
3. Enter a valid event name.
4. Complete the required fields.
5. Save the Event.

**Expected Result:**
The Event is created successfully and appears in the Events list.

**Status:** Not Executed

---

### TC-EVENT-002 – Create Event Without a Name

**Priority:** High

**Preconditions:**
- User is on the Event creation form.

**Steps:**
1. Leave the Event Name field empty.
2. Complete the other required fields.
3. Attempt to create the Event.

**Expected Result:**
The system should prevent creation if the Event Name is required and display an appropriate validation message.

**Status:** Not Executed

---

### TC-EVENT-003 – Create Event With Whitespace-Only Name

**Priority:** High

**Preconditions:**
- User is on the Event creation form.

**Steps:**
1. Enter only spaces in the Event Name field.
2. Complete the other required fields.
3. Click Create.

**Expected Result:**
The system should reject whitespace-only input and display a validation message.

**Status:** Not Executed

---

### TC-EVENT-004 – Create Event With a One-Character Name

**Priority:** Low

**Preconditions:**
- User is on the Event creation form.

**Steps:**
1. Enter a single character as the Event Name.
2. Complete the required fields.
3. Create the Event.

**Expected Result:**
The system should follow the defined minimum-length validation rules for Event names.

**Status:** Not Executed

---

### TC-EVENT-005 – Create Event With a Very Long Name

**Priority:** Medium

**Preconditions:**
- User is on the Event creation form.

**Steps:**
1. Enter a very long string in the Event Name field.
2. Complete the required fields.
3. Attempt to create the Event.

**Expected Result:**
The system should enforce the supported name length and prevent the interface from breaking.

**Status:** Not Executed

---

### TC-EVENT-006 – Edit an Existing Event

**Priority:** High

**Preconditions:**
- An existing Event is available.

**Steps:**
1. Open the Event.
2. Change an editable field.
3. Save the changes.
4. Reopen the Event.

**Expected Result:**
The updated information is saved correctly.

**Status:** Not Executed

---

### TC-EVENT-007 – Delete an Event

**Priority:** High

**Preconditions:**
- An existing Event is available.

**Steps:**
1. Select the Event.
2. Click Delete.
3. Confirm the deletion.

**Expected Result:**
The Event is deleted and handled according to the application's deletion flow.

**Status:** Not Executed

---

# 5. Workflows

### TC-WF-001 – Open Updated From Calendar

**Priority:** Medium

**Preconditions:**
- User has access to Workflows.

**Steps:**
1. Open the Workflows page.
2. Click Updated From.

**Expected Result:**
A calendar opens and allows the user to select a date.

**Status:** Not Executed

---

### TC-WF-002 – Navigate Between Calendar Months

**Priority:** Low

**Preconditions:**
- The Updated From calendar is open.

**Steps:**
1. Click the next month arrow.
2. Click the previous month arrow.
3. Repeat several times.

**Expected Result:**
The calendar moves between months correctly and displays the selected month clearly.

**Status:** Not Executed

---

### TC-WF-003 – Apply Updated From Filter

**Priority:** High

**Preconditions:**
- Workflow records are available.

**Steps:**
1. Open the Updated From filter.
2. Select a date.
3. Apply the filter.

**Expected Result:**
Only records matching the selected date criteria are displayed.

**Status:** Not Executed

---

### TC-WF-004 – Verify Workflow Status Filters

**Priority:** High

**Preconditions:**
- User is on the Workflows page.

**Steps:**
1. Select each available status/filter.
2. Observe the displayed results.

**Expected Result:**
Each filter responds to the user's selection and displays the appropriate records.

**Status:** Not Executed

---

### TC-WF-005 – Clear Workflow Filters

**Priority:** Medium

**Preconditions:**
- One or more workflow filters are applied.

**Steps:**
1. Apply a workflow filter.
2. Clear the filter.

**Expected Result:**
The filter is removed and the default set of workflow records is displayed.

**Status:** Not Executed

---

# 6. AI Assistant

### TC-AI-001 – Send a Basic Message

**Priority:** High

**Preconditions:**
- User has access to the AI Assistant.

**Steps:**
1. Open the AI Assistant.
2. Enter a simple message.
3. Send the message.

**Expected Result:**
The message is displayed and the AI Assistant returns a response.

**Status:** Not Executed

---

### TC-AI-002 – Send an Empty Message

**Priority:** Medium

**Preconditions:**
- AI Assistant is open.

**Steps:**
1. Leave the message field empty.
2. Attempt to send the message.

**Expected Result:**
The system should prevent an empty message from being submitted.

**Status:** Not Executed

---

### TC-AI-003 – Start a New Conversation

**Priority:** High

**Preconditions:**
- An existing conversation contains messages.

**Steps:**
1. Open the AI Assistant.
2. Send a message.
3. Start a new conversation.

**Expected Result:**
A new conversation is opened without incorrectly carrying over messages from the previous conversation.

**Status:** Not Executed

---

### TC-AI-004 – Refresh AI Assistant

**Priority:** Medium

**Preconditions:**
- The AI Assistant contains an active conversation.

**Steps:**
1. Send a message.
2. Refresh the browser.
3. Wait for the page to load.

**Expected Result:**
The application should behave according to its intended conversation persistence rules.

**Status:** Not Executed

---

### TC-AI-005 – Navigate Away From AI Assistant

**Priority:** Medium

**Preconditions:**
- The AI Assistant contains an active conversation.

**Steps:**
1. Send a message.
2. Navigate to another section.
3. Return to the AI Assistant.

**Expected Result:**
Conversation history should behave according to the application's intended persistence rules.

**Status:** Not Executed

---

### TC-AI-006 – Send a Long Message

**Priority:** Medium

**Preconditions:**
- AI Assistant is open.

**Steps:**
1. Enter a long text message.
2. Send the message.

**Expected Result:**
The message is submitted successfully or the user receives a clear validation message if a length limit is exceeded.

**Status:** Not Executed

---

# 7. Search

### TC-SEARCH-001 – Search for an Existing Document

**Priority:** High

**Preconditions:**
- At least one searchable document exists.

**Steps:**
1. Open Search.
2. Enter part of the document name.
3. Submit the search.

**Expected Result:**
Relevant results are displayed.

**Status:** Not Executed

---

### TC-SEARCH-002 – Search With No Matching Results

**Priority:** Medium

**Preconditions:**
- User is on the Search page.

**Steps:**
1. Enter a value that does not exist.
2. Run the search.

**Expected Result:**
The system displays an appropriate no-results state.

**Status:** Not Executed

---

### TC-SEARCH-003 – Clear Search

**Priority:** Medium

**Preconditions:**
- A search has been performed.

**Steps:**
1. Enter a search term.
2. Run the search.
3. Click the Clear button/icon.

**Expected Result:**
The search term is removed and the search state is reset.

**Status:** Not Executed

---

### TC-SEARCH-004 – Search Using Documents and Global Modes

**Priority:** High

**Preconditions:**
- Search functionality is available.

**Steps:**
1. Search for a known value using Documents.
2. Repeat the search using Global.

**Expected Result:**
Each search mode returns results according to its intended scope.

**Status:** Not Executed

---

### TC-SEARCH-005 – Search With Special Characters

**Priority:** Low

**Preconditions:**
- Search field is available.

**Steps:**
1. Enter special characters into the search field.
2. Run the search.

**Expected Result:**
The application handles the input safely and provides an appropriate result or no-results state without breaking the page.

**Status:** Not Executed

---

# 8. Recycle Bin

### TC-REC-001 – Verify Deleted Item Appears in Recycle Bin

**Priority:** High

**Preconditions:**
- An item can be deleted.

**Steps:**
1. Delete an item.
2. Open the Recycle Bin.

**Expected Result:**
The deleted item appears in the Recycle Bin.

**Status:** Not Executed

---

### TC-REC-002 – Restore an Item

**Priority:** High

**Preconditions:**
- A deleted item exists in the Recycle Bin.

**Steps:**
1. Open the Recycle Bin.
2. Select the deleted item.
3. Choose Restore.

**Expected Result:**
The item is restored and becomes available in its original location.

**Status:** Not Executed

---

### TC-REC-003 – Permanently Delete an Item

**Priority:** High

**Preconditions:**
- A deleted item exists in the Recycle Bin.

**Steps:**
1. Open the Recycle Bin.
2. Select the item.
3. Choose Permanent Delete.
4. Confirm the action.

**Expected Result:**
The item is permanently removed and is no longer available for restoration.

**Status:** Not Executed

---

# 9. General Validation

### TC-VAL-001 – Verify Required Fields

**Priority:** High

**Steps:**
1. Open forms containing required fields.
2. Leave required fields empty.
3. Attempt to save.

**Expected Result:**
The system prevents submission and clearly identifies the required fields.

**Status:** Not Executed

---

### TC-VAL-002 – Verify Whitespace-Only Input

**Priority:** Medium

**Steps:**
1. Enter only spaces into text fields.
2. Attempt to save the form.

**Expected Result:**
Whitespace-only input should be rejected where meaningful text is required.

**Status:** Not Executed

---

### TC-VAL-003 – Verify Long Text Input

**Priority:** Medium

**Steps:**
1. Enter a very long value into a text field.
2. Attempt to save.

**Expected Result:**
The application should enforce any defined character limit and maintain a stable layout.

**Status:** Not Executed

---

### TC-VAL-004 – Verify Special Characters

**Priority:** Low

**Steps:**
1. Enter special characters into supported text fields.
2. Save the information.

**Expected Result:**
The application handles the input correctly without unexpected errors or UI issues.

**Status:** Not Executed
Not Executed
