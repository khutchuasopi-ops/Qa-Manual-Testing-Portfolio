# E-commerce Web Application — QA Case Study

## 1. Project Overview

This case study describes a manual QA testing project performed on a web-based e-commerce application.

The main goal was to practice and demonstrate a structured manual testing process from test planning and test case design to test execution, defect reporting, and test summary.

**Testing Role:** Junior Manual QA Tester
**Testing Type:** Manual Testing
**Application Type:** E-commerce Web Application

---

# 2. Testing Objective

The main objectives of the testing activity were to:

* Verify the core e-commerce user journey.
* Check whether the main features behave as expected.
* Identify functional and UI-related issues.
* Validate positive and negative scenarios.
* Practice writing clear and reproducible test cases.
* Document discovered defects professionally.
* Understand the relationship between test cases, execution results, and bug reports.

---

# 3. Application Scope

The testing focused on the following areas:

* User Login
* Logout
* Product Search
* Product Details
* Product Size Selection
* Product Quantity
* Shopping Cart
* Cart Price Calculation
* Checkout
* Localization
* UI and Navigation

The main customer journey was tested as:

```text
Login
  ↓
Search Product
  ↓
Open Product
  ↓
Select Size / Quantity
  ↓
Add to Cart
  ↓
Review Cart
  ↓
Checkout
```

---

# 4. Test Approach

As a Junior Manual QA Tester, I used a structured but practical testing approach.

The main testing activities included:

### Functional Testing

I verified whether application features behaved according to their expected functionality.

Examples:

* Login with valid credentials
* Login with invalid credentials
* Product search
* Adding products to the cart
* Changing product quantity
* Checkout navigation

### Positive Testing

I used valid input and expected user behavior to verify successful flows.

Examples:

* Valid login
* Valid product search
* Selecting an available product size
* Adding a valid product to the cart

### Negative Testing

I intentionally used invalid or incomplete input to verify application validation.

Examples:

* Invalid credentials
* Empty required fields
* Invalid email format
* Invalid quantity
* Incomplete checkout information

### Boundary Testing

I considered minimum and maximum values where applicable.

Examples:

* Minimum product quantity
* Maximum product quantity
* Quantity changes in the cart

### UI Testing

I checked basic visual and usability aspects such as:

* Element visibility
* Button availability
* Navigation
* Text readability
* Product information
* Layout consistency

### Localization Testing

I checked whether the application content changed correctly when a different language was selected.

---

# 5. Test Design

Test scenarios and test cases were created before execution.

The test suite included coverage for:

* Authentication
* Search
* Product selection
* Shopping cart
* Checkout
* Localization
* UI
* Negative and edge cases

The test cases contain:

* Test Case ID
* Title
* Related Scenario
* Test Type
* Priority
* Preconditions
* Test Data
* Steps
* Expected Result
* Actual Result
* Status

This structure was used to make the test execution easier to understand and trace.

---

# 6. Test Execution

The initial execution contained 40 historical test cases.

The recorded results were:

| Result       | Count |
| ------------ | ----: |
| PASS         |     2 |
| FAIL         |     3 |
| BLOCKED      |     0 |
| NOT RECORDED |    35 |

During the test execution, three functional issues were identified.

The test execution report was later expanded to include additional test cases covering validation, boundaries, session behavior, cart calculations, checkout, and localization regression.

The newly added test cases are currently marked as `NOT EXECUTED` until they are actually tested.

---

# 7. Defects Identified

## BUG-001 — Localization Issue

### Area

Localization

### Problem

After changing the application language, some website content remained in English.

### Expected Result

The user-facing content should be displayed in the selected language.

### Actual Result

The content remained in English after another language was selected.

### Severity

Medium

### Priority

Medium

### QA Observation

This issue can negatively affect users who rely on the selected language and creates an inconsistent user experience.

---

## BUG-002 — Cart Total Calculation

### Area

Shopping Cart

### Problem

The cart total did not update correctly after changing the product quantity.

### Expected Result

The cart total should be recalculated after every quantity change.

### Actual Result

The displayed total did not update correctly.

### Severity

High

### Priority

High

### QA Observation

This is an important e-commerce defect because incorrect pricing can directly affect the customer order.

---

## BUG-003 — Invalid Email Accepted During Login

### Area

Authentication

### Problem

An invalid email credential was accepted during the login flow.

### Expected Result

