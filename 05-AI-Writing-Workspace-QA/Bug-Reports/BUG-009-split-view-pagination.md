# BUG-009 — Split View Duplicates or Resets Pagination

## Title
Split View duplicates or resets pagination/page breaks in the second pane

## Preconditions
- User is logged in.
- A project/manuscript contains a Draft with enough content to span multiple pages.
- Pagination or page breaks are visible in the Draft.

## Steps to Reproduce
1. Open a project/manuscript.
2. Open the Draft.
3. Add or use enough content to create multiple pages.
4. Open the same Draft in Split View.
5. Compare the pagination/page breaks between the two panes.
6. Observe the pagination behavior in the second pane.

## Expected Result
Both Split View panes should display consistent pagination and page-break positions for the same Draft content.

Pagination should not be duplicated, reset, or repositioned unexpectedly.

## Actual Result
Pagination/page breaks in the second Split View pane are duplicated or appear to restart from the beginning instead of remaining consistent with the original Draft view.

The issue was reproduced during testing.

## Priority
High

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Split View / Draft

## Evidence
Screen recording showing the same Draft opened in Split View and the inconsistent pagination/page-break behavior between the two panes.

## Status
Reproduced
