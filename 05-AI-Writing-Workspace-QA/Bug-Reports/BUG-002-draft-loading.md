# BUG-002 — Draft Initially Fails to Load on First Open

## Title
Draft does not load correctly when opened for the first time

## Preconditions
- User is logged in.
- A project/manuscript with an existing Draft is available.

## Steps to Reproduce
1. Open the project/manuscript from the Home or Library page.
2. Navigate directly to the Draft section.
3. Observe the Draft loading state.
4. Wait for the Draft to finish loading.
5. Navigate to the Plan section.
6. Navigate back to the Draft section.
7. Observe the Draft again.

## Expected Result
The Draft should load correctly when opened for the first time without requiring navigation to another section and back.

## Actual Result
The Draft remains in a loading state when opened initially and does not load correctly.

After navigating to Plan and then returning to Draft, the Draft loads correctly.

## Workaround
Navigate from Draft to Plan and then back to Draft.

## Priority
Medium

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Draft

## Evidence
Screen recording showing the initial Draft loading state and the successful load after navigating to Plan and back to Draft.

## Status
Open
