# BUG-004 – Event Accepts an Excessively Long Name

## Area

Events

## Severity

Medium

## Priority

Medium

## Preconditions

- User is logged in.
- User has permission to create Events.

## Steps to Reproduce

1. Open the Events section.
2. Select Create Event.
3. Enter an extremely long string in the Event Name field.
4. Complete the remaining required fields.
5. Create the Event.
6. Open the created Event and check how the name is displayed.

## Expected Result

The system should enforce a reasonable character limit for the Event Name field.

If the maximum length is exceeded, the user should receive a clear validation message and the Event should not be created with an unsupported name.

## Actual Result

The system accepts an extremely long Event name and allows the Event to be created without displaying a validation message.

## Impact

Allowing excessively long names can make Events difficult to identify and may cause display or layout issues in lists, cards, tables, and other parts of the application.

## Status

Open
