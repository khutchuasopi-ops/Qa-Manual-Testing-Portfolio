# BUG-001 – Old File Name Remains After Replacing a Document

## Area

Repository

## Severity

Medium

## Priority

Medium

## Preconditions

- User is logged in.
- User has access to the Repository.
- A document has already been uploaded.

## Steps to Reproduce

1. Open the Repository.
2. Upload a PDF document.
3. Open the uploaded document.
4. Select the option to replace the file.
5. Select a different PDF document from the computer.
6. Save the changes.
7. Check the file name displayed in the Repository.

## Expected Result

The newly uploaded document should replace the previous document, and the new file name should be displayed correctly.

## Actual Result

The new document is uploaded successfully, but the file name displayed in the interface remains the name of the previously uploaded document.

## Impact

The displayed file name does not match the newly uploaded document. This may confuse users and make it difficult to identify the current file.

## Status

Open
