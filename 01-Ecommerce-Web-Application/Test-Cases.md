# Test Cases — E-commerce Web Application

## Test Case Overview

This document contains detailed manual test cases for the e-commerce web application.

The test cases are derived from the high-level test scenarios and cover positive, negative, functional, validation, UI, and user-flow testing.

### Test Case Status

All test cases are initially marked as **Not Executed** because test execution will be performed separately.

---

# 1. Login

## TC-001 — Login with Valid Credentials

| Field                | Details                                                          |
| -------------------- | ---------------------------------------------------------------- |
| **Test Case ID**     | TC-001                                                           |
| **Title**            | Verify that a user can log in with valid credentials             |
| **Related Scenario** | TS-001, TS-002                                                   |
| **Test Type**        | Functional / Positive                                            |
| **Priority**         | High                                                             |
| **Preconditions**    | The login page is accessible and the user has valid credentials. |
| **Test Data**        | Valid username and valid password                                |
| **Status**           | Not Executed                                                     |

### Test Steps

1. Open the application login page.
2. Enter a valid username.
3. Enter a valid password.
4. Click the **Login** button.

### Expected Result

The user should be successfully authenticated and redirected to the appropriate application page.

### Actual Result

Not Executed.

---

## TC-002 — Login with Invalid Username

| Field                | Details                                          |
| -------------------- | ------------------------------------------------ |
| **Test Case ID**     | TC-002                                           |
| **Title**            | Verify that login fails with an invalid username |
| **Related Scenario** | TS-002                                           |
| **Test Type**        | Functional / Negative                            |
| **Priority**         | High                                             |
| **Preconditions**    | The login page is accessible.                    |
| **Test Data**        | Invalid username and valid password              |
| **Status**           | Not Executed                                     |

### Test Steps

1. Open the login page.
2. Enter an invalid username.
3. Enter a valid password.
4. Click **Login**.

### Expected Result

The user should not be authenticated and an appropriate error message should be displayed.

### Actual Result

Not Executed.

---

## TC-003 — Login with Invalid Password

| Field                | Details                                          |
| -------------------- | ------------------------------------------------ |
| **Test Case ID**     | TC-003                                           |
| **Title**            | Verify that login fails with an invalid password |
| **Related Scenario** | TS-002                                           |
| **Test Type**        | Functional / Negative                            |
| **Priority**         | High                                             |
| **Preconditions**    | The login page is accessible.                    |
| **Test Data**        | Valid username and invalid password              |
| **Status**           | Not Executed                                     |

### Test Steps

1. Open the login page.
2. Enter a valid username.
3. Enter an invalid password.
4. Click **Login**.

### Expected Result

The user should not be authenticated and an appropriate error message should be displayed.

### Actual Result

Not Executed.

---

## TC-004 — Login with Empty Username

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-004                                             |
| **Title**            | Verify validation when the username field is empty |
| **Related Scenario** | TS-003                                             |
| **Test Type**        | Functional / Negative / Validation                 |
| **Priority**         | High                                               |
| **Preconditions**    | The login page is accessible.                      |
| **Test Data**        | Empty username and valid password                  |
| **Status**           | Not Executed                                       |

### Test Steps

1. Open the login page.
2. Leave the username field empty.
3. Enter a valid password.
4. Click **Login**.

### Expected Result

The user should not be authenticated and a validation message should indicate that the username is required.

### Actual Result

Not Executed.

---

## TC-005 — Login with Empty Password

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-005                                             |
| **Title**            | Verify validation when the password field is empty |
| **Related Scenario** | TS-003                                             |
| **Test Type**        | Functional / Negative / Validation                 |
| **Priority**         | High                                               |
| **Preconditions**    | The login page is accessible.                      |
| **Test Data**        | Valid username and empty password                  |
| **Status**           | Not Executed                                       |

### Test Steps

1. Open the login page.
2. Enter a valid username.
3. Leave the password field empty.
4. Click **Login**.

### Expected Result

The user should not be authenticated and a validation message should indicate that the password is required.

### Actual Result

Not Executed.

---

## TC-006 — Login with Empty Username and Password

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-006                                             |
| **Title**            | Verify validation when both login fields are empty |
| **Related Scenario** | TS-003                                             |
| **Test Type**        | Functional / Negative / Validation                 |
| **Priority**         | High                                               |
| **Preconditions**    | The login page is accessible.                      |
| **Test Data**        | Empty username and empty password                  |
| **Status**           | Not Executed                                       |

### Test Steps

1. Open the login page.
2. Leave the username field empty.
3. Leave the password field empty.
4. Click **Login**.

### Expected Result

The user should not be authenticated and appropriate validation messages should be displayed.

### Actual Result

Not Executed.

---

## TC-007 — Logout

| Field                | Details                                               |
| -------------------- | ----------------------------------------------------- |
| **Test Case ID**     | TC-007                                                |
| **Title**            | Verify that a logged-in user can log out successfully |
| **Related Scenario** | TS-004                                                |
| **Test Type**        | Functional / Positive                                 |
| **Priority**         | Medium                                                |
| **Preconditions**    | The user is successfully logged in.                   |
| **Test Data**        | Valid logged-in user session                          |
| **Status**           | Not Executed                                          |

### Test Steps

1. Log in with valid credentials.
2. Locate the **Logout** option.
3. Click **Logout**.

### Expected Result

The user should be logged out and redirected to the appropriate login or public page.

### Actual Result

Not Executed.

---

# 2. Product Search

## TC-008 — Search for an Existing Product

| Field                | Details                                     |
| -------------------- | ------------------------------------------- |
| **Test Case ID**     | TC-008                                      |
| **Title**            | Verify product search using a valid keyword |
| **Related Scenario** | TS-005, TS-006                              |
| **Test Type**        | Functional / Positive                       |
| **Priority**         | High                                        |
| **Preconditions**    | The application is accessible.              |
| **Test Data**        | Valid product name or keyword               |
| **Status**           | Not Executed                                |

### Test Steps

