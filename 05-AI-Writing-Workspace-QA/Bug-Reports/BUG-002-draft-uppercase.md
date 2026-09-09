# BUG-002 — Draft Editor Automatically Enters Text in Uppercase

## Title
Draft Editor automatically enters lowercase text in uppercase

## Preconditions
- User is logged in.
- A project/manuscript with an available Draft exists.
- The Draft Editor is accessible.
- Caps Lock is turned off.
- Shift is not being held.

## Steps to Reproduce
1. Open a project/manuscript.
2. Navigate to the Draft section.
3. Click inside the actual Draft Editor.
4. Make sure Caps Lock is turned off.
5. Type lowercase text, for example:
   `once upon a time`
6. Observe the text while typing.

## Expected Result
Text should appear exactly as entered by the user.

Example:
`once upon a time`

## Actual Result
Lowercase text is automatically entered as uppercase.

Example:
`ONCE UPON A TIME`

The text appears in uppercase immediately while typing.

## Priority
High

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Draft Editor

## Evidence
Screen recording showing:
1. Caps Lock is turned off.
2. Lowercase text is typed into the Draft Editor.
3. The text appears in uppercase immediately while typing.

## Status
Open
