# BUG-009 — Split View Pagination / Page State Breaks

## Summary

Pagination in **Split View** becomes inconsistent when navigating between pages. Pages can be duplicated or the displayed page state can reset unexpectedly.

## Preconditions

* User has access to a document or manuscript with multiple pages.
* Split View is available for the document.

## Steps to Reproduce

1. Open a document or manuscript.
2. Open **Split View**.
3. Navigate between the available pages using the pagination controls.
4. Continue moving between different pages.
5. Observe the displayed page content and page number.

## Actual Result

During navigation, Split View pagination becomes inconsistent.

Pages may be duplicated, and the displayed page state can reset unexpectedly instead of remaining on the selected page.

## Expected Result

When navigating between pages in Split View:

* The selected page should be displayed correctly.
* The page number should correspond to the displayed content.
* Pages should not be duplicated.
* The current page should not unexpectedly reset.
* Pagination should remain consistent during repeated navigation.

## Severity

**Medium**

## Environment

**Staging / Preview**

## Related Test Case

**TC-026 — Split View: Pagination**

## Status

**Open**

## Reproduction

**Reproduced during manual testing.**

## Notes

The issue affects navigation within Split View and can make it difficult for the user to determine which page is currently being viewed.

The pagination state should remain synchronized with the displayed document content during navigation.