1. Open the application.
2. Locate the search field.
3. Enter a valid product keyword.
4. Submit the search.

### Expected Result

Products relevant to the entered keyword should be displayed.

### Actual Result

Not Executed.

---

## TC-009 — Search with Invalid Keyword

| Field                | Details                                                               |
| -------------------- | --------------------------------------------------------------------- |
| **Test Case ID**     | TC-009                                                                |
| **Title**            | Verify search behavior with a keyword that does not match any product |
| **Related Scenario** | TS-006                                                                |
| **Test Type**        | Functional / Negative                                                 |
| **Priority**         | High                                                                  |
| **Preconditions**    | The application is accessible.                                        |
| **Test Data**        | Non-existing product keyword                                          |
| **Status**           | Not Executed                                                          |

### Test Steps

1. Open the application.
2. Enter a non-existing product keyword.
3. Submit the search.

### Expected Result

The application should display an appropriate no-results message or an empty result state.

### Actual Result

Not Executed.

---

## TC-010 — Search with Empty Search Field

| Field                | Details                                               |
| -------------------- | ----------------------------------------------------- |
| **Test Case ID**     | TC-010                                                |
| **Title**            | Verify search behavior when the search field is empty |
| **Related Scenario** | TS-007                                                |
| **Test Type**        | Functional / Negative / Validation                    |
| **Priority**         | Medium                                                |
| **Preconditions**    | The application is accessible.                        |
| **Test Data**        | Empty search field                                    |
| **Status**           | Not Executed                                          |

### Test Steps

1. Open the application.
2. Leave the search field empty.
3. Submit the search.

### Expected Result

The application should handle the empty search appropriately without errors.

### Actual Result

Not Executed.

---

## TC-011 — Verify Search Result Relevance

| Field                | Details                                                        |
| -------------------- | -------------------------------------------------------------- |
| **Test Case ID**     | TC-011                                                         |
| **Title**            | Verify that search results are relevant to the entered keyword |
| **Related Scenario** | TS-008                                                         |
| **Test Type**        | Functional                                                     |
| **Priority**         | High                                                           |
| **Preconditions**    | The application contains products matching the test keyword.   |
| **Test Data**        | Valid product keyword                                          |
| **Status**           | Not Executed                                                   |

### Test Steps

1. Enter a valid product keyword.
2. Submit the search.
3. Review the returned products.

### Expected Result

Displayed products should be relevant to the entered search keyword.

### Actual Result

Not Executed.

---

## TC-012 — Search Using Partial Product Name

| Field                | Details                                                       |
| -------------------- | ------------------------------------------------------------- |
| **Test Case ID**     | TC-012                                                        |
| **Title**            | Verify search behavior when a partial product name is entered |
| **Related Scenario** | TS-006, TS-008                                                |
| **Test Type**        | Functional                                                    |
| **Priority**         | Medium                                                        |
| **Preconditions**    | The application is accessible.                                |
| **Test Data**        | Partial product name                                          |
| **Status**           | Not Executed                                                  |

### Test Steps

1. Enter part of an existing product name.
2. Submit the search.
3. Review the search results.

### Expected Result

The application should return relevant results if partial keyword searching is supported.

### Actual Result

Not Executed.

---

## TC-013 — Search Result Navigation

| Field                | Details                                                   |
| -------------------- | --------------------------------------------------------- |
| **Test Case ID**     | TC-013                                                    |
| **Title**            | Verify that a user can open a product from search results |
| **Related Scenario** | TS-005, TS-008                                            |
| **Test Type**        | Functional / Positive                                     |
| **Priority**         | High                                                      |
| **Preconditions**    | Search results are displayed.                             |
| **Test Data**        | Existing product from search results                      |
| **Status**           | Not Executed                                              |

### Test Steps

1. Perform a valid product search.
2. Select a product from the results.
3. Click the product.

### Expected Result

The selected product's details page should open.

### Actual Result

Not Executed.

---

# 3. Product Page and Size Selection

## TC-014 — Verify Product Information

| Field                | Details                                                  |
| -------------------- | -------------------------------------------------------- |
| **Test Case ID**     | TC-014                                                   |
| **Title**            | Verify product information displayed on the product page |
| **Related Scenario** | TS-009                                                   |
| **Test Type**        | Functional / UI                                          |
| **Priority**         | High                                                     |
| **Preconditions**    | A product details page is accessible.                    |
| **Test Data**        | Existing product                                         |
| **Status**           | Not Executed                                             |

### Test Steps

1. Open a product details page.
2. Review the product name.
3. Review the product image.
4. Review the product price.
5. Review available product information.

### Expected Result

All relevant product information should be displayed correctly and consistently.

### Actual Result

Not Executed.

---

## TC-015 — Select Available Product Size

| Field                | Details                                               |
| -------------------- | ----------------------------------------------------- |
| **Test Case ID**     | TC-015                                                |
| **Title**            | Verify that an available product size can be selected |
| **Related Scenario** | TS-010                                                |
| **Test Type**        | Functional / Positive                                 |
| **Priority**         | High                                                  |
| **Preconditions**    | A product with available sizes is displayed.          |
| **Test Data**        | Available product size                                |
| **Status**           | Not Executed                                          |

### Test Steps

1. Open a product details page.
2. Locate the size selector.
3. Select an available size.

### Expected Result

The selected size should be visually indicated and associated with the product selection.

### Actual Result

Not Executed.

---

## TC-016 — Verify Unavailable Product Size

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-016                                             |
| **Title**            | Verify behavior when a product size is unavailable |
| **Related Scenario** | TS-011                                             |
| **Test Type**        | Functional / Negative                              |
| **Priority**         | High                                               |
| **Preconditions**    | A product with unavailable sizes is displayed.     |
| **Test Data**        | Unavailable product size                           |
| **Status**           | Not Executed                                       |

### Test Steps

1. Open a product details page.
2. Locate an unavailable size.
3. Attempt to select the unavailable size.

### Expected Result

The unavailable size should be clearly identified and should not be selectable for purchase.

