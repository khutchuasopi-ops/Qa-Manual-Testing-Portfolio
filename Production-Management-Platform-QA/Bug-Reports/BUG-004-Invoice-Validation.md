:::writing{variant="document" id="zb3zqe" title="BUG-004 — Negative Invoice Amount Displays [object Object]"}
# BUG-004 — Negative Invoice Amount Displays `[object Object]`

**Area:** Invoice Management  
**Type:** Validation / Error Handling  
**Severity:** Medium  
**Environment:** Test Environment

## Preconditions

The New Invoice form is available.

## Steps to Reproduce

1. Open the **New Invoice** form.
2. Enter valid values in all required fields.
3. Enter a negative value in the **Amount** field, for example `-100`.
4. Submit the invoice.
5. Observe the validation response.

## Actual Result

Instead of displaying a readable validation message, the application displays:

`[object Object]`

## Expected Result

The invoice should be rejected and a clear validation message should inform the user that a negative amount is not allowed.

## Impact

The error message is not understandable to the user and exposes an internal object representation instead of a meaningful validation message.
:::
