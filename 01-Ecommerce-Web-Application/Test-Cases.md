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