Invalid credentials should be rejected and the user should remain unauthenticated.

### Actual Result

The invalid email credentials were accepted and the user was redirected to the home page.

### Severity

Medium

### Priority

High

### QA Observation

Authentication validation should be investigated because unexpected acceptance of invalid credentials may affect the reliability of the login flow.

---

# 8. Defect Prioritization

The defects were prioritized based on their potential impact on the user journey.

| Bug     | Area           | Severity | Priority |
| ------- | -------------- | -------- | -------- |
| BUG-002 | Shopping Cart  | High     | High     |
| BUG-003 | Authentication | Medium   | High     |
| BUG-001 | Localization   | Medium   | Medium   |

The cart calculation issue was considered the highest priority because pricing accuracy is directly related to the purchase process.

---

# 9. QA Traceability

The defects were connected to the test cases that identified them.

```text
TC-002
  ↓
BUG-003
  ↓
Retest
  ↓
Regression Testing
```

```text
TC-024
  ↓
BUG-002
  ↓
Retest
  ↓
Regression Testing
```

```text
TC-036
  ↓
BUG-001
  ↓
Retest
  ↓
Regression Testing
```

This provides basic traceability between testing and defect management.

---

# 10. Testing Challenges

During this project, several challenges were identified.

### Incomplete Historical Execution Data

Not all original test execution results were available.

Instead of assuming that unrecorded tests had passed, they were marked as:

`NOT RECORDED`

This approach keeps the portfolio honest and avoids presenting unsupported test results.

### Expanding Test Coverage

The initial test suite covered the main functionality but needed additional edge cases.

Additional coverage was therefore added for:

* Session behavior
* Invalid input
* Quantity boundaries
* Cart state
* Checkout validation
* Duplicate submission
* Localization regression

---

# 11. What I Learned

This project helped me understand the practical relationship between different QA activities.

I learned that writing test cases is not enough. A complete QA process also requires:

* Clear test scenarios
* Structured test cases
* Actual test execution
* Accurate result recording
* Reproducible bug reports
* Retesting
* Regression testing
* Final test reporting

I also learned the importance of testing beyond the happy path.

For example, a basic cart test may confirm that a product can be added successfully, but additional testing should also verify:

* Quantity changes
* Minimum and maximum quantity
* Invalid quantity
* Price recalculation
* Multiple products
* Cart state after refresh

---

# 12. Junior QA Perspective

As a Junior Manual QA Tester, my focus in this project was on building strong fundamentals:

* Understanding requirements
* Designing meaningful test scenarios
* Writing clear test cases
* Performing manual functional testing
* Identifying defects
* Writing reproducible bug reports
* Understanding severity and priority
* Performing basic regression planning
* Communicating test results clearly

This project represents my practical QA learning and portfolio work rather than claiming production-level experience in advanced testing areas.

---

# 13. Improvement Opportunities

For a future testing cycle, I would improve the project by:

1. Executing the complete expanded test suite.
2. Recording actual results for every executed test.
3. Adding screenshots or other evidence for confirmed defects.
4. Performing retesting after defect fixes.
5. Performing regression testing around fixed functionality.
6. Expanding browser coverage.
7. Performing responsive testing on different viewport sizes.
8. Improving test data coverage.
9. Adding API testing as a separate learning exercise.
10. Gradually introducing automation after strengthening manual testing fundamentals.

---

# 14. Final QA Assessment

Based on the currently recorded results, further testing is required.

The test execution identified issues in:

* Authentication
* Shopping Cart
* Localization

The project demonstrates a complete basic manual QA workflow:

```text
Test Planning
      ↓
Scenario Design
      ↓
Test Case Design
      ↓
Test Execution
      ↓
Defect Reporting
      ↓
Retesting
      ↓
Regression Testing
      ↓
Test Summary
```

The main outcome of this project was not only identifying defects, but also developing a structured approach to manual software testing.

---

# 15. Portfolio Value

This project demonstrates my ability to:

* Create structured manual test documentation.
* Think about positive and negative scenarios.
* Test core e-commerce user journeys.
* Identify functional issues.
* Document defects clearly.
* Connect defects to test cases.
* Understand basic severity and priority concepts.
* Report incomplete testing honestly.
* Plan retesting and regression coverage.

It also demonstrates my current development as a **Junior Manual QA Tester** and provides a foundation for more advanced QA practices in future projects.
