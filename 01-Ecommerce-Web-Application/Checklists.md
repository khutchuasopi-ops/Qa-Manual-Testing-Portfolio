# E-commerce Web Application — QA Checklists

## 1. Purpose

This checklist provides a structured set of manual QA checks for the e-commerce web application.

It is designed to support:

* Smoke Testing
* Functional Testing
* Regression Testing
* UI Testing
* Localization Testing
* Cart and Checkout Validation
* Negative Testing
* Responsive and Cross-Browser Checks

The checklist is intended for quick verification before and after changes, fixes, or new releases.

---

# 2. Test Status

| Status | Meaning                          |
| ------ | -------------------------------- |
| ☐      | Not Checked                      |
| ✅      | Passed                           |
| ❌      | Failed                           |
| ⚠️     | Blocked / Requires Investigation |
| N/A    | Not Applicable                   |

---

# 3. Smoke Testing Checklist

## Application Availability

* ☐ Application loads successfully
* ☐ Main page loads without visible errors
* ☐ Main navigation is available
* ☐ Main UI elements are visible
* ☐ No obvious broken layout is present
* ☐ Search functionality is available
* ☐ Product pages can be opened
* ☐ Shopping cart can be opened
* ☐ Login page can be opened
* ☐ Checkout page can be reached

## Critical User Journey

* ☐ User can open the application
* ☐ User can log in with valid credentials
* ☐ User can search for a product
* ☐ User can open a product
* ☐ User can select required product options
* ☐ User can add a product to the cart
* ☐ User can open the cart
* ☐ User can proceed to checkout

### Smoke Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Notes:**

---

# 4. Authentication Checklist

## Login

* ☐ Login page loads correctly
* ☐ Username/email field is visible
* ☐ Password field is visible
* ☐ Login button is visible and enabled
* ☐ Valid credentials allow authentication
* ☐ Invalid username/email is rejected
* ☐ Invalid password is rejected
* ☐ Both invalid credentials are rejected
* ☐ Empty username/email is validated
* ☐ Empty password is validated
* ☐ Empty form submission is validated
* ☐ Malformed email is rejected
* ☐ Leading/trailing spaces are handled correctly
* ☐ Appropriate error messages are displayed

## Session / Logout

* ☐ User can log out successfully
* ☐ User is no longer authenticated after logout
* ☐ Protected content is not accessible after logout
* ☐ Browser Back navigation does not restore authenticated access
* ☐ Refresh behaves correctly after logout
* ☐ Session behavior after refresh is correct

### Authentication Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 5. Product Search Checklist

## Search Functionality

* ☐ Search field is visible
* ☐ Search can be submitted
* ☐ Existing product can be found
* ☐ Partial product name returns expected results
* ☐ Invalid keyword is handled correctly
* ☐ Empty search is handled correctly
* ☐ Whitespace-only search is handled correctly
* ☐ Search results are relevant
* ☐ No-result state is displayed correctly
* ☐ Search behavior is consistent with letter casing rules
* ☐ Special characters are handled safely
* ☐ Search results can be opened
* ☐ Product result links lead to the correct product

### Search Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 6. Product Details Checklist

## Product Information

* ☐ Product name is displayed
* ☐ Product price is displayed
* ☐ Product image is displayed
* ☐ Product availability is displayed
* ☐ Product information is readable
* ☐ Product image loads correctly
* ☐ Product page does not contain broken elements

## Product Options

* ☐ Available sizes/options are displayed
* ☐ Available size can be selected
* ☐ Unavailable size cannot be selected
* ☐ Selected size is visually identifiable
* ☐ Required product options are validated
* ☐ Selected options are retained when expected
* ☐ Product can be added to cart after valid selection

### Product Details Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 7. Shopping Cart Checklist

## Cart Contents

* ☐ Product can be added to cart
* ☐ Correct product appears in cart
* ☐ Correct product name is displayed
* ☐ Correct price is displayed
* ☐ Selected size/option is displayed
* ☐ Correct quantity is displayed
* ☐ Cart item count is correct

## Quantity

* ☐ Quantity can be increased
* ☐ Quantity can be decreased
* ☐ Minimum quantity is enforced
* ☐ Maximum quantity is enforced
* ☐ Zero quantity is handled correctly
* ☐ Negative quantity is rejected
* ☐ Invalid text input is rejected
* ☐ Unsupported decimal quantity is rejected

## Price Calculation

