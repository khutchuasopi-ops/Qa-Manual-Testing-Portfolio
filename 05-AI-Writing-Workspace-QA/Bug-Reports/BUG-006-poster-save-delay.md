# BUG-006 — Save Poster Action Delayed / Unresponsive

## Summary

The **Save Poster** action does not respond immediately after a new poster image is selected. The user can click the button multiple times without receiving a visible response, while the poster is updated only after a noticeable delay.

## Preconditions

* User has access to an existing Project / Manuscript.
* The Project has an existing Poster / Cover.
* User is able to edit the Poster.

## Steps

1. Open a Project / Manuscript.
2. Select **Edit**.
3. Open the **Upload** option.
4. Select a new poster image.
5. Click **Save Poster**.
6. Observe the result immediately after clicking.
7. Wait and observe the Poster again.

## Actual Result

After clicking **Save Poster**, the action does not respond immediately.

The Poster does not update immediately, and clicking the **Save Poster** button multiple times does not provide clear feedback that the save operation is being processed.

After some time, the Poster is eventually updated with the new image.

## Expected Result

After clicking **Save Poster**:

* The save operation should start immediately.
* The user should receive clear feedback that the save is in progress or has completed.
* The new Poster should be displayed after the save is completed.
* The user should not need to click the **Save Poster** button multiple times to trigger the operation.

## Severity

**Medium**

## Environment

**Staging / Preview**

## Related Test Case

**TC-020 — Verify Save Poster Action**

## Status

**Open**

## Reproduction

**Reproduced during manual testing.**

## Notes

The issue is related to delayed save behavior rather than a complete failure of the Save Poster functionality.

The new Poster was eventually updated, but the lack of immediate response or clear save feedback can make the user believe that the action was not registered and may lead to repeated clicks.

