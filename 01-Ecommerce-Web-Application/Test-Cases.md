# Test Cases

Manual test cases created for the e-commerce web application.

## Test Case Structure

Each test case contains:

- Test Case ID
- Title
- Priority
- Preconditions
- Test Data
- Test Steps
- Expected Result
- Status

## Login

### TC-001 — Verify login with valid credentials

**Priority:** High

**Preconditions:**  
User has a registered account and is on the Login page.

**Test Data:**  
Valid email and password.

**Test Steps:**
1. Enter a valid email.
2. Enter a valid password.
3. Click **Login**.

**Expected Result:**  
User is successfully logged in and redirected to the appropriate page.

**Status:** Not Executed

### TC-002 — Verify login with an incorrect password

**Priority:** High

**Preconditions:**  
User has a registered account and is on the Login page.

**Test Data:**  
Valid email and incorrect password.

**Test Steps:**
1. Enter a valid email.
2. Enter an incorrect password.
3. Click **Login**.

**Expected Result:**  
An appropriate error message is displayed and the user is not logged in.

**Status:** Not Executed
### TC-003 — Verify login with empty required fields

**Priority:** High

**Preconditions:**  
User is on the Login page.

**Test Data:**  
Empty email and password fields.

**Test Steps:**

1. Leave the email field empty.
2. Leave the password field empty.
3. Click **Login**.

**Expected Result:**  
Validation messages are displayed for the required fields.

**Status:** Not Executed

### TC-004 — Verify product search with a valid keyword

**Priority:** High

**Preconditions:**  
User is on the homepage.

**Test Data:**  
Search keyword: "dress".

**Test Steps:**

1. Open the website.
2. Enter "dress" in the search field.
3. Click the search icon/button.

**Expected Result:**  
Relevant products matching the search keyword are displayed.

**Status:** Not Executed

### TC-005 — Verify product search with a non-existing keyword

**Priority:** Medium

**Preconditions:**  
User is on the homepage.

**Test Data:**  
Search keyword: "xyz123".

**Test Steps:**

1. Enter "xyz123" in the search field.
2. Start the search.

**Expected Result:**  
A clear message indicating that no results were found is displayed.

**Status:** Not Executed

### TC-006 — Verify product search with an empty field

**Priority:** Medium

**Preconditions:**  
User is on the homepage.

**Test Data:**  
Empty search field.

**Test Steps:**

1. Leave the search field empty.
2. Click the search icon/button.

**Expected Result:**  
The system handles the empty search appropriately and does not produce an error.

**Status:** Not Executed

### TC-007 — Verify that the user can select a product size

**Priority:** High

**Preconditions:**  
User is logged in and a product with available sizes is displayed.

**Test Data:**  
Product: T-shirt; Size: M.

**Test Steps:**

1. Open the website.
2. Select a product, e.g. a T-shirt.
3. Open the size dropdown.
4. Select size M.

**Expected Result:**  
Size M is successfully selected and displayed on the product page.

**Status:** Passed

### TC-008 — Verify that the selected product size is retained after adding the product to the cart

**Priority:** High

**Preconditions:**  
User is logged in and a product with available sizes is displayed.

**Test Data:**  
Product: T-shirt; Size: M.

**Test Steps:**

1. Select a product.
2. Select size M.
3. Click **Add to Cart**.
4. Open the shopping cart.

**Expected Result:**  
The product is added to the cart and size M is correctly displayed.

**Status:** Passed

### TC-009 — Verify that a product can be added to the shopping cart

**Priority:** High

**Preconditions:**  
User is on a product page and the product is available.

**Test Data:**  
Product: T-shirt.

**Test Steps:**

1. Open a product page.
2. Select a required size.
3. Click **Add to Cart**.
4. Open the cart.

**Expected Result:**  
The selected product is successfully added to the cart.

**Status:** Not Executed

### TC-010 — Verify that the cart displays correct product information

**Priority:** High

**Preconditions:**  
A product has been added to the cart.

**Test Data:**  
Product: T-shirt; Size: M.

**Test Steps:**

1. Add a product to the cart.
2. Open the shopping cart.

**Expected Result:**  
Product name, selected size, quantity, and price are displayed correctly.

**Status:** Not Executed

### TC-011 — Verify that a product can be removed from the cart

**Priority:** High

**Preconditions:**  
The shopping cart contains at least one product.

**Test Data:**  
Product: T-shirt.

**Test Steps:**

1. Open the shopping cart.
2. Click **Remove** for the selected product.

**Expected Result:**  
The product is removed from the cart.

**Status:** Not Executed

### TC-012 — Verify that the cart total is calculated correctly

**Priority:** High

**Preconditions:**  
The shopping cart contains at least one product.

**Test Data:**  
Product price and quantity.

**Test Steps:**

1. Add a product to the cart.
2. Open the cart.
3. Check the displayed total.

**Expected Result:**  
The cart total is calculated correctly based on product price and quantity.

**Status:** Not Executed

### TC-013 — Verify that product details are displayed correctly

**Priority:** High

**Preconditions:**  
User is on a product page.

**Test Data:**  
Available product.

**Test Steps:**

1. Open a product page.
2. Review the product information.

**Expected Result:**  
Product name, image, price, available sizes, and other relevant information are displayed correctly.

**Status:** Not Executed

### TC-014 — Verify that an unavailable product size cannot be selected

**Priority:** High

**Preconditions:**  
User is on a product page with at least one unavailable size.

**Test Data:**  
Product with an unavailable size.

**Test Steps:**

1. Open a product page.
2. Open the size selection.
3. Try to select an unavailable size.

**Expected Result:**  
The unavailable size cannot be selected or is clearly marked as unavailable.

**Status:** Not Executed

### TC-015 — Verify that the user can proceed to checkout

**Priority:** High

**Preconditions:**  
User has a product in the shopping cart.

**Test Data:**  
Product: T-shirt.

**Test Steps:**

1. Add a product to the cart.
2. Open the cart.
3. Click **Checkout**.

**Expected Result:**  
User is successfully redirected to the checkout process.

**Status:** Not Executed