* ☐ Single-product total is correct
* ☐ Multiple-product total is correct
* ☐ Total updates after increasing quantity
* ☐ Total updates after decreasing quantity
* ☐ Total remains correct after repeated quantity changes
* ☐ Cart subtotal is mathematically correct
* ☐ Applicable additional charges are reflected correctly
* ☐ Cart total matches expected calculation

## Cart Actions

* ☐ Product can be removed
* ☐ Removing one product updates the cart correctly
* ☐ Removing the last product displays the empty-cart state
* ☐ Empty cart is handled correctly
* ☐ Cart state after page refresh behaves as expected

### Cart Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 8. Checkout Checklist

## Checkout Access

* ☐ Checkout can be opened from the cart
* ☐ Correct cart contents are displayed
* ☐ Checkout page loads correctly
* ☐ Required checkout fields are visible

## Customer Information

* ☐ Required fields are clearly identified
* ☐ Valid customer information is accepted
* ☐ Empty required fields are rejected
* ☐ Invalid email is rejected
* ☐ Invalid phone number is rejected
* ☐ Invalid address data is rejected
* ☐ Validation messages are understandable
* ☐ Input values are handled correctly

## Delivery

* ☐ Delivery options are displayed
* ☐ Available delivery option can be selected
* ☐ Selected delivery option is retained
* ☐ Delivery cost is reflected correctly when applicable

## Payment

* ☐ Available payment methods are displayed
* ☐ Payment method can be selected
* ☐ Required payment information is validated
* ☐ Invalid payment input is rejected where applicable

## Order Summary

* ☐ Product information is correct
* ☐ Quantity is correct
* ☐ Product prices are correct
* ☐ Shipping/delivery information is correct
* ☐ Checkout total matches the applicable cart total
* ☐ Final order summary is displayed correctly

## Order Submission

* ☐ Valid checkout information allows order submission
* ☐ Incomplete checkout cannot be submitted
* ☐ Invalid information prevents order submission
* ☐ Multiple rapid submissions do not create duplicate orders
* ☐ Successful order displays an appropriate confirmation
* ☐ Order state is handled correctly after submission

### Checkout Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 9. Localization Checklist

## Language Selection

* ☐ Language selector is available
* ☐ Supported languages are displayed
* ☐ User can change the language
* ☐ Selected language is visually identifiable
* ☐ Language selection persists when expected

## Translated Content

* ☐ Navigation labels use the selected language
* ☐ Buttons use the selected language
* ☐ Product information uses the selected language
* ☐ Form labels use the selected language
* ☐ Validation messages use the selected language
* ☐ Error messages use the selected language
* ☐ Checkout content uses the selected language
* ☐ No unexpected untranslated text is displayed
* ☐ No unexpected mixed-language content is displayed

### Localization Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 10. UI and Navigation Checklist

## Navigation

* ☐ Main navigation is visible
* ☐ Navigation links work correctly
* ☐ Links lead to the correct pages
* ☐ No broken links are observed
* ☐ Browser Back navigation behaves correctly
* ☐ Browser Forward navigation behaves correctly
* ☐ Page refresh does not cause unexpected behavior

## UI

* ☐ Buttons are visible
* ☐ Buttons have appropriate states
* ☐ Input fields are visible and usable
* ☐ Text is readable
* ☐ Images are displayed correctly
* ☐ No overlapping elements are visible
* ☐ No clipped content is visible
* ☐ No obvious alignment issues are present
* ☐ Error messages are visible
* ☐ Important actions provide appropriate visual feedback

### UI Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Bug ID(s):**

**Notes:**

---

# 11. Responsive Testing Checklist

## Desktop

* ☐ Main page displays correctly
* ☐ Navigation displays correctly
* ☐ Product page displays correctly
* ☐ Cart displays correctly
* ☐ Checkout displays correctly
* ☐ No horizontal scrolling occurs unexpectedly

## Mobile

* ☐ Main page is usable
* ☐ Navigation is usable
* ☐ Product information fits the viewport
* ☐ Product options are usable
* ☐ Cart is usable
* ☐ Quantity controls are usable
* ☐ Checkout fields are usable
* ☐ Buttons are accessible
* ☐ No important content is hidden
* ☐ No unexpected horizontal scrolling occurs

### Responsive Result

**Status:** ☐ PASS ☐ FAIL ☐ BLOCKED

**Device / Viewport:**

**Notes:**

---

# 12. Cross-Browser Checklist

Execute the critical user journey on supported browsers.

