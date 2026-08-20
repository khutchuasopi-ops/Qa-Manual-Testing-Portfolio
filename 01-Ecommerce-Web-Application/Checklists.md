# Checklists

Functional testing checklists for the main areas of the e-commerce web application.

## 1. Login Checklist

| ID | Checklist Item | Status |
|---|---|---|
| LC-001 | Verify that the Login page opens successfully | Not Checked |
| LC-002 | Verify that the email/username field is displayed | Not Checked |
| LC-003 | Verify that the password field is displayed | Not Checked |
| LC-004 | Verify that the password is masked | Not Checked |
| LC-005 | Verify login with valid credentials | Not Checked |
| LC-006 | Verify login with an incorrect password | Not Checked |
| LC-007 | Verify login with an unregistered email | Not Checked |
| LC-008 | Verify validation for an empty email field | Not Checked |
| LC-009 | Verify validation for an empty password field | Not Checked |
| LC-010 | Verify validation when both fields are empty | Not Checked |
| LC-011 | Verify Forgot Password functionality | Not Checked |
| LC-012 | Verify that the user can log out successfully | Not Checked |

---

## 2. Search Checklist

| ID | Checklist Item | Status |
|---|---|---|
| SC-001 | Verify that the search field is displayed | Not Checked |
| SC-002 | Verify search with a valid product name | Not Checked |
| SC-003 | Verify search with a partial product name | Not Checked |
| SC-004 | Verify search with a non-existing product name | Not Checked |
| SC-005 | Verify search with an empty search field | Not Checked |
| SC-006 | Verify search using uppercase letters | Not Checked |
| SC-007 | Verify search using lowercase letters | Not Checked |
| SC-008 | Verify search with leading/trailing spaces | Not Checked |
| SC-009 | Verify that search results are relevant to the entered keyword | Not Checked |
| SC-010 | Verify that product names in search results are displayed correctly | Not Checked |
| SC-011 | Verify that product images in search results are displayed correctly | Not Checked |
| SC-012 | Verify that product prices in search results are displayed correctly | Not Checked |
| SC-013 | Verify that a product can be opened from the search results | Not Checked |
| SC-014 | Verify that the search field can be cleared | Not Checked |

---

## 3. Product & Size Checklist

| ID | Checklist Item | Status |
|---|---|---|
| PS-001 | Verify that the product page opens successfully | Not Checked |
| PS-002 | Verify that the product name is displayed correctly | Not Checked |
| PS-003 | Verify that the product image is displayed correctly | Not Checked |
| PS-004 | Verify that the product price is displayed correctly | Not Checked |
| PS-005 | Verify that available product sizes are displayed | Not Checked |
| PS-006 | Verify that the size selection control is displayed correctly | Not Checked |
| PS-007 | Verify that the user can select an available size | Not Checked |
| PS-008 | Verify that the selected size is clearly indicated | Passed |
| PS-009 | Verify that the selected size remains selected before adding the product to the cart | Not Checked |
| PS-010 | Verify that an unavailable size is clearly indicated | Not Checked |
| PS-011 | Verify that an unavailable size cannot be selected | Not Checked |
| PS-012 | Verify that the user cannot add a product without selecting a required size | Not Checked |
| PS-013 | Verify that the selected size is retained after adding the product to the cart | Passed |
| PS-014 | Verify that the correct product size is displayed in the shopping cart | Not Checked |

---

## 4. Shopping Cart Checklist

| ID | Checklist Item | Status |
|---|---|---|
| CC-001 | Verify that the shopping cart can be opened | Not Checked |
| CC-002 | Verify that an added product is displayed in the shopping cart | Not Checked |
| CC-003 | Verify that the correct product name is displayed | Not Checked |
| CC-004 | Verify that the correct product image is displayed | Not Checked |
| CC-005 | Verify that the selected product size is displayed correctly | Not Checked |
| CC-006 | Verify that the correct product price is displayed | Not Checked |
| CC-007 | Verify that the selected product quantity is displayed correctly | Not Checked |
| CC-008 | Verify that the product quantity can be increased | Not Checked |
| CC-009 | Verify that the product quantity can be decreased | Not Checked |
| CC-010 | Verify that the cart total is updated after changing the quantity | Not Checked |
| CC-011 | Verify that a product can be removed from the shopping cart | Not Checked |
| CC-012 | Verify that the cart total is updated after removing a product | Not Checked |
| CC-013 | Verify that multiple products can be added to the shopping cart | Not Checked |
| CC-014 | Verify that the cart total is calculated correctly for multiple products | Not Checked |
| CC-015 | Verify the behavior of an empty shopping cart | Not Checked |
| CC-016 | Verify that the user can continue shopping from the cart | Not Checked |
| CC-017 | Verify that the user can proceed to checkout from the cart | Not Checked |

---

## 5. Checkout Checklist

| ID | Checklist Item | Status |
|---|---|---|
| CO-001 | Verify that the user can access the checkout page from the shopping cart | Not Checked |
| CO-002 | Verify that the checkout page loads successfully | Not Checked |
| CO-003 | Verify that the selected product is displayed correctly during checkout | Not Checked |
| CO-004 | Verify that the selected product size is displayed correctly during checkout | Not Checked |
| CO-005 | Verify that the product quantity is displayed correctly | Not Checked |
| CO-006 | Verify that the product price is displayed correctly | Not Checked |
| CO-007 | Verify that the order subtotal is calculated correctly | Not Checked |
| CO-008 | Verify that the total order amount is calculated correctly | Not Checked |
| CO-009 | Verify that required customer information fields are displayed | Not Checked |
| CO-010 | Verify validation for empty required customer information fields | Not Checked |
| CO-011 | Verify that valid customer information can be entered | Not Checked |
| CO-012 | Verify that invalid customer information is rejected with appropriate validation | Not Checked |
| CO-013 | Verify that available delivery/shipping options are displayed | Not Checked |
| CO-014 | Verify that the user can select a delivery/shipping option | Not Checked |
| CO-015 | Verify that the delivery/shipping cost is calculated correctly | Not Checked |
| CO-016 | Verify that the final order total is updated after selecting delivery/shipping | Not Checked |
| CO-017 | Verify that available payment methods are displayed | Not Checked |
| CO-018 | Verify that the user can select a payment method | Not Checked |
| CO-019 | Verify that the order summary contains correct product, quantity, price, and total information | Not Checked |
| CO-020 | Verify that the user can complete the order with valid information | Not Checked |
| CO-021 | Verify that an appropriate validation/error message is displayed when required checkout information is invalid | Not Checked |
| CO-022 | Verify that the order confirmation is displayed after successful order placement | Not Checked |
