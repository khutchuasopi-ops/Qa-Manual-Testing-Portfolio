# BUG-003 – Event Can Be Created With Whitespace-Only Name

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
3. Enter only spaces in the Event Name field.
4. Complete any other required fields.
5. Click Create.
6. Check the Events list.

## Expected Result

The system should treat whitespace-only input as empty and prevent the Event from being created.

A validation message should inform the user that a valid Event name is required.

## Actual Result

The Event is created successfully even though the Event Name contains only spaces.

## Impact

This allows invalid data to be stored in the system. It may also make the Event difficult to identify or manage later.

## Status

Open
