# BUG-006 — Poster Save Is Delayed or Unresponsive

## Title
Save Poster action is delayed and does not update the poster immediately

## Preconditions
- User is logged in.
- A project/manuscript exists.
- The user has access to Poster editing.
- A new poster image has been selected.

## Steps to Reproduce
1. Open a project/manuscript.
2. Navigate to Poster editing.
3. Select or upload a new poster image.
4. Click `Save Poster`.
5. Observe the poster immediately after clicking the button.
6. Wait for some time and observe the poster again.

## Expected Result
The selected poster image should be saved immediately after clicking `Save Poster`.

The updated poster should be displayed without a significant delay.

## Actual Result
The `Save Poster` action appears unresponsive after clicking.

The selected image is not applied immediately.

After some time, the poster is eventually updated.

## Priority
Medium

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Poster

## Evidence
Screen recording showing the selected image, the Save Poster action, delayed update, and final poster state.

## Status
Open
