# QA Checklists — E-commerce Web Application

## 1. Purpose

This checklist is used to support manual testing of the main functionality and user flows of the e-commerce web application.

It can be used for:

* Smoke Testing
* Functional Testing
* UI Checks
* Negative Testing
* Localization Checks
* Shopping Cart and Checkout Checks
* Regression / Retesting

### Status

* `[ ]` Not Checked
* `[x]` Passed
* `[F]` Failed
* `[B]` Blocked
* `[N/A]` Not Applicable

---

# 2. Smoke Testing Checklist

## Application Access

* [ ] Application opens successfully
* [ ] Main page loads correctly
* [ ] Main navigation is visible
* [ ] Main page does not show obvious errors

## Login

* [ ] Login page opens
* [ ] Username/email field is available
* [ ] Password field is available
* [ ] Valid login can be attempted
* [ ] Invalid login can be attempted
* [ ] Logout option is available after login

## Product

* [ ] Product list is visible
* [ ] Product details can be opened
* [ ] Product price is visible
* [ ] Product size can be selected when required
* [ ] Product can be added to cart

## Shopping Cart

* [ ] Cart can be opened
* [ ] Added product is displayed
* [ ] Product quantity is displayed
* [ ] Product price is displayed
* [ ] Cart total is displayed
* [ ] Product can be removed

## Checkout

* [ ] Checkout can be opened
* [ ] Required checkout fields are available
* [ ] Delivery information can be entered
* [ ] Payment section is available
* [ ] Order summary is displayed

---

# 3. Login and Authentication Checklist

## Valid Login

* [ ] Login with valid credentials
* [ ] User is redirected to the expected page
* [ ] Logged-in state is displayed correctly

## Invalid Login

* [ ] Invalid email/username is rejected
* [ ] Invalid password is rejected
* [ ] Invalid credentials show an appropriate message
* [ ] User is not incorrectly logged in

## Required Fields

* [ ] Empty username/email is handled correctly
* [ ] Empty password is handled correctly
* [ ] Both fields empty are handled correctly
* [ ] Required field validation is clear

## Logout

* [ ] Logout option is available
* [ ] User can log out successfully
* [ ] User is returned to the expected state/page

---

# 4. Product Search Checklist

* [ ] Search field is visible
* [ ] Search can be submitted
* [ ] Valid product name returns results
* [ ] Partial product name can be searched
* [ ] Invalid search term is handled correctly
* [ ] Empty search is handled correctly
* [ ] Search results are relevant
* [ ] Search result can be opened
* [ ] Product details open correctly from search results

---

# 5. Product Details Checklist

* [ ] Product name is displayed
* [ ] Product image is displayed
* [ ] Product price is displayed
* [ ] Product information is visible
* [ ] Available sizes are displayed
* [ ] Size can be selected
* [ ] Unavailable size cannot be selected incorrectly
* [ ] Selected size remains selected when expected
* [ ] Required product options are validated
* [ ] Product can be added to cart

---

# 6. Shopping Cart Checklist

## Cart Content

* [ ] Added product appears in cart
* [ ] Product name is correct
* [ ] Product price is correct
* [ ] Selected size is displayed when applicable
* [ ] Quantity is displayed correctly

## Quantity

* [ ] Quantity can be increased
* [ ] Quantity can be decreased
* [ ] Quantity cannot become invalid
* [ ] Quantity limits are handled correctly

## Price Calculation

* [ ] Product price is correct
* [ ] Quantity change updates the expected values
* [ ] Cart total is calculated correctly
* [ ] Cart total updates after quantity change

## Cart Actions

* [ ] Product can be removed
* [ ] Empty cart is displayed correctly
* [ ] User can continue from cart to checkout

---

# 7. Checkout Checklist

## Checkout Access

* [ ] Checkout can be opened from the cart
* [ ] Checkout page loads correctly
* [ ] Order information is visible

## Customer Information

* [ ] Required fields are visible
* [ ] Valid information can be entered
* [ ] Empty required fields are handled correctly
* [ ] Invalid input is handled correctly

## Delivery

* [ ] Delivery information can be entered
* [ ] Required delivery fields are validated
* [ ] Delivery information appears correctly in the order summary

## Payment

* [ ] Payment section is available
* [ ] Required payment fields are displayed
* [ ] Invalid or missing payment information is handled correctly

## Order Summary

* [ ] Product information is correct
* [ ] Quantity is correct
* [ ] Price is correct
* [ ] Total is correct
* [ ] Entered information is displayed correctly

## Order Completion

* [ ] Order can be submitted when valid information is provided
* [ ] Successful order result is displayed correctly
* [ ] User receives appropriate confirmation

---

# 8. Localization Checklist