### Actual Result

Not Executed.

---

## TC-017 — Verify Selected Size is Retained

| Field                | Details                                                                               |
| -------------------- | ------------------------------------------------------------------------------------- |
| **Test Case ID**     | TC-017                                                                                |
| **Title**            | Verify that the selected product size is retained when adding the product to the cart |
| **Related Scenario** | TS-012                                                                                |
| **Test Type**        | Functional                                                                            |
| **Priority**         | High                                                                                  |
| **Preconditions**    | A product with available sizes is displayed.                                          |
| **Test Data**        | Available product and selected size                                                   |
| **Status**           | Not Executed                                                                          |

### Test Steps

1. Open a product details page.
2. Select an available size.
3. Add the product to the cart.
4. Open the shopping cart.

### Expected Result

The selected product size should be displayed correctly in the shopping cart.

### Actual Result

Not Executed.

---

## TC-018 — Add Product Without Selecting Required Size

| Field                | Details                                                           |
| -------------------- | ----------------------------------------------------------------- |
| **Test Case ID**     | TC-018                                                            |
| **Title**            | Verify validation when a required product size is not selected    |
| **Related Scenario** | TS-010, TS-012                                                    |
| **Test Type**        | Functional / Negative / Validation                                |
| **Priority**         | High                                                              |
| **Preconditions**    | The product requires size selection before adding it to the cart. |
| **Test Data**        | Product with no selected size                                     |
| **Status**           | Not Executed                                                      |

### Test Steps

1. Open a product details page.
2. Do not select a size.
3. Click **Add to Cart**.

### Expected Result

The product should not be added without a required size selection and an appropriate validation message should be displayed.

### Actual Result

Not Executed.

---

## TC-019 — Verify Product Image and Price

| Field                | Details                                                |
| -------------------- | ------------------------------------------------------ |
| **Test Case ID**     | TC-019                                                 |
| **Title**            | Verify product image and price are displayed correctly |
| **Related Scenario** | TS-009                                                 |
| **Test Type**        | UI / Functional                                        |
| **Priority**         | Medium                                                 |
| **Preconditions**    | A product details page is accessible.                  |
| **Test Data**        | Existing product                                       |
| **Status**           | Not Executed                                           |

### Test Steps

1. Open a product details page.
2. Check the product image.
3. Check the displayed price.
4. Compare the information with the corresponding product information.

### Expected Result

The correct product image and price should be displayed without visual or content-related errors.

### Actual Result

Not Executed.

---

# 4. Shopping Cart

## TC-020 — Add Product to Cart

| Field                | Details                                                 |
| -------------------- | ------------------------------------------------------- |
| **Test Case ID**     | TC-020                                                  |
| **Title**            | Verify that a product can be added to the shopping cart |
| **Related Scenario** | TS-013                                                  |
| **Test Type**        | Functional / Positive                                   |
| **Priority**         | High                                                    |
| **Preconditions**    | A valid product is available for purchase.              |
| **Test Data**        | Available product                                       |
| **Status**           | Not Executed                                            |

### Test Steps

1. Open a product details page.
2. Select required product options.
3. Click **Add to Cart**.
4. Open the shopping cart.

### Expected Result

The selected product should be added to the shopping cart with the correct information.

### Actual Result

Not Executed.

---

## TC-021 — Verify Product Information in Cart

| Field                | Details                                                   |
| -------------------- | --------------------------------------------------------- |
| **Test Case ID**     | TC-021                                                    |
| **Title**            | Verify product information displayed in the shopping cart |
| **Related Scenario** | TS-014                                                    |
| **Test Type**        | Functional / UI                                           |
| **Priority**         | High                                                      |
| **Preconditions**    | At least one product has been added to the cart.          |
| **Test Data**        | Product added to cart                                     |
| **Status**           | Not Executed                                              |

### Test Steps

1. Add a product to the cart.
2. Open the shopping cart.
3. Review product name, image, price, size, and quantity where applicable.

### Expected Result

The cart should display accurate product information.

### Actual Result

Not Executed.

---

## TC-022 — Increase Product Quantity

| Field                | Details                                                   |
| -------------------- | --------------------------------------------------------- |
| **Test Case ID**     | TC-022                                                    |
| **Title**            | Verify that product quantity can be increased in the cart |
| **Related Scenario** | TS-015                                                    |
| **Test Type**        | Functional / Positive                                     |
| **Priority**         | High                                                      |
| **Preconditions**    | The cart contains at least one product.                   |
| **Test Data**        | Product quantity increased from 1 to 2                    |
| **Status**           | Not Executed                                              |

### Test Steps

1. Open the shopping cart.
2. Increase the product quantity.
3. Observe the updated quantity.
4. Observe the updated total price.

### Expected Result

The product quantity should increase correctly and the total price should be recalculated accordingly.

### Actual Result

Not Executed.

---

## TC-023 — Decrease Product Quantity

| Field                | Details                                                     |
| -------------------- | ----------------------------------------------------------- |
| **Test Case ID**     | TC-023                                                      |
| **Title**            | Verify that product quantity can be decreased in the cart   |
| **Related Scenario** | TS-015                                                      |
| **Test Type**        | Functional                                                  |
| **Priority**         | High                                                        |
| **Preconditions**    | The cart contains a product with quantity greater than one. |
| **Test Data**        | Product quantity decreased from 2 to 1                      |
| **Status**           | Not Executed                                                |

### Test Steps

1. Open the shopping cart.
2. Decrease the product quantity.
3. Observe the updated quantity.
4. Observe the updated total price.

### Expected Result

The quantity should decrease correctly and the total price should be recalculated accordingly.

### Actual Result

Not Executed.

---

## TC-024 — Verify Cart Total Calculation

| Field                | Details                                                     |
| -------------------- | ----------------------------------------------------------- |
| **Test Case ID**     | TC-024                                                      |
| **Title**            | Verify that the shopping cart total is calculated correctly |
| **Related Scenario** | TS-016                                                      |
| **Test Type**        | Functional                                                  |
| **Priority**         | High                                                        |
| **Preconditions**    | The cart contains at least one product.                     |
| **Test Data**        | Product price and quantity                                  |
| **Status**           | Not Executed                                                |

