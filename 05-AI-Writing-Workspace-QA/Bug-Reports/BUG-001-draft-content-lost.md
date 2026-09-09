# BUG-001 — Draft Content Is Lost After Refresh

## Title
Text entered in the Draft Editor is lost after page refresh

## Preconditions
- User is logged in.
- A project/manuscript with an available Draft exists.
- The Draft Editor is accessible.

## Steps to Reproduce
1. Open a project/manuscript.
2. Navigate to the Draft section.
3. Wait until the Draft Editor is available.
4. Click inside the actual Draft Editor.
5. Enter text, for example:
   `Once upon a time there was a small village.`
6. Confirm that the text is visible in the Draft Editor.
7. Refresh the page.
8. Check the Draft content again.

## Expected Result
Text entered in the Draft Editor should be saved and remain available after refreshing the page.

## Actual Result
The text entered in the Draft Editor disappears after refreshing the page.

## Priority
High

## Severity
Critical

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Draft Editor

## Evidence
Screen recording showing:
1. Text being entered into the Draft Editor.
2. The text being visible before refresh.
3. The text disappearing after refresh.

## Status
Open
