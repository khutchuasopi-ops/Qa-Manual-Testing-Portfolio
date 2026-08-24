# BUG-005 – Template Accepts an Excessively Long Name

## Area

Templates

## Severity

Medium

## Priority

Medium

## Preconditions

- User is logged in.
- User has access to Templates.
- User is on the New Template page.

## Steps to Reproduce

1. Open the Templates section.
2. Select New Template.
3. Enter an extremely long string in the Template Name field.
4. Upload a valid document.
5. Complete the template creation process.
6. Save the Template.
7. Check the created Template in the Templates list.

## Expected Result

The Template Name field should enforce the supported character limit.

If the entered name exceeds the allowed limit, the system should display a clear validation message and prevent the Template from being saved.

## Actual Result

The system accepts an extremely long Template name and allows the Template to be created without displaying a validation message.

## Impact

Excessively long Template names may make Templates difficult to identify and can cause readability or layout issues in lists and other parts of the application.

## Status

Open