### Test Steps

1. Add a product to the cart.
2. Note the product price.
3. Note the selected quantity.
4. Calculate the expected total manually.
5. Compare it with the displayed cart total.

### Expected Result

The displayed cart total should match the expected calculation based on product price and quantity.

### Actual Result

Not Executed.

---

## TC-025 — Remove Product from Cart

| Field                | Details                                                     |
| -------------------- | ----------------------------------------------------------- |
| **Test Case ID**     | TC-025                                                      |
| **Title**            | Verify that a product can be removed from the shopping cart |
| **Related Scenario** | TS-017                                                      |
| **Test Type**        | Functional / Positive                                       |
| **Priority**         | High                                                        |
| **Preconditions**    | The cart contains at least one product.                     |
| **Test Data**        | Existing cart product                                       |
| **Status**           | Not Executed                                                |

### Test Steps

1. Open the shopping cart.
2. Locate the product.
3. Click the **Remove** option.
4. Review the cart.

### Expected Result

The selected product should be removed from the cart and the cart information should be updated.

### Actual Result

Not Executed.

---

## TC-026 — Verify Empty Shopping Cart

| Field                | Details                                       |
| -------------------- | --------------------------------------------- |
| **Test Case ID**     | TC-026                                        |
| **Title**            | Verify the behavior of an empty shopping cart |
| **Related Scenario** | TS-018                                        |
| **Test Type**        | Functional / UI                               |
| **Priority**         | Medium                                        |
| **Preconditions**    | The shopping cart is empty.                   |
| **Test Data**        | Empty cart                                    |
| **Status**           | Not Executed                                  |

### Test Steps

1. Open the shopping cart.
2. Review the displayed content.

### Expected Result

The application should clearly indicate that the cart is empty and should not display incorrect product or total information.

### Actual Result

Not Executed.

---

# 5. Checkout

## TC-027 — Navigate from Cart to Checkout

| Field                | Details                                              |
| -------------------- | ---------------------------------------------------- |
| **Test Case ID**     | TC-027                                               |
| **Title**            | Verify navigation from the shopping cart to checkout |
| **Related Scenario** | TS-019                                               |
| **Test Type**        | Functional / Positive                                |
| **Priority**         | High                                                 |
| **Preconditions**    | The cart contains at least one valid product.        |
| **Test Data**        | Product in cart                                      |
| **Status**           | Not Executed                                         |

### Test Steps

1. Add a product to the cart.
2. Open the cart.
3. Click the checkout button.

### Expected Result

The user should be successfully navigated to the checkout page.

### Actual Result

Not Executed.

---

## TC-028 — Checkout with Valid Information

| Field                | Details                                                                |
| -------------------- | ---------------------------------------------------------------------- |
| **Test Case ID**     | TC-028                                                                 |
| **Title**            | Verify checkout with valid customer information                        |
| **Related Scenario** | TS-020                                                                 |
| **Test Type**        | Functional / Positive                                                  |
| **Priority**         | High                                                                   |
| **Preconditions**    | The cart contains a product and checkout is accessible.                |
| **Test Data**        | Valid name, address, city, postal code, and other required information |
| **Status**           | Not Executed                                                           |

### Test Steps

1. Proceed to checkout.
2. Enter valid customer information.
3. Complete all required fields.
4. Continue to the next checkout step.

### Expected Result

The information should be accepted and the user should be allowed to continue the checkout process.

### Actual Result

Not Executed.

---

## TC-029 — Checkout with Missing Required Information

| Field                | Details                                                         |
| -------------------- | --------------------------------------------------------------- |
| **Test Case ID**     | TC-029                                                          |
| **Title**            | Verify checkout validation when required information is missing |
| **Related Scenario** | TS-020, TS-027                                                  |
| **Test Type**        | Functional / Negative / Validation                              |
| **Priority**         | High                                                            |
| **Preconditions**    | Checkout page is accessible.                                    |
| **Test Data**        | One or more required fields left empty                          |
| **Status**           | Not Executed                                                    |

### Test Steps

1. Proceed to checkout.
2. Leave one or more required fields empty.
3. Click the button to continue.

### Expected Result

The user should not be allowed to continue until required information is provided. Appropriate validation messages should be displayed.

### Actual Result

Not Executed.

---

## TC-030 — Checkout with Invalid Input Data

| Field                | Details                                                      |
| -------------------- | ------------------------------------------------------------ |
| **Test Case ID**     | TC-030                                                       |
| **Title**            | Verify checkout validation with invalid customer information |
| **Related Scenario** | TS-020, TS-028                                               |
| **Test Type**        | Functional / Negative / Validation                           |
| **Priority**         | High                                                         |
| **Preconditions**    | Checkout page is accessible.                                 |
| **Test Data**        | Invalid input in one or more checkout fields                 |
| **Status**           | Not Executed                                                 |

### Test Steps

1. Proceed to checkout.
2. Enter invalid data into a relevant field.
3. Attempt to continue.

### Expected Result

The application should validate the entered data and display an appropriate error message when invalid information is submitted.

### Actual Result

Not Executed.

---

## TC-031 — Verify Delivery Information

| Field                | Details                                                 |
| -------------------- | ------------------------------------------------------- |
| **Test Case ID**     | TC-031                                                  |
| **Title**            | Verify delivery or shipping information during checkout |
| **Related Scenario** | TS-021                                                  |
| **Test Type**        | Functional                                              |
| **Priority**         | High                                                    |
| **Preconditions**    | Checkout is accessible.                                 |
| **Test Data**        | Valid delivery information                              |
| **Status**           | Not Executed                                            |

### Test Steps

1. Proceed to checkout.
2. Enter valid delivery information.
3. Review the entered information.
4. Continue to the next step.

### Expected Result

The delivery information should be accepted and displayed correctly.

### Actual Result

