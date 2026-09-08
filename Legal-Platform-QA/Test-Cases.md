# Test Cases — Legal Platform QA

## Documents

### TC-001 — Create a Document

**Precondition:** User is logged in and Documents section is available.

**Steps:**

1. Open Documents.
2. Click **Create**.
3. Enter valid document information.
4. Save the document.

**Expected Result:**
The document is created and displayed in the Documents section.

---

### TC-002 — Required Document Fields

**Steps:**

1. Open the document creation form.
2. Leave a required field empty.
3. Click **Save**.

**Expected Result:**
The document is not created and a validation message is displayed.

---

### TC-003 — Edit a Document

**Steps:**

1. Open an existing document.
2. Change one of its values.
3. Save the changes.

**Expected Result:**
The updated information is displayed correctly.

---

### TC-004 — Delete a Document

**Steps:**

1. Open an existing document.
2. Click **Delete**.
3. Confirm the action.

**Expected Result:**
The document is removed from the active document list.

---

### TC-005 — Document Data After Refresh

**Steps:**

1. Open an existing document.
2. Make a change.
3. Save the change.
4. Refresh the page.

**Expected Result:**
The saved information is still displayed correctly after refresh.

---

## File Upload

### TC-006 — Upload a Valid File

**Steps:**

1. Open the file upload section.
2. Select a supported file.
3. Upload the file.

**Expected Result:**
The file is uploaded successfully and appears in the expected location.

---

### TC-007 — Upload an Unsupported File

**Steps:**

1. Open the file upload section.
2. Select an unsupported file type.
3. Try to upload the file.

**Expected Result:**
The application prevents the upload and displays an appropriate validation message.

---

### TC-008 — Upload File With Invalid Name

**Steps:**

1. Open the file upload section.
2. Select a file with an invalid or unsupported name.
3. Upload the file.

**Expected Result:**
The application handles the invalid filename correctly and displays a validation message if required.

---

### TC-009 — Verify Uploaded File Information

**Steps:**

1. Upload a valid file.
2. Open the uploaded file information.

**Expected Result:**
The displayed file information is correct.

---

## File Replacement

### TC-010 — Replace an Existing File

**Steps:**

1. Open an existing file.
2. Select the replace option.
3. Upload another valid file.
4. Save the change.

**Expected Result:**
The original file is replaced with the new file.

---

### TC-011 — Verify New File After Replacement

**Steps:**

1. Replace an existing file.
2. Open the file again.

**Expected Result:**
The new file is displayed.

---

### TC-012 — Verify File Data After Replacement

**Steps:**

1. Replace an existing file.
2. Check the file information.
3. Refresh the page.

**Expected Result:**
The correct new file and related information remain displayed after refresh.

---

## Repository

### TC-013 — Open Repository

**Steps:**

1. Open the Repository section.

**Expected Result:**
The Repository opens and available items are displayed.

---

### TC-014 — Open Repository Item

**Steps:**

1. Open the Repository.
2. Select an existing item.

**Expected Result:**
The selected item opens correctly.

---

### TC-015 — Delete Repository Item

**Steps:**

1. Open the Repository.
2. Select an item.
3. Delete the item.
4. Confirm the action.

**Expected Result:**
The item is removed from the active Repository list.

---

### TC-016 — Restore Repository Item

**Steps:**

1. Delete an existing Repository item.
2. Open the Recycle Bin.
3. Select the deleted item.
4. Restore it.

**Expected Result:**
The item is restored and becomes available again.

---

## Templates

### TC-017 — Create a Template

**Steps:**

1. Open Templates.
2. Click **Create**.
3. Enter valid information.
4. Save the template.

**Expected Result:**
The template is created successfully.

---

### TC-018 — Required Template Fields

**Steps:**

1. Open the template creation form.
2. Leave a required field empty.
3. Click **Save**.

**Expected Result:**
The template is not created and a validation message is displayed.

---

### TC-019 — Template Name Validation

**Steps:**

1. Open the template creation form.
2. Enter an invalid template name.
3. Try to save the template.

**Expected Result:**
The application rejects the invalid name and displays a validation message.

---

### TC-020 — Empty Template Name

**Steps:**

1. Open the template creation form.
2. Leave the template name empty.
3. Click **Save**.

