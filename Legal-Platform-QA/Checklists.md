# QA Checklists — Legal Platform

## 1. Document Upload Checklist

* [ ] Upload a valid PDF file
* [ ] Upload a valid DOCX file
* [ ] Try an unsupported file format
* [ ] Try uploading an empty file
* [ ] Try uploading a large file
* [ ] Try a file with a long file name
* [ ] Try special characters in the file name
* [ ] Try uploading a duplicate file
* [ ] Replace an existing file
* [ ] Delete an uploaded file
* [ ] Download an uploaded file
* [ ] Verify the correct file name after upload
* [ ] Verify the file can be opened after upload

---

## 2. File Replacement Checklist

* [ ] Select an existing file
* [ ] Replace the file with a valid file
* [ ] Verify the new file is displayed
* [ ] Verify the new file name is displayed correctly
* [ ] Verify the previous file is no longer shown as the current file
* [ ] Refresh the page after replacement
* [ ] Verify the replaced file remains available
* [ ] Try replacing the file with an unsupported format
* [ ] Check whether an appropriate validation message is displayed

---

## 3. Template Checklist

* [ ] Create a new template
* [ ] Edit an existing template
* [ ] Delete a template
* [ ] Restore a deleted template
* [ ] Try an empty template name
* [ ] Try a whitespace-only template name
* [ ] Try a one-character template name
* [ ] Try a long template name
* [ ] Try special characters in the template name
* [ ] Upload a document to a template
* [ ] Generate a Playbook from a template
* [ ] Verify the created template appears correctly
* [ ] Verify template changes are saved

---

## 4. Event Checklist

* [ ] Create a new event
* [ ] Edit an existing event
* [ ] Delete an event
* [ ] Try an empty event name
* [ ] Try a whitespace-only event name
* [ ] Try a one-character event name
* [ ] Try a long event name
* [ ] Try special characters in the event name
* [ ] Enter valid event dates
* [ ] Try invalid date values
* [ ] Try past dates where not allowed
* [ ] Verify the event is displayed after creation
* [ ] Verify edited event information is saved

---

## 5. Search Checklist

* [ ] Search using a valid keyword
* [ ] Search using a partial keyword
* [ ] Search for an existing item
* [ ] Search for an item that does not exist
* [ ] Check the no-results message
* [ ] Search with an empty field
* [ ] Search using special characters
* [ ] Clear the search field
* [ ] Verify search results after clearing the field
* [ ] Test search in Documents mode
* [ ] Test search in Global mode
* [ ] Verify that results match the entered search term

---

## 6. Repository Checklist

* [ ] Open the Repository
* [ ] View available files and folders
* [ ] Open an existing document
* [ ] Search for a repository item
* [ ] Check available file actions
* [ ] Upload a document
* [ ] Replace a document
* [ ] Delete a document
* [ ] Verify the correct file information is displayed
* [ ] Refresh the page and verify the data remains correct

---

## 7. Documents Checklist

* [ ] Open the Documents section
* [ ] Open an existing document
* [ ] Upload a document
* [ ] Download a document
* [ ] Delete a document
* [ ] Search for a document
* [ ] Verify the document name
* [ ] Verify the document type
* [ ] Verify document actions
* [ ] Refresh the page and verify the document is still available

---

## 8. Recycle Bin Checklist

* [ ] Open the Recycle Bin
* [ ] Verify deleted items are displayed
* [ ] Restore a deleted item
* [ ] Verify the restored item appears in its original location
* [ ] Delete an item from the Recycle Bin
* [ ] Verify the item is no longer available
* [ ] Refresh the page and verify the result

---

## 9. AI Assistant Checklist

* [ ] Open the AI Assistant
* [ ] Send a valid question
* [ ] Verify a response is returned
* [ ] Ask a follow-up question
* [ ] Check whether the conversation context is maintained
* [ ] Try an unclear question
* [ ] Try an invalid or unsupported request
* [ ] Verify the response is displayed correctly
* [ ] Check the loading state
* [ ] Check error handling if the request cannot be completed

---

## 10. Playbook Generation Checklist

* [ ] Open a template
* [ ] Upload the required document
* [ ] Start Playbook generation
* [ ] Verify the generation process starts
* [ ] Check the loading state
* [ ] Verify the generated Playbook is displayed
* [ ] Check the generated content
* [ ] Verify the correct template/document was used
* [ ] Check error handling if generation cannot be completed

---

## 11. UI and Usability Checklist

* [ ] Check button text visibility
* [ ] Check button hover states
* [ ] Check cursor states
* [ ] Check text overflow
* [ ] Check long text inside fields
* [ ] Check modal layout
* [ ] Check form alignment
* [ ] Check loading indicators
* [ ] Check validation messages
* [ ] Check error messages
* [ ] Check that important actions are clearly visible
* [ ] Check basic responsive behavior

---

## 12. Data Consistency Checklist

* [ ] Verify data after creating an item
* [ ] Verify data after editing an item
* [ ] Verify data after deleting an item
* [ ] Verify data after restoring an item
* [ ] Verify file information after replacement
* [ ] Refresh the page and verify saved data
* [ ] Verify that related sections show consistent information
* [ ] Check that old information is not displayed after an update

---

## 13. Regression Checklist

After a defect is fixed:

* [ ] Reproduce the original issue
* [ ] Confirm the issue is fixed
* [ ] Verify the expected result
* [ ] Repeat the original test steps
* [ ] Test the main related functionality
* [ ] Check for side effects
* [ ] Refresh the page and verify the result
* [ ] Record the retest result
* [ ] Perform regression testing around the affected area

---

## 14. General QA Checklist

* [ ] Main user flow works as expected
* [ ] Valid input is accepted
* [ ] Invalid input is handled correctly
* [ ] Empty input is validated
* [ ] Boundary values are checked
* [ ] Error messages are clear
* [ ] Data is saved correctly
* [ ] Data remains correct after refresh
* [ ] UI elements are usable
* [ ] Reported defects have clear reproduction steps
* [ ] Retesting is performed after fixes
* [ ] Related functionality is checked during regression

---

## Checklist Purpose

These checklists are used as a practical support during manual testing.

They help verify the main functionality, common negative cases, boundary values, data consistency, and basic UI behavior without replacing detailed test cases.

The checklists are intentionally kept simple so they can be reused during smoke, regression, exploratory, and general manual testing.