Not Executed.

---

## TC-032 — Verify Payment Method

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-032                                             |
| **Title**            | Verify available payment method options            |
| **Related Scenario** | TS-022                                             |
| **Test Type**        | Functional / UI                                    |
| **Priority**         | High                                               |
| **Preconditions**    | The checkout process has reached the payment step. |
| **Test Data**        | Available payment method                           |
| **Status**           | Not Executed                                       |

### Test Steps

1. Proceed through checkout to the payment step.
2. Review the available payment methods.
3. Select an available payment method where applicable.

### Expected Result

Available payment methods should be displayed correctly and selectable according to the application's requirements.

### Actual Result

Not Executed.

---

## TC-033 — Verify Order Summary and Total

| Field                | Details                                                      |
| -------------------- | ------------------------------------------------------------ |
| **Test Case ID**     | TC-033                                                       |
| **Title**            | Verify order summary and total amount before order placement |
| **Related Scenario** | TS-023                                                       |
| **Test Type**        | Functional                                                   |
| **Priority**         | High                                                         |
| **Preconditions**    | The user has reached the order summary step.                 |
| **Test Data**        | Product, quantity, price, and applicable charges             |
| **Status**           | Not Executed                                                 |

### Test Steps

1. Proceed to the order summary.
2. Review product information.
3. Review quantity.
4. Review product price.
5. Review the final total amount.

### Expected Result

The order summary should accurately reflect the selected products, quantities, prices, and final total.

### Actual Result

Not Executed.

---

## TC-034 — Successful Order Placement

| Field                | Details                                                                                 |
| -------------------- | --------------------------------------------------------------------------------------- |
| **Test Case ID**     | TC-034                                                                                  |
| **Title**            | Verify that an order can be placed successfully                                         |
| **Related Scenario** | TS-024                                                                                  |
| **Test Type**        | Functional / Positive                                                                   |
| **Priority**         | High                                                                                    |
| **Preconditions**    | A valid product is in the cart and all required checkout information has been provided. |
| **Test Data**        | Valid checkout information                                                              |
| **Status**           | Not Executed                                                                            |

### Test Steps

1. Complete the checkout process with valid information.
2. Review the order summary.
3. Submit/place the order.

### Expected Result

The order should be successfully submitted and an appropriate confirmation message or confirmation page should be displayed.

### Actual Result

Not Executed.

---

# 6. Localization

## TC-035 — Change Website Language

| Field                | Details                                         |
| -------------------- | ----------------------------------------------- |
| **Test Case ID**     | TC-035                                          |
| **Title**            | Verify website language selection functionality |
| **Related Scenario** | TS-025                                          |
| **Test Type**        | Functional / UI                                 |
| **Priority**         | Medium                                          |
| **Preconditions**    | The application supports multiple languages.    |
| **Test Data**        | Supported alternative language                  |
| **Status**           | Not Executed                                    |

### Test Steps

1. Open the application.
2. Locate the language selector.
3. Select a supported alternative language.
4. Observe the application content.

### Expected Result

The selected language should be applied according to the application's localization functionality.

### Actual Result

Not Executed.

---

## TC-036 — Verify Content in Selected Language

| Field                | Details                                                           |
| -------------------- | ----------------------------------------------------------------- |
| **Test Case ID**     | TC-036                                                            |
| **Title**            | Verify that website content is displayed in the selected language |
| **Related Scenario** | TS-026                                                            |
| **Test Type**        | Functional / UI                                                   |
| **Priority**         | High                                                              |
| **Preconditions**    | A supported alternative language has been selected.               |
| **Test Data**        | Selected supported language                                       |
| **Status**           | Not Executed                                                      |

### Test Steps

1. Change the application language.
2. Navigate through several application pages.
3. Review page titles, navigation labels, buttons, and relevant content.

### Expected Result

Application content should be displayed consistently in the selected language.

### Actual Result

Not Executed.

---

## TC-037 — Verify Language Consistency Across Pages

| Field                | Details                                                                            |
| -------------------- | ---------------------------------------------------------------------------------- |
| **Test Case ID**     | TC-037                                                                             |
| **Title**            | Verify that the selected language remains consistent when navigating between pages |
| **Related Scenario** | TS-026                                                                             |
| **Test Type**        | Functional / UI                                                                    |
| **Priority**         | Medium                                                                             |
| **Preconditions**    | A supported language has been selected.                                            |
| **Test Data**        | Selected alternative language                                                      |
| **Status**           | Not Executed                                                                       |

### Test Steps

1. Select an alternative language.
2. Navigate to the product page.
3. Navigate to the shopping cart.
4. Navigate to checkout.
5. Review the displayed text.

### Expected Result

The selected language should remain consistent across supported application pages.

### Actual Result

Not Executed.

---

# 7. UI and Navigation

## TC-038 — Verify Main Navigation

| Field                | Details                                          |
| -------------------- | ------------------------------------------------ |
| **Test Case ID**     | TC-038                                           |
| **Title**            | Verify navigation between main application pages |
| **Related Scenario** | TS-029                                           |
| **Test Type**        | UI / Functional                                  |
| **Priority**         | Medium                                           |
| **Preconditions**    | The application is accessible.                   |
| **Test Data**        | Main navigation options                          |
| **Status**           | Not Executed                                     |

### Test Steps

1. Open the application.
2. Identify the main navigation options.
3. Click each relevant navigation option.
4. Observe the destination page.

### Expected Result

Each navigation option should direct the user to the correct page without broken links or unexpected behavior.

### Actual Result

Not Executed.

---

## TC-039 — Verify Visibility of Major UI Elements

| Field                | Details                                            |
| -------------------- | -------------------------------------------------- |
| **Test Case ID**     | TC-039                                             |
| **Title**            | Verify visibility of major user interface elements |
| **Related Scenario** | TS-030                                             |
| **Test Type**        | UI                                                 |
| **Priority**         | Medium                                             |
| **Preconditions**    | The application page is loaded successfully.       |
| **Test Data**        | Main application page                              |
| **Status**           | Not Executed                                       |

