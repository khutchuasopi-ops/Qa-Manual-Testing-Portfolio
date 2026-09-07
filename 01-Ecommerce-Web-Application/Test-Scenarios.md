# Test Scenarios — E-commerce Web Application

## 1. Login and Authentication

### TS-001 — User Login

Verify that a user can log in with valid credentials.

### TS-002 — Login with Valid and Invalid Credentials

Verify login behavior with valid and invalid credentials.

### TS-003 — Required Login Fields

Verify validation when required login fields are empty.

### TS-004 — User Logout

Verify that a logged-in user can log out successfully.

---

## 2. Product Search

### TS-005 — Product Search

Verify that users can search for products.

### TS-006 — Valid and Invalid Search Keywords

Verify search behavior with valid, invalid, and partial keywords.

### TS-007 — Empty Search

Verify the application behavior when search is submitted without a keyword.

### TS-008 — Search Result Relevance

Verify that search results are relevant to the entered keyword.

---

## 3. Product Details and Selection

### TS-009 — Product Information

Verify that product information is displayed correctly.

### TS-010 — Product Size Selection

Verify that an available product size can be selected.

### TS-011 — Unavailable Product Size

Verify that an unavailable size cannot be selected incorrectly.

### TS-012 — Selected Size Retention

Verify that the selected product size remains selected when expected.

---

## 4. Shopping Cart

### TS-013 — Add Product to Cart

Verify that a selected product can be added to the shopping cart.

### TS-014 — Cart Product Information

Verify that product information is displayed correctly in the cart.

### TS-015 — Change Product Quantity

Verify that product quantity can be increased and decreased.

### TS-016 — Cart Total Calculation

Verify that the cart total is calculated correctly.

### TS-017 — Remove Product from Cart

Verify that a product can be removed from the cart.

### TS-018 — Empty Shopping Cart

Verify that the empty cart state is displayed correctly.

---

## 5. Checkout

### TS-019 — Navigate from Cart to Checkout

Verify that the user can proceed from the shopping cart to checkout.

### TS-020 — Checkout Information and Validation

Verify checkout information fields and their basic validation.

### TS-021 — Delivery Information

Verify that delivery information can be entered and validated.

### TS-022 — Payment Information

Verify that payment information fields are available and handled correctly.

### TS-023 — Order Summary and Total

Verify that the order summary displays the correct product, quantity, price, and total information.

### TS-024 — Successful Order Flow

Verify that a user can complete the order flow with valid information.

### TS-025 — Missing Required Checkout Information

Verify that required checkout fields are validated when information is missing.

### TS-026 — Invalid Checkout Input

Verify checkout behavior when invalid information is entered.

---

## 6. Localization

### TS-027 — Language Selection

Verify that the user can select another available language.

### TS-028 — Selected Language Content

Verify that visible application content changes according to the selected language.

---

## 7. UI and Navigation

### TS-029 — Main Navigation

Verify that the main navigation and important links work correctly.

### TS-030 — UI Element Visibility

Verify that important UI elements are visible and understandable.

### TS-031 — Interactive UI Elements

Verify that buttons, links, and other interactive elements can be used as expected.

---

## 8. Product Quantity

### TS-032 — Product Quantity Selection

Verify that the user can select or enter a valid product quantity.

### TS-033 — Increase and Decrease Quantity

Verify that product quantity can be increased and decreased correctly.

### TS-034 — Quantity Limits and Invalid Quantity

Verify that invalid quantities and quantity limits are handled correctly.

---

## Scenario Summary

| Area                          | Scenarios |
| ----------------------------- | --------: |
| Login and Authentication      |         4 |
| Product Search                |         4 |
| Product Details and Selection |         4 |
| Shopping Cart                 |         6 |
| Checkout                      |         8 |
| Localization                  |         2 |
| UI and Navigation             |         3 |
| Product Quantity              |         3 |
| **Total**                     |    **34** |

---

## Notes

These scenarios describe the documented functional coverage of the project.

They represent test scenarios and should not be interpreted as proof that every scenario was executed.

Historical execution results are documented separately in the `Test-Execution` folder.
