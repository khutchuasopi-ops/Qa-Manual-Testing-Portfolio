# BUG-005 — Meeting Activity View Displays Call Activities

**Area:** Sales / Activity Management
**Type:** Functional / Data Filtering
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

The Sales Activity area contains both Call and Meeting activities.

## Steps to Reproduce

1. Open the **Sales Activity** area.
2. Open a **Call** activity.
3. Review the displayed activities.
4. Return to the activity list.
5. Open a **Meeting** activity.
6. Review the displayed activities.

## Actual Result

The Call view displays only Call activities.

However, the Meeting view displays both Meeting and Call activities.

## Expected Result

The Meeting view should display only Meeting activities, in the same way that the Call view displays only Call activities.

## Impact

Users may see unrelated activities when reviewing a specific activity type, which can cause confusion and inaccurate activity tracking.