### Test Steps

1. Open the application.
2. Review the header.
3. Review navigation elements.
4. Review buttons and forms.
5. Review product cards or other major content elements.

### Expected Result

Major UI elements should be visible, properly positioned, readable, and accessible to the user.

### Actual Result

Not Executed.

---

## TC-040 — Verify Interactive UI Elements

| Field                | Details                                        |
| -------------------- | ---------------------------------------------- |
| **Test Case ID**     | TC-040                                         |
| **Title**            | Verify that interactive UI elements are usable |
| **Related Scenario** | TS-031                                         |
| **Test Type**        | UI / Functional                                |
| **Priority**         | Medium                                         |
| **Preconditions**    | The application is loaded successfully.        |
| **Test Data**        | Buttons, links, selectors, and form controls   |
| **Status**           | Not Executed                                   |

### Test Steps

1. Open the application.
2. Identify interactive UI elements.
3. Click relevant buttons and links.
4. Interact with available selectors and form controls.
5. Observe the application response.

### Expected Result

Interactive UI elements should respond correctly to user actions and provide the expected functionality.

### Actual Result

Not Executed.

---

# Test Case Summary

| Category                      | Test Cases |
| ----------------------------- | ---------: |
| Login                         |          7 |
| Product Search                |          6 |
| Product Page & Size Selection |          6 |
| Shopping Cart                 |          7 |
| Checkout                      |          8 |
| Localization                  |          3 |
| UI & Navigation               |          3 |
| **Total**                     |     **40** |

## Test Case Types Covered

* Positive Testing
* Negative Testing
* Functional Testing
* UI Testing
* Validation Testing
* User Flow Testing

## Execution Status

All test cases are currently marked as:

**Not Executed**

Test execution results, actual results, Pass/Fail status, and defect references will be added during the Test Execution phase.
# 8. Additional Authentication and Session Test Cases

## TC-041 — Session Persistence After Page Refresh

| Field            | Details                                                                   |
| ---------------- | ------------------------------------------------------------------------- |
| Test Case ID     | TC-041                                                                    |
| Title            | Verify that an authenticated session behaves correctly after page refresh |
| Related Scenario | TS-011                                                                    |
| Test Type        | Functional / Session                                                      |
| Priority         | High                                                                      |
| Preconditions    | User is successfully logged in                                            |
| Test Data        | Valid authenticated user session                                          |
| Status           | Not Executed                                                              |

### Test Steps

1. Log in with valid credentials.
2. Navigate to an authenticated page.
3. Refresh the browser page.
4. Observe the user's authentication state.

### Expected Result

The application should maintain the expected authentication state after refresh and should not unexpectedly log the user out.

### Actual Result

Not Executed.

---

## TC-042 — Access Protected Page After Logout

| Field            | Details                                                       |
| ---------------- | ------------------------------------------------------------- |
| Test Case ID     | TC-042                                                        |
| Title            | Verify that a logged-out user cannot access protected content |
| Related Scenario | TS-012                                                        |
| Test Type        | Functional / Security-related                                 |
| Priority         | High                                                          |
| Preconditions    | User is logged in and can access a protected page             |
| Test Data        | Previously authenticated session                              |
| Status           | Not Executed                                                  |

### Test Steps

1. Log in successfully.
2. Open an authenticated/protected page.
3. Log out.
4. Use browser Back navigation or directly revisit the protected page.

### Expected Result

The user should not regain access to protected content after logout and should be redirected to an appropriate public/login page if required.

### Actual Result

Not Executed.

---

## TC-043 — Login with Leading and Trailing Spaces

| Field            | Details                                                                   |
| ---------------- | ------------------------------------------------------------------------- |
| Test Case ID     | TC-043                                                                    |
| Title            | Verify login behavior when credentials contain leading or trailing spaces |
| Related Scenario | TS-009                                                                    |
| Test Type        | Negative / Validation                                                     |
| Priority         | Medium                                                                    |
| Preconditions    | Login page is accessible                                                  |
| Test Data        | Valid credential values with leading/trailing spaces                      |
| Status           | Not Executed                                                              |

### Test Steps

1. Open the login page.
2. Enter a valid username/email with leading or trailing spaces.
3. Enter a valid password.
4. Submit the login form.

### Expected Result

The application should handle whitespace consistently according to the defined validation rules and should not create unexpected authentication behavior.

### Actual Result

Not Executed.

---

## TC-044 — Login with Malformed Email

| Field            | Details                                                           |
| ---------------- | ----------------------------------------------------------------- |
| Test Case ID     | TC-044                                                            |
| Title            | Verify validation for malformed email format                      |
| Related Scenario | TS-008                                                            |
| Test Type        | Negative / Validation                                             |
| Priority         | High                                                              |
| Preconditions    | Login page is accessible and email format validation is supported |
| Test Data        | `user@`, `user.com`, `user@@example.com`                          |
| Status           | Not Executed                                                      |

### Test Steps

1. Open the login page.
2. Enter a malformed email address.
3. Enter any password.
4. Submit the form.

### Expected Result

The application should reject the malformed email and display an appropriate validation or authentication message.

### Actual Result

Not Executed.

---

# 9. Additional Product Search Test Cases

## TC-045 — Search Using Whitespace Only

| Field            | Details                                                |
| ---------------- | ------------------------------------------------------ |
| Test Case ID     | TC-045                                                 |
| Title            | Verify search behavior when only whitespace is entered |
| Related Scenario | TS-016                                                 |
| Test Type        | Negative / Validation                                  |
| Priority         | Medium                                                 |
| Preconditions    | Search functionality is available                      |
| Test Data        | Spaces only                                            |
| Status           | Not Executed                                           |

### Test Steps

1. Open the application.
2. Enter only whitespace into the search field.
3. Submit the search.

### Expected Result

The application should handle the input gracefully and should not return unexpected results or an application error.

### Actual Result

Not Executed.

---

## TC-046 — Search Case Sensitivity

