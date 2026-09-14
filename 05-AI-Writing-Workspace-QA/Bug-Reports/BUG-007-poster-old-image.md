# BUG-007 — Upload Dialog Shows Previous Image

## Summary

The image upload dialog displays the previously selected image when the user starts a new image upload operation.

## Preconditions

* User has access to a Project / Manuscript.
* A Poster / Cover can be edited.
* An image has previously been selected or uploaded.

## Steps to Reproduce

1. Open a Project / Manuscript.
2. Open the **Poster / Cover** section.
3. Select **Edit**.
4. Open the image **Upload** option.
5. Select an image and complete or cancel the upload flow.
6. Open the **Upload** option again.
7. Observe the image displayed in the upload dialog.

## Actual Result

The upload dialog displays the image from the previous upload operation.

The previous image remains visible when starting a new upload operation, instead of showing a clean upload state.

## Expected Result

When the user opens the upload dialog for a new upload operation, it should display the current upload state only.

A previously selected image should not remain visible unless it is intentionally associated with the current Poster / Cover.

## Severity

**Medium**

## Environment

**Staging / Preview**

## Related Test Case

**TC-021 — Poster: Upload Image**

## Status

**Open**

## Reproduction

**Reproduced during manual testing.**

## Notes

The issue can cause confusion because the user may believe that the previously displayed image is still selected for the current upload operation.

The upload dialog should reset its temporary state when a new upload operation is started.