**Expected Result:**
The template is not created.

---

### TC-021 — Edit a Template

**Steps:**

1. Open an existing template.
2. Change the template information.
3. Save the changes.

**Expected Result:**
The updated template information is displayed correctly.

---

## Events

### TC-022 — Create an Event

**Steps:**

1. Open Events.
2. Click **Create**.
3. Enter valid event information.
4. Save the event.

**Expected Result:**
The event is created successfully.

---

### TC-023 — Required Event Fields

**Steps:**

1. Open the event creation form.
2. Leave a required field empty.
3. Click **Save**.

**Expected Result:**
The event is not created and a validation message is displayed.

---

### TC-024 — Event Name Validation

**Steps:**

1. Open the event creation form.
2. Enter an invalid event name.
3. Save the event.

**Expected Result:**
The application rejects the invalid name.

---

### TC-025 — Event Name Boundary Value

**Steps:**

1. Open the event creation form.
2. Enter a name at the allowed character limit.
3. Save the event.
4. Repeat using a value above the allowed limit.

**Expected Result:**
The value within the allowed limit is accepted.
The value above the limit is rejected or handled according to the requirements.

---

### TC-026 — Verify Event After Saving

**Steps:**

1. Create an event with valid information.
2. Open the created event.

**Expected Result:**
The saved event information is displayed correctly.

---

## Workflows

### TC-027 — Start a Workflow

**Steps:**

1. Open Workflows.
2. Select an available workflow.
3. Start the workflow.

**Expected Result:**
The selected workflow starts successfully.

---

### TC-028 — Workflow Required Information

**Steps:**

1. Start a workflow.
2. Leave a required field empty.
3. Continue.

**Expected Result:**
The application prevents the user from continuing and displays a validation message.

---

### TC-029 — Workflow Invalid Input

**Steps:**

1. Start a workflow.
2. Enter invalid information.
3. Continue.

**Expected Result:**
The invalid input is rejected and an appropriate message is displayed.

---

### TC-030 — Workflow Result

**Steps:**

1. Start a workflow.
2. Enter valid information.
3. Complete the workflow.

**Expected Result:**
The workflow completes and the expected result is displayed.

---

## AI Assistant

### TC-031 — Open AI Assistant

**Steps:**

1. Open the AI Assistant section.

**Expected Result:**
The AI Assistant opens correctly.

---

### TC-032 — Send a Valid Request

**Steps:**

1. Open the AI Assistant.
2. Enter a valid request.
3. Send the request.

**Expected Result:**
The request is submitted and a response is displayed.

---

### TC-033 — Empty AI Request

**Steps:**

1. Open the AI Assistant.
2. Leave the input empty.
3. Try to send the request.

**Expected Result:**
The application prevents an empty request or handles it with an appropriate message.

---

### TC-034 — Invalid AI Input

**Steps:**

1. Open the AI Assistant.
2. Enter invalid or unexpected input.
3. Send the request.

**Expected Result:**
The application handles the input without breaking the page or conversation.

---

### TC-035 — Multiple AI Requests

**Steps:**

1. Open the AI Assistant.
2. Send one valid request.
3. Send another request.

**Expected Result:**
Both requests are handled correctly and the conversation remains usable.

---

## Search

### TC-036 — Search Existing Value

**Steps:**

1. Open Search.
2. Enter a value that exists.
3. Run the search.

**Expected Result:**
Matching results are displayed.

---

### TC-037 — Search Partial Value

**Steps:**

1. Open Search.
2. Enter part of an existing value.
3. Run the search.

**Expected Result:**
Relevant matching results are displayed.

---

### TC-038 — Search With No Results

**Steps:**

1. Open Search.
2. Enter a value that does not exist.
3. Run the search.

**Expected Result:**
No matching results are displayed and the application provides an appropriate empty-state message.

---

### TC-039 — Empty Search

**Steps:**

1. Open Search.
2. Leave the search field empty.
3. Run the search.

**Expected Result:**
The application handles the empty search correctly.

---

### TC-040 — Search Results

**Steps:**

1. Search for an existing value.
2. Review the returned results.

**Expected Result:**
The results match the search criteria.

---

### TC-041 — Filter Search Results

**Steps:**

1. Perform a search.
2. Apply an available filter.
3. Review the results.