* [ ] Language selection is available
* [ ] User can select another language
* [ ] Selected language is reflected in the interface
* [ ] Main page content changes to the selected language
* [ ] Navigation content changes to the selected language
* [ ] Product-related content changes to the selected language
* [ ] Checkout-related content changes to the selected language
* [ ] No unexpected mixed-language content is displayed

---

# 9. UI and Navigation Checklist

## Navigation

* [ ] Main navigation is visible
* [ ] Navigation links work
* [ ] Important pages are accessible
* [ ] Back/navigation actions work as expected

## UI Elements

* [ ] Buttons are visible
* [ ] Buttons can be used
* [ ] Input fields are visible
* [ ] Labels are understandable
* [ ] Important information is visible
* [ ] No obvious overlapping elements are present
* [ ] No obvious broken UI elements are present

---

# 10. Responsive Testing Checklist

Where supported, check the main user flows on different screen sizes.

* [ ] Main page remains usable
* [ ] Navigation remains accessible
* [ ] Product information remains readable
* [ ] Product images display correctly
* [ ] Search remains usable
* [ ] Cart remains usable
* [ ] Checkout remains usable
* [ ] Buttons remain accessible
* [ ] Input fields remain usable
* [ ] No obvious horizontal overflow is present

> Responsive checks are documented as additional coverage and should only be marked as executed when actually tested.

---

# 11. Cross-Browser Checklist

Where supported, verify the main flows in supported browsers.

* [ ] Application opens correctly
* [ ] Login works as expected
* [ ] Search works as expected
* [ ] Product details display correctly
* [ ] Add to cart works as expected
* [ ] Cart calculations display correctly
* [ ] Checkout pages display correctly
* [ ] Navigation works correctly
* [ ] No obvious browser-specific UI issue is observed

> Cross-browser items are coverage checks. They should not be reported as executed results unless they were actually tested.

---

# 12. Negative Testing Checklist

## Login

* [ ] Invalid email/username
* [ ] Invalid password
* [ ] Empty email/username
* [ ] Empty password
* [ ] Both fields empty

## Search

* [ ] Invalid search term
* [ ] Empty search
* [ ] Partial search term
* [ ] Special characters where applicable

## Product

* [ ] Attempt to continue without selecting a required size
* [ ] Unavailable size selection

## Cart

* [ ] Invalid quantity
* [ ] Minimum quantity
* [ ] Maximum quantity
* [ ] Removing the only product

## Checkout

* [ ] Empty required fields
* [ ] Invalid input
* [ ] Incomplete delivery information
* [ ] Incomplete payment information

---

# 13. Regression / Retesting Checklist

Use this checklist after a defect is reported as fixed.

## Defect Verification

* [ ] Reproduce the original issue
* [ ] Apply or verify the reported fix
* [ ] Repeat the original steps
* [ ] Confirm the expected result
* [ ] Check related functionality
* [ ] Record the new result

## Related Areas

* [ ] Login changes do not affect normal login
* [ ] Cart changes do not affect product selection
* [ ] Quantity changes do not cause incorrect totals
* [ ] Localization changes do not cause unexpected mixed-language content
* [ ] Checkout changes do not affect order information

> Retesting and regression checks should only be marked as completed when they are actually performed.

---

# 14. Defect Verification

Known defects in this project:

* [ ] BUG-001 — Localization
* [ ] BUG-002 — Shopping Cart
* [ ] BUG-003 — Login / Authentication

For each defect:

* [ ] Original issue can be reproduced
* [ ] Steps are documented
* [ ] Expected result is clear
* [ ] Actual result is recorded
* [ ] Fix can be verified when available
* [ ] Final retest result is recorded

---

# 15. Evidence Checklist

When evidence is safe to include:

* [ ] Screenshot captured
* [ ] Screenshot does not contain confidential information
* [ ] Screenshot does not contain real credentials
* [ ] Screenshot does not contain sensitive user information
* [ ] Screenshot clearly shows the issue
* [ ] Evidence is connected to the relevant bug report

---

# 16. Final QA Checklist

* [ ] Main functionality reviewed
* [ ] Test scenarios documented
* [ ] Test cases documented
* [ ] Available test execution results recorded
* [ ] Missing historical results marked as NOT RECORDED
* [ ] Defects documented
* [ ] Severity assigned
* [ ] Priority assigned
* [ ] Expected and actual results documented
* [ ] Related test cases identified
* [ ] Test summary prepared
* [ ] Confidential information removed
* [ ] Final documentation reviewed

---

# 17. Notes

This checklist is part of a Junior Manual QA portfolio project.

It represents practical manual testing coverage and documentation.

Checklist items should only be marked as completed when the corresponding check has actually been performed.
