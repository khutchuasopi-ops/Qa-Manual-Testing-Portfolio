# BUG-002 – Clear Search Icon Does Not Display Pointer Cursor

## Area

Search

## Severity

Low

## Priority

Low

## Preconditions

- User is logged in.
- Search functionality is available.

## Steps to Reproduce

1. Open the Search section.
2. Enter a search term.
3. Wait for the Clear icon to appear.
4. Move the mouse pointer over the Clear icon.
5. Click the Clear icon.

## Expected Result

The cursor should change to a pointer when hovering over the clickable Clear icon, indicating that the element is interactive.

The search input should also be cleared when the icon is clicked.

## Actual Result

The Clear icon is clickable, but the cursor does not change to a pointer when hovering over it. The default cursor remains visible.

## Impact

The cursor behavior may make the Clear icon appear less obviously interactive and can reduce consistency with other clickable elements in the interface.

## Status

Open