**Expected Result:**
The results are filtered according to the selected filter.

---

## Recycle Bin

### TC-042 — Deleted Item Appears in Recycle Bin

**Steps:**

1. Delete an item.
2. Open the Recycle Bin.

**Expected Result:**
The deleted item appears in the Recycle Bin.

---

### TC-043 — Restore an Item

**Steps:**

1. Open the Recycle Bin.
2. Select a deleted item.
3. Click **Restore**.

**Expected Result:**
The item is restored successfully.

---

### TC-044 — Verify Item After Restore

**Steps:**

1. Restore a deleted item.
2. Return to its original section.

**Expected Result:**
The restored item is available in its original location.

---

### TC-045 — Verify Data After Restore

**Steps:**

1. Delete an item.
2. Restore the item.
3. Open the restored item.

**Expected Result:**
The item and its information are displayed correctly after restoration.

---

## Playbook Generation

### TC-046 — Start Playbook Generation

**Steps:**

1. Open Playbook Generation.
2. Start the process.

**Expected Result:**
The Playbook Generation process starts successfully.

---

### TC-047 — Required Playbook Input

**Steps:**

1. Open Playbook Generation.
2. Leave a required field empty.
3. Try to continue.

**Expected Result:**
The application prevents the user from continuing and displays a validation message.

---

### TC-048 — Invalid Playbook Input

**Steps:**

1. Open Playbook Generation.
2. Enter invalid input.
3. Try to continue.

**Expected Result:**
The invalid input is rejected or handled correctly.

---

### TC-049 — Generated Playbook

**Steps:**

1. Enter valid information.
2. Complete the Playbook Generation process.
3. Review the result.

**Expected Result:**
A Playbook is generated and the content is displayed correctly.

---

## UI and Usability

### TC-050 — Button Display

**Steps:**

1. Open the main sections of the application.
2. Review the available buttons and controls.

**Expected Result:**
Buttons and controls are visible and readable.

---

### TC-051 — Text Readability

**Steps:**

1. Open different sections.
2. Review labels, buttons, and messages.

**Expected Result:**
Text is readable and does not overlap or become hidden.

---

### TC-052 — Validation Messages

**Steps:**

1. Trigger a validation error.
2. Review the displayed message.

**Expected Result:**
The message clearly explains the problem.

---

### TC-053 — Navigation

**Steps:**

1. Navigate between the main application sections.
2. Use the available navigation controls.

**Expected Result:**
Navigation works correctly and the selected section opens.

---

### TC-054 — UI After Saving

**Steps:**

1. Create or update an item.
2. Save the changes.
3. Review the page.

**Expected Result:**
The updated information is displayed correctly and the UI remains usable.

---

### TC-055 — UI After Error

**Steps:**

1. Perform an action that causes a validation or application error.
2. Review the page.

**Expected Result:**
The error is handled without breaking the page or preventing normal navigation.

---

## Regression

### TC-056 — Document Regression

**Steps:**

1. Open Documents after an application change.
2. Create or edit a document.
3. Save the changes.

**Expected Result:**
Document functionality continues to work correctly.

---

### TC-057 — File Regression

**Steps:**

1. Upload a valid file.
2. Replace the file.
3. Refresh the page.

**Expected Result:**
File upload and replacement continue to work correctly and the correct file is displayed.

---

### TC-058 — Search Regression

**Steps:**

1. Open Search after an application change.
2. Search for an existing value.
3. Apply a filter.

**Expected Result:**
Search and filtering continue to work correctly.

---

### TC-059 — Template and Event Regression

**Steps:**

1. Open Templates and Events.
2. Create or update an item.
3. Save the changes.

**Expected Result:**
Template and Event functionality continues to work correctly.

---

### TC-060 — Recycle Bin Regression

**Steps:**

1. Delete an item.
2. Open the Recycle Bin.
3. Restore the item.

**Expected Result:**
The item is restored correctly and appears in its original location.

---

## Test Case Summary

**Total Test Cases: 60**

The test cases cover:

* Documents
* Repository
* File Upload
* File Replacement
* Templates
* Events
* Workflows
* AI Assistant
* Search
* Recycle Bin
* Playbook Generation
* UI and Usability
* Regression Testing

Test execution results are documented separately in `Test-Execution.md`.