| Browser | Login | Search | Product | Cart | Checkout | Result |
| ------- | ----- | ------ | ------- | ---- | -------- | ------ |
| Chrome  | ☐     | ☐      | ☐       | ☐    | ☐        |        |
| Firefox | ☐     | ☐      | ☐       | ☐    | ☐        |        |
| Edge    | ☐     | ☐      | ☐       | ☐    | ☐        |        |
| Safari  | ☐     | ☐      | ☐       | ☐    | ☐        |        |

> Browser coverage should be limited to browsers officially supported by the application when that information is available.

---

# 13. Negative Testing Checklist

* ☐ Empty required fields
* ☐ Invalid credentials
* ☐ Invalid email format
* ☐ Invalid phone format
* ☐ Invalid search input
* ☐ Whitespace-only input
* ☐ Special characters
* ☐ Very long input
* ☐ Invalid quantity
* ☐ Zero quantity
* ☐ Negative quantity
* ☐ Unavailable product size
* ☐ Missing required product option
* ☐ Incomplete checkout
* ☐ Invalid checkout information
* ☐ Repeated order submission
* ☐ Refresh during an important user flow
* ☐ Back navigation during checkout
* ☐ Unexpected cart state

---

# 14. Regression Checklist

Regression testing should be performed after defect fixes or significant application changes.

## Authentication Regression

* ☐ Valid login
* ☐ Invalid email
* ☐ Invalid password
* ☐ Logout
* ☐ Protected page after logout
* ☐ Session after refresh

## Cart Regression

* ☐ Add product
* ☐ Change quantity
* ☐ Minimum quantity
* ☐ Maximum quantity
* ☐ Remove product
* ☐ Multiple products
* ☐ Cart total calculation
* ☐ Cart-to-checkout total consistency

## Localization Regression

* ☐ Change language
* ☐ Navigation translation
* ☐ Product translation
* ☐ Validation messages
* ☐ Checkout translation
* ☐ No mixed-language content

## Checkout Regression

* ☐ Required field validation
* ☐ Invalid email
* ☐ Invalid phone
* ☐ Delivery selection
* ☐ Payment selection
* ☐ Order summary
* ☐ Final total
* ☐ Order submission

---

# 15. Defect Verification Checklist

For every reported defect:

* ☐ Bug ID exists
* ☐ Bug has a clear title
* ☐ Reproduction steps are documented
* ☐ Expected result is documented
* ☐ Actual result is documented
* ☐ Severity is assigned
* ☐ Priority is assigned
* ☐ Environment is documented
* ☐ Evidence is attached where appropriate
* ☐ Developer fix is available
* ☐ Original failed test is retested
* ☐ Related regression tests are executed
* ☐ Defect status is updated
* ☐ Test execution report is updated

---

# 16. Evidence Checklist

When a test fails:

* ☐ Screenshot captured
* ☐ Relevant page/state is visible
* ☐ Sensitive information is removed
* ☐ Browser/environment is recorded
* ☐ Test Case ID is recorded
* ☐ Bug ID is recorded
* ☐ Reproduction steps are documented
* ☐ Expected vs Actual result is documented

---

# 17. Final QA Checklist

Before closing a test cycle:

* ☐ All planned critical tests are executed
* ☐ Failed tests have corresponding Bug IDs
* ☐ Blocked tests have documented blockers
* ☐ Retesting is completed for fixed defects
* ☐ Regression testing is completed
* ☐ Test execution report is updated
* ☐ Bug reports are updated
* ☐ Test summary report is updated
* ☐ Test evidence is organized
* ☐ No confidential information is exposed
* ☐ Final QA recommendation is documented

---

# 18. QA Checklist Summary

| Area                        | Coverage |
| --------------------------- | -------- |
| Smoke Testing               | ✅        |
| Authentication              | ✅        |
| Session / Logout            | ✅        |
| Product Search              | ✅        |
| Product Details             | ✅        |
| Shopping Cart               | ✅        |
| Quantity / Boundary Testing | ✅        |
| Price Calculation           | ✅        |
| Checkout                    | ✅        |
| Localization                | ✅        |
| UI / Navigation             | ✅        |
| Responsive Testing          | ✅        |
| Cross-Browser Testing       | ✅        |
| Negative Testing            | ✅        |
| Regression Testing          | ✅        |
| Defect Verification         | ✅        |
| Evidence Collection         | ✅        |

---

## QA Note

This checklist is intended as a practical manual testing aid. Individual checklist items should be supported by detailed test cases when formal test execution evidence is required.

Checklist results should never be marked as passed without actual verification.
