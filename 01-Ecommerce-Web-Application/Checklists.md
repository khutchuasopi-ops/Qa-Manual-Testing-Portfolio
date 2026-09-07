# QA Checklists — E-commerce Web Application

## 1. Purpose

This document contains manual QA checklists for reviewing the main functionality and user-facing areas of the e-commerce web application.

The checklist is intended to support structured manual testing and help ensure that important areas are considered during test execution.

> **Note:** A checklist item should only be marked as completed when that check has actually been performed.

---

# 2. Login & Authentication Checklist

* [ ] Login page loads correctly
* [ ] Username field is visible
* [ ] Password field is visible
* [ ] Login button is visible and usable
* [ ] User can log in with valid credentials
* [ ] Login fails with invalid username
* [ ] Login fails with invalid password
* [ ] Login validation works when username is empty
* [ ] Login validation works when password is empty
* [ ] Login validation works when both fields are empty
* [ ] Invalid email format is handled correctly
* [ ] Appropriate error messages are displayed
* [ ] Password input is visually protected
* [ ] Logout option is available after successful login
* [ ] User can log out successfully

---

# 3. Product Search Checklist

* [ ] Search field is visible
* [ ] Search field accepts text input
* [ ] Search works with a valid product keyword
* [ ] Relevant products are displayed
* [ ] Search handles a non-existing keyword
* [ ] Appropriate no-results behavior is displayed
* [ ] Empty search input is handled correctly
* [ ] Partial product name is handled correctly if supported
* [ ] Search results contain relevant products
* [ ] User can open a product from search results
* [ ] Search results do not display unexpected errors

---

# 4. Product Details Checklist

* [ ] Product details page loads correctly
* [ ] Product name is displayed
* [ ] Product image is displayed
* [ ] Product price is displayed
* [ ] Product information is readable
* [ ] Available product sizes are displayed
* [ ] Available size can be selected
* [ ] Selected size is visually indicated
* [ ] Unavailable size is clearly identified
* [ ] Unavailable size cannot be selected for purchase
* [ ] Required product options are validated
* [ ] Product can be added to the cart when required options are selected
* [ ] Product cannot be added when required options are missing

---

# 5. Shopping Cart Checklist

* [ ] Cart page loads correctly
* [ ] Product can be added to the cart
* [ ] Added product is displayed in the cart
* [ ] Product name is correct
* [ ] Product image is correct
* [ ] Product price is correct
* [ ] Selected size is displayed correctly
* [ ] Product quantity is displayed correctly
* [ ] Quantity can be increased
* [ ] Quantity can be decreased
* [ ] Total updates after quantity changes
* [ ] Product can be removed from the cart
* [ ] Cart updates after product removal
* [ ] Empty cart state is displayed correctly
* [ ] Empty cart does not display incorrect product information
* [ ] Empty cart does not display an incorrect total
* [ ] Cart total is calculated correctly

---

# 6. Checkout Checklist

* [ ] User can navigate from cart to checkout
* [ ] Checkout page loads correctly
* [ ] Required customer information fields are visible
* [ ] Valid customer information is accepted
* [ ] Required fields are validated
* [ ] Checkout does not continue when required information is missing
* [ ] Appropriate validation messages are displayed
* [ ] Invalid input is handled correctly
* [ ] Delivery/shipping information can be entered
* [ ] Delivery/shipping information is displayed correctly
* [ ] Available payment methods are displayed
* [ ] Payment method can be selected where applicable
* [ ] Order summary is displayed
* [ ] Product information in the order summary is correct
* [ ] Product quantity in the order summary is correct
* [ ] Product price in the order summary is correct
* [ ] Final total is displayed
* [ ] Final total matches the expected amount
* [ ] User can place an order with valid information
* [ ] Appropriate order confirmation is displayed after successful order placement

---

# 7. Localization Checklist

* [ ] Language selector is visible
* [ ] Supported language options are displayed
* [ ] User can select another supported language
* [ ] Selected language is applied correctly
* [ ] Navigation labels are displayed in the selected language
* [ ] Buttons are displayed in the selected language
* [ ] Page titles are displayed in the selected language
* [ ] Product-related content is displayed consistently
* [ ] Cart content is displayed consistently
* [ ] Checkout content is displayed consistently
* [ ] Selected language remains consistent when navigating between supported pages
* [ ] No unexpected mixed-language content is displayed

---

# 8. UI & Navigation Checklist

* [ ] Main page loads without obvious UI errors
* [ ] Header is visible
* [ ] Main navigation is visible
* [ ] Navigation links are readable
* [ ] Navigation links lead to the expected pages
* [ ] Buttons are visible
* [ ] Buttons are readable
* [ ] Interactive elements respond to user actions
* [ ] Forms are readable
* [ ] Important content is not overlapping
* [ ] Major elements are properly positioned
* [ ] Product cards or main content elements are displayed correctly
* [ ] No obvious broken links are present
* [ ] No obvious layout issues are present

---

# 9. Negative Testing Checklist

* [ ] Invalid login username is handled correctly
* [ ] Invalid login password is handled correctly
* [ ] Empty login fields are handled correctly
* [ ] Invalid email format is handled correctly
* [ ] Invalid search input is handled correctly
* [ ] Empty search input is handled correctly
* [ ] Required product options are validated
* [ ] Unavailable product options cannot be selected
* [ ] Required checkout fields are validated
* [ ] Invalid checkout input is handled correctly
* [ ] Incorrect or unexpected input does not cause an obvious application error
* [ ] Appropriate validation or error messages are displayed