| Field            | Details                                              |
| ---------------- | ---------------------------------------------------- |
| Test Case ID     | TC-046                                               |
| Title            | Verify search behavior with different letter casing  |
| Related Scenario | TS-019                                               |
| Test Type        | Functional                                           |
| Priority         | Medium                                               |
| Preconditions    | At least one searchable product exists               |
| Test Data        | Same keyword in lowercase, uppercase, and mixed case |
| Status           | Not Executed                                         |

### Test Steps

1. Search using a lowercase keyword.
2. Record the results.
3. Search using the same keyword in uppercase.
4. Compare the results.

### Expected Result

Search behavior should be consistent with the application's defined case-sensitivity rules.

### Actual Result

Not Executed.

---

## TC-047 — Search Using Special Characters

| Field            | Details                                        |
| ---------------- | ---------------------------------------------- |
| Test Case ID     | TC-047                                         |
| Title            | Verify search behavior with special characters |
| Related Scenario | TS-020                                         |
| Test Type        | Negative / Robustness                          |
| Priority         | Medium                                         |
| Preconditions    | Search functionality is available              |
| Test Data        | `@#$%^&*` and other special characters         |
| Status           | Not Executed                                   |

### Test Steps

1. Open the search field.
2. Enter special characters.
3. Submit the search.
4. Observe the application behavior.

### Expected Result

The application should handle the input safely without UI errors, crashes, or unexpected behavior.

### Actual Result

Not Executed.

---

# 10. Additional Shopping Cart Test Cases

## TC-048 — Minimum Allowed Quantity

| Field            | Details                                     |
| ---------------- | ------------------------------------------- |
| Test Case ID     | TC-048                                      |
| Title            | Verify the minimum allowed product quantity |
| Related Scenario | TS-035                                      |
| Test Type        | Functional / Boundary                       |
| Priority         | High                                        |
| Preconditions    | Product exists in the cart                  |
| Test Data        | Minimum quantity value, normally 1          |
| Status           | Not Executed                                |

### Test Steps

1. Add a product to the cart.
2. Set quantity to the minimum allowed value.
3. Attempt to decrease the quantity below the minimum.

### Expected Result

The application should prevent an invalid quantity below the defined minimum.

### Actual Result

Not Executed.

---

## TC-049 — Maximum Allowed Quantity

| Field            | Details                                                    |
| ---------------- | ---------------------------------------------------------- |
| Test Case ID     | TC-049                                                     |
| Title            | Verify the maximum allowed product quantity                |
| Related Scenario | TS-036                                                     |
| Test Type        | Functional / Boundary                                      |
| Priority         | High                                                       |
| Preconditions    | Product exists in the cart and quantity limits are defined |
| Test Data        | Maximum supported quantity                                 |
| Status           | Not Executed                                               |

### Test Steps

1. Add a product to the cart.
2. Increase the quantity repeatedly.
3. Reach the maximum allowed quantity.
4. Attempt to increase the quantity further.

### Expected Result

The application should prevent the quantity from exceeding the defined maximum.

### Actual Result

Not Executed.

---

## TC-050 — Invalid Quantity Input

| Field            | Details                                                    |
| ---------------- | ---------------------------------------------------------- |
| Test Case ID     | TC-050                                                     |
| Title            | Verify cart behavior with invalid quantity input           |
| Related Scenario | TS-037                                                     |
| Test Type        | Negative / Validation                                      |
| Priority         | High                                                       |
| Preconditions    | Product exists in the cart                                 |
| Test Data        | `0`, negative value, text, decimal value where unsupported |
| Status           | Not Executed                                               |

### Test Steps

1. Open the cart.
2. Attempt to enter an invalid quantity.
3. Confirm or submit the value.

### Expected Result

The application should reject invalid quantity values and preserve a valid cart state.

### Actual Result

Not Executed.

---

## TC-051 — Total Calculation for Multiple Products

| Field            | Details                                                         |
| ---------------- | --------------------------------------------------------------- |
| Test Case ID     | TC-051                                                          |
| Title            | Verify total calculation when multiple products are in the cart |
| Related Scenario | TS-039                                                          |
| Test Type        | Functional / Calculation                                        |
| Priority         | High                                                            |
| Preconditions    | At least two products can be added to the cart                  |
| Test Data        | Product A + Product B with known prices and quantities          |
| Status           | Not Executed                                                    |

### Test Steps

1. Add Product A to the cart.
2. Add Product B to the cart.
3. Record prices and quantities.
4. Calculate the expected total manually.
5. Compare it with the displayed total.

### Expected Result

The displayed cart total should equal the sum of all applicable product line totals.

### Actual Result

Not Executed.

---

## TC-052 — Cart Total Recalculation After Quantity Update

| Field            | Details                                                                   |
| ---------------- | ------------------------------------------------------------------------- |
| Test Case ID     | TC-052                                                                    |
| Title            | Verify that cart total is recalculated immediately after quantity changes |
| Related Scenario | TS-040                                                                    |
| Test Type        | Functional / Calculation / Regression                                     |
| Priority         | Critical                                                                  |
| Preconditions    | Cart contains a product with a known price                                |
| Test Data        | Example: Product price = 50, quantity changed from 1 to 2                 |
| Status           | Not Executed                                                              |

### Test Steps

1. Add a product to the cart.
2. Record the initial price and total.
3. Increase the quantity.
4. Observe the updated total.
5. Decrease the quantity.
6. Observe the total again.

### Expected Result

The cart total should be recalculated correctly after every quantity change.

### Actual Result

Not Executed.

### Defect Reference

Potential regression coverage for **BUG-002 — Cart total price does not change when product quantity is updated**.

---

## TC-053 — Cart State After Page Refresh

| Field            | Details                                 |
| ---------------- | --------------------------------------- |
| Test Case ID     | TC-053                                  |
| Title            | Verify cart state after browser refresh |
| Related Scenario | TS-044                                  |
| Test Type        | Functional / Session                    |
| Priority         | High                                    |
| Preconditions    | Product has been added to the cart      |
| Test Data        | Product with selected size and quantity |
| Status           | Not Executed                            |

