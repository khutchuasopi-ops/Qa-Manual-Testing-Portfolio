# BUG-001 — Event Cannot Be Added to Director Availability

**Area:** Director Availability
**Type:** Functional
**Severity:** High
**Environment:** Test Environment

## Preconditions

A Director is available in the application and the Director Availability section is accessible.

## Steps to Reproduce

1. Open the **Director** section.
2. Select a Director.
3. Open the **Availability** section.
4. Click **+ EVENT**.
5. Enter the required Event information.
6. Select valid start and end dates.
7. Submit the Event.

## Actual Result

The Event cannot be added successfully to the Director's Availability.

## Expected Result

The Event should be created successfully and displayed in the Director's Availability.

## Impact

Users cannot add availability events for a Director, which prevents accurate management of the Director's availability schedule.

## Retest

The issue was later fixed and successfully retested in the test environment.
