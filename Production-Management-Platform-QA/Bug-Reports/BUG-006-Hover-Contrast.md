# BUG-006 — Button Text Becomes Unreadable on Hover

**Area:** UI / Usability
**Type:** Visual / Accessibility
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

* Cloud Import page is accessible.
* Relevant Cloud integration settings are available.

## Steps

1. Open **Files**.
2. Click **Import from Cloud**.
3. Click **Set up in Settings**.
4. Navigate to the relevant Cloud integration settings.
5. Locate the action button.
6. Hover over the button.
7. Compare the normal and hover states.

## Actual Result

When hovering over the button, the background becomes white while the text remains white. As a result, the text blends into the background and becomes difficult to read.

## Expected Result

The button text should remain clearly readable in both normal and hover states, with sufficient contrast between the text and background.

## Impact

Users may have difficulty reading the button label and understanding the available action.