---

# 10. Validation Checklist

* [ ] Required fields are identified
* [ ] Empty required fields are rejected
* [ ] Invalid input is rejected where validation is expected
* [ ] Validation messages are understandable
* [ ] Validation messages appear near the relevant field where applicable
* [ ] User can correct invalid input
* [ ] Valid input is accepted
* [ ] Form submission does not proceed when required validation fails

---

# 11. User Flow Checklist

## Login Flow

* [ ] Open application
* [ ] Navigate to login
* [ ] Enter credentials
* [ ] Submit login
* [ ] Verify login result
* [ ] Logout successfully

## Product Purchase Flow

* [ ] Open application
* [ ] Search for a product
* [ ] Open product details
* [ ] Select required product options
* [ ] Add product to cart
* [ ] Open cart
* [ ] Verify product information
* [ ] Verify quantity
* [ ] Verify total
* [ ] Continue to checkout
* [ ] Enter required information
* [ ] Review order summary
* [ ] Place order where applicable
* [ ] Verify confirmation

---

# 12. Responsive Layout Checklist

These checks are included as **additional testing opportunities** and should only be marked as completed when responsive behavior has actually been tested.

* [ ] Main page displays correctly on a smaller screen
* [ ] Header remains usable
* [ ] Navigation remains accessible
* [ ] Product content remains readable
* [ ] Product images fit within the available screen area
* [ ] Buttons remain visible and usable
* [ ] Forms remain usable
* [ ] Shopping cart content remains readable
* [ ] Checkout content remains usable
* [ ] No obvious horizontal overflow is present
* [ ] No major element overlap is present

---

# 13. Cross-Browser Checklist

These checks are included as **additional testing opportunities**.

They should only be marked as completed when the application has actually been tested in the relevant browsers.

* [ ] Application loads correctly
* [ ] Login works correctly
* [ ] Product search works correctly
* [ ] Product details display correctly
* [ ] Shopping cart works correctly
* [ ] Checkout pages display correctly
* [ ] Main navigation works correctly
* [ ] Important UI elements display correctly
* [ ] No major browser-specific UI issue is observed

---

# 14. Regression Testing Checklist

Regression checks are included for use **after a relevant application change or defect fix**.

They should not be considered completed unless regression testing has actually been performed.

* [ ] Previously affected functionality was checked after the change
* [ ] Related user flow was checked
* [ ] Main login flow still works
* [ ] Product search still works
* [ ] Product selection still works
* [ ] Shopping cart still works
* [ ] Cart total still calculates correctly
* [ ] Checkout still works
* [ ] Localization still works
* [ ] Main navigation still works
* [ ] No obvious new issue was introduced

---

# 15. Defect Verification Checklist

Use this checklist when a reported defect has been fixed and is ready for verification.

* [ ] Original defect report is available
* [ ] Original reproduction steps are understood
* [ ] Fix is available for testing
* [ ] Original defect can no longer be reproduced
* [ ] Expected behavior is now observed
* [ ] Related functionality still works
* [ ] Related user flow was checked
* [ ] No obvious new issue was introduced
* [ ] Verification result is documented

> **Note:** Defect verification should only be marked as completed when the fix has actually been tested.

---

# 16. Evidence Checklist

When evidence is required for a test result or defect:

* [ ] Screenshot captured where useful
* [ ] Relevant application page is visible
* [ ] Error message is visible where applicable
* [ ] Important test data is visible where appropriate
* [ ] Evidence is connected to the relevant test case or bug report
* [ ] Confidential information is removed or protected
* [ ] Evidence is clear enough to support the reported result

---

# 17. Final QA Review Checklist

* [ ] Main application pages were reviewed
* [ ] Important user flows were considered
* [ ] Positive scenarios were considered
* [ ] Negative scenarios were considered
* [ ] Validation scenarios were considered
* [ ] UI issues were considered
* [ ] Localization was considered
* [ ] Identified defects were documented
* [ ] Severity was assigned to reported defects
* [ ] Priority was assigned to reported defects
* [ ] Test cases are linked to relevant scenarios
* [ ] Defects are linked to relevant test cases
* [ ] Test execution results are documented separately
* [ ] Unexecuted or unrecorded tests are clearly identified
* [ ] Confidential information is excluded from the public portfolio

---

# 18. Checklist Usage Notes

This checklist is a supporting QA document and does not replace detailed test cases.

Detailed execution results should be recorded in the **Test Execution Report**.

Defects identified during testing should be documented in the **Bug Reports** section.

Responsive testing, cross-browser testing, regression testing, and defect verification are included as reusable checklist areas and should only be marked as executed when those activities have actually been performed.

---

## Summary

The checklist covers the main areas of the e-commerce application:

* Authentication
* Product Search
* Product Details
* Shopping Cart
* Checkout
* Localization
* UI and Navigation
* Negative Testing
* Validation
* User Flows
* Responsive Checks
* Cross-Browser Checks
* Regression Checks
* Defect Verification
* Evidence
* Final QA Review

The checklist is designed to support a structured **Junior Manual QA Testing** workflow while keeping completed and potential testing activities clearly separated.
