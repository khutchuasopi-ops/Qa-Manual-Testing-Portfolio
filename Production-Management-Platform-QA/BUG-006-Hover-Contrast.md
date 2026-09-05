# BUG-006 — Button Text Becomes Unreadable on Hover

**Area:** UI / Usability
**Type:** Visual / Accessibility
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

The Cloud Import page is accessible and the relevant Cloud integration settings are available.

## Steps to Reproduce

1. Open **Files**.
2. Click **Import from Cloud**.
3. Click **Set up in Settings**.
4. Navigate to the relevant Cloud integration settings.
5. Locate the action button.
6. Move the mouse over the button.
7. Compare the normal and hover states.

## Actual Result

In the hover state, the button background becomes white while the text remains white. The text blends into the background and becomes practically unreadable.

## Expected Result

The hover state should maintain sufficient contrast between the button text and background.

## Impact

Users may have difficulty reading the action and identifying what the button does.
