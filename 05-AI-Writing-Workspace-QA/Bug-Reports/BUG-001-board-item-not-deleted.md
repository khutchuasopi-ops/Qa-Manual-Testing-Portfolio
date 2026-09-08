# BUG-001 — Deleted Board Item Remains Visible After Refresh

## Title
Deleted Board item remains visible after refresh

## Preconditions
- User is logged in.
- A project/manuscript contains an item on the Board.
- The item is visible on the Board before deletion.

## Steps to Reproduce
1. Open the project/manuscript.
2. Navigate to the Board.
3. Select an existing Board item.
4. Delete the item.
5. Observe the Board after deletion.
6. Refresh the page.
7. Check whether the deleted item is still visible.

## Expected Result
The deleted Board item should be removed from the Board immediately and should remain removed after refreshing the page.

## Actual Result
The deleted Board item remains visible on the Board after deletion and is still displayed after refreshing the page.

## Priority
High

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Board

## Evidence
Screen recording or screenshot showing the deletion action and the item remaining visible after refresh.

## Status
Open
