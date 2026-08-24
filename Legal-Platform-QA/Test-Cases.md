# Test Cases

## TC-001 – Upload PDF Document

**Priority:** High

### Preconditions

User is authenticated and has access to the Repository.

### Steps

1. Open Repository.
2. Click Upload.
3. Select a valid PDF file.
4. Complete the upload.

### Expected Result

The PDF should be uploaded successfully and displayed with the correct file name.

### Status

Not Executed

## TC-002 – Replace Uploaded Document

**Priority:** High

### Preconditions

A document has already been uploaded to the Repository.

### Steps

1. Open the uploaded document.
2. Select the option to replace the file.
3. Choose a different PDF file.
4. Save the changes.

### Expected Result

The new file should replace the previous file and the displayed file name should be updated accordingly.

### Status

Not Executed

## TC-003 – Create Event With Whitespace-Only Name

**Priority:** Medium

### Preconditions

User has permission to create an Event.

### Steps

1. Open the Event creation form.
2. Enter only whitespace characters in the Event Name field.
3. Complete other required fields.
4. Click Create.

### Expected Result

The system should reject whitespace-only input and display an appropriate validation message.

### Status

Not Executed