### Test Steps

1. Add a product to the cart.
2. Record product, size, quantity, and total.
3. Refresh the browser.
4. Open the cart again.

### Expected Result

The cart should behave according to the application's defined persistence rules and should not lose or corrupt cart data unexpectedly.

### Actual Result

Not Executed.

---

# 11. Additional Checkout Test Cases

## TC-054 — Invalid Checkout Email

| Field            | Details                          |
| ---------------- | -------------------------------- |
| Test Case ID     | TC-054                           |
| Title            | Verify checkout email validation |
| Related Scenario | TS-050                           |
| Test Type        | Negative / Validation            |
| Priority         | High                             |
| Preconditions    | User has reached checkout        |
| Test Data        | Invalid email formats            |
| Status           | Not Executed                     |

### Test Steps

1. Open checkout.
2. Enter an invalid email address.
3. Fill other required fields with valid data.
4. Submit the order.

### Expected Result

The application should reject the invalid email and prevent order submission until the value is corrected.

### Actual Result

Not Executed.

---

## TC-055 — Invalid Checkout Phone Number

| Field            | Details                                 |
| ---------------- | --------------------------------------- |
| Test Case ID     | TC-055                                  |
| Title            | Verify checkout phone number validation |
| Related Scenario | TS-051                                  |
| Test Type        | Negative / Validation                   |
| Priority         | Medium                                  |
| Preconditions    | Checkout page is accessible             |
| Test Data        | Invalid phone number format             |
| Status           | Not Executed                            |

### Test Steps

1. Open checkout.
2. Enter an invalid phone number.
3. Complete the remaining required fields.
4. Attempt to submit the order.

### Expected Result

The application should reject invalid phone input and display an appropriate validation message.

### Actual Result

Not Executed.

---

## TC-056 — Prevent Order Submission with Incomplete Information

| Field            | Details                                                     |
| ---------------- | ----------------------------------------------------------- |
| Test Case ID     | TC-056                                                      |
| Title            | Verify that an incomplete checkout form cannot be submitted |
| Related Scenario | TS-059                                                      |
| Test Type        | Negative / Validation                                       |
| Priority         | Critical                                                    |
| Preconditions    | Cart contains at least one product                          |
| Test Data        | One or more required checkout fields left empty             |
| Status           | Not Executed                                                |

### Test Steps

1. Proceed to checkout.
2. Leave at least one required field empty.
3. Fill the remaining required fields.
4. Attempt to place the order.

### Expected Result

The order should not be submitted and the missing required information should be clearly identified.

### Actual Result

Not Executed.

---

## TC-057 — Prevent Duplicate Order Submission

| Field            | Details                                                                |
| ---------------- | ---------------------------------------------------------------------- |
| Test Case ID     | TC-057                                                                 |
| Title            | Verify that repeated order submission does not create duplicate orders |
| Related Scenario | TS-060                                                                 |
| Test Type        | Negative / Functional                                                  |
| Priority         | High                                                                   |
| Preconditions    | Checkout form is completed with valid information                      |
| Test Data        | Valid checkout data                                                    |
| Status           | Not Executed                                                           |

### Test Steps

1. Complete the checkout form.
2. Click the final order submission button.
3. Attempt to click the button repeatedly or submit again if the UI allows it.
4. Review the resulting order state.

### Expected Result

Only one order should be created for a single user action. The application should prevent duplicate submissions.

### Actual Result

Not Executed.

---

## TC-058 — Checkout Total Matches Cart Total

| Field            | Details                                                 |
| ---------------- | ------------------------------------------------------- |
| Test Case ID     | TC-058                                                  |
| Title            | Verify that checkout total matches the final cart total |
| Related Scenario | TS-058                                                  |
| Test Type        | Functional / Calculation                                |
| Priority         | Critical                                                |
| Preconditions    | Cart contains one or more products                      |
| Test Data        | Known product prices and quantities                     |
| Status           | Not Executed                                            |

### Test Steps

1. Open the shopping cart.
2. Record the final cart total.
3. Proceed to checkout.
4. Compare the checkout total with the cart total.

### Expected Result

The checkout total should match the applicable final cart total, including any defined shipping or additional charges.

### Actual Result

Not Executed.

---

# 12. Additional Localization Test Cases

## TC-059 — Localization of Validation Messages

| Field            | Details                                                                |
| ---------------- | ---------------------------------------------------------------------- |
| Test Case ID     | TC-059                                                                 |
| Title            | Verify that validation and error messages follow the selected language |
| Related Scenario | TS-065                                                                 |
| Test Type        | Functional / Localization                                              |
| Priority         | Medium                                                                 |
| Preconditions    | Application supports multiple languages                                |
| Test Data        | Non-default application language                                       |
| Status           | Not Executed                                                           |

### Test Steps

1. Change the application language.
2. Navigate to a form with validation.
3. Trigger a validation error.
4. Review the displayed message.

### Expected Result

Validation and error messages should appear in the selected language.

### Actual Result

Not Executed.

### Defect Reference

Additional regression coverage for **BUG-001 — Website content remains in English after changing language**.

---

## TC-060 — No Mixed-Language Content

| Field            | Details                                                                      |
| ---------------- | ---------------------------------------------------------------------------- |
| Test Case ID     | TC-060                                                                       |
| Title            | Verify that the interface does not contain unexpected mixed-language content |
| Related Scenario | TS-068                                                                       |
| Test Type        | Functional / Localization / UI                                               |
| Priority         | Medium                                                                       |
| Preconditions    | A non-default language is selected                                           |
| Test Data        | Supported non-default language                                               |
| Status           | Not Executed                                                                 |

### Test Steps

1. Select a supported non-default language.
2. Navigate through the main user journey.
3. Review navigation labels, buttons, product information, validation messages, and checkout content.

### Expected Result

User-facing content should consistently use the selected language. Unexpected untranslated English or other-language text should not appear.

### Actual Result

Not Executed.

