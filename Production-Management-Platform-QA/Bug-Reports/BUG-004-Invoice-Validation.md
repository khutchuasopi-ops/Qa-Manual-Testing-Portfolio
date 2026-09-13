# BUG-004 — Negative Invoice Amount Displays `[object Object]`

**Area:** Invoice Management
**Type:** Validation / Error Handling
**Severity:** Medium
**Environment:** Test Environment

## Preconditions

* New Invoice form is available.

## Steps

1. Open **New Invoice**.
2. Enter all required valid fields.
3. Enter a negative amount, for example `-100`.
4. Submit the invoice.
5. Observe the validation message.

## Actual Result

Instead of a readable validation message, the system displays `[object Object]`.

## Expected Result

The invoice should not be created, and a clear validation message should inform the user that negative amounts are not allowed.

## Impact

The error message is not understandable to the user and exposes an internal object representation.
