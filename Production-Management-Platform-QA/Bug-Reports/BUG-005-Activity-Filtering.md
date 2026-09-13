# BUG-005 — Meeting Activity View Displays Call Activities

**Area:** Sales / Activity Management
**Type:** Functional / Data Filtering
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

* Sales Activity contains both **Call** and **Meeting** activities.

## Steps

1. Open **Sales Activity**.
2. Open a **Call** activity.
3. Review the displayed activities.
4. Return to the activity list.
5. Open a **Meeting** activity.
6. Review the displayed activities.

## Actual Result

The Call view displays only Call activities, but the Meeting view displays both Meeting and Call activities.

## Expected Result

The Meeting view should display only Meeting activities, consistent with the filtering behavior of the Call view.

## Impact

Displaying unrelated activities can cause confusion and make activity tracking inaccurate.
