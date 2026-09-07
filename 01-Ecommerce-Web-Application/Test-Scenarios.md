# Test Scenarios

High-level test scenarios for the E-commerce Web Application.

These scenarios define the main functional, validation, negative, boundary, usability, and user-flow areas to be tested before detailed test cases are created.

---

## 1. Authentication and Login

| Scenario ID | Test Scenario                                      | Priority |
| ----------- | -------------------------------------------------- | -------- |
| TS-001      | Verify user login with valid credentials           | High     |
| TS-002      | Verify login with invalid username/email           | High     |
| TS-003      | Verify login with invalid password                 | High     |
| TS-004      | Verify login with both invalid credentials         | High     |
| TS-005      | Verify validation when username/email is empty     | High     |
| TS-006      | Verify validation when password is empty           | High     |
| TS-007      | Verify validation when both login fields are empty | High     |
| TS-008      | Verify login behavior with malformed email format  | Medium   |
| TS-009      | Verify login behavior with leading/trailing spaces | Medium   |
| TS-010      | Verify logout functionality                        | High     |
| TS-011      | Verify authenticated session after page refresh    | Medium   |
| TS-012      | Verify protected page access after logout          | High     |

---

## 2. Product Search

| Scenario ID | Test Scenario                                                 | Priority |
| ----------- | ------------------------------------------------------------- | -------- |
| TS-013      | Verify product search with a valid keyword                    | High     |
| TS-014      | Verify search with an invalid/non-existing keyword            | High     |
| TS-015      | Verify search behavior with an empty search field             | Medium   |
| TS-016      | Verify search behavior with whitespace-only input             | Medium   |
| TS-017      | Verify search result relevance to the entered keyword         | High     |
| TS-018      | Verify search behavior with partial product name              | Medium   |
| TS-019      | Verify search behavior with different letter cases            | Low      |
| TS-020      | Verify search behavior with special characters                | Low      |
| TS-021      | Verify search result behavior when no matching products exist | High     |

---

## 3. Product Details and Selection

| Scenario ID | Test Scenario                                                               | Priority |
| ----------- | --------------------------------------------------------------------------- | -------- |
| TS-022      | Verify product details displayed correctly                                  | High     |
| TS-023      | Verify product name, price, image, and availability                         | High     |
| TS-024      | Verify product size selection                                               | High     |
| TS-025      | Verify unavailable product sizes cannot be selected                         | High     |
| TS-026      | Verify required size selection before adding a product to cart              | High     |
| TS-027      | Verify selected product size is retained when adding the product to cart    | High     |
| TS-028      | Verify product information remains consistent between product page and cart | High     |

---

## 4. Shopping Cart

| Scenario ID | Test Scenario                                             | Priority |
| ----------- | --------------------------------------------------------- | -------- |
| TS-029      | Verify adding a product to the shopping cart              | High     |
| TS-030      | Verify product information displayed in the shopping cart | High     |
| TS-031      | Verify selected size is displayed correctly in the cart   | High     |
| TS-032      | Verify changing product quantity in the shopping cart     | High     |
| TS-033      | Verify increasing product quantity                        | High     |
| TS-034      | Verify decreasing product quantity                        | High     |
| TS-035      | Verify minimum allowed quantity                           | High     |
| TS-036      | Verify maximum allowed quantity                           | High     |
| TS-037      | Verify behavior with invalid quantity values              | High     |
| TS-038      | Verify cart total calculation for a single product        | High     |
| TS-039      | Verify cart total calculation for multiple products       | High     |
| TS-040      | Verify cart total recalculation after quantity changes    | Critical |
| TS-041      | Verify removing a product from the shopping cart          | High     |
| TS-042      | Verify removing the last product from the cart            | Medium   |
| TS-043      | Verify empty shopping cart behavior                       | Medium   |
| TS-044      | Verify cart contents after page refresh                   | Medium   |

---

## 5. Checkout

| Scenario ID | Test Scenario                                                        | Priority |
| ----------- | -------------------------------------------------------------------- | -------- |
| TS-045      | Verify navigation from shopping cart to checkout                     | High     |
| TS-046      | Verify checkout information fields are displayed                     | High     |
| TS-047      | Verify required checkout field validation                            | High     |
| TS-048      | Verify checkout behavior with missing required information           | High     |
| TS-049      | Verify checkout behavior with invalid input data                     | High     |
| TS-050      | Verify validation of email address                                   | High     |
| TS-051      | Verify validation of phone number                                    | Medium   |
| TS-052      | Verify validation of address information                             | Medium   |
| TS-053      | Verify available delivery/shipping options                           | High     |
| TS-054      | Verify delivery/shipping information selection                       | High     |
| TS-055      | Verify available payment methods                                     | High     |
| TS-056      | Verify order summary information                                     | High     |
| TS-057      | Verify checkout total matches shopping cart total                    | Critical |
| TS-058      | Verify successful order placement with valid information             | Critical |
| TS-059      | Verify order cannot be submitted with invalid/incomplete information | Critical |
| TS-060      | Verify behavior when attempting to place an order multiple times     | High     |

---

## 6. Localization

| Scenario ID | Test Scenario                                                     | Priority |
| ----------- | ----------------------------------------------------------------- | -------- |
| TS-061      | Verify website language selection functionality                   | Medium   |
| TS-062      | Verify page content is displayed in the selected language         | High     |
| TS-063      | Verify navigation labels are translated correctly                 | Medium   |
| TS-064      | Verify buttons and UI labels are translated correctly             | Medium   |
| TS-065      | Verify validation and error messages are translated correctly     | High     |
| TS-066      | Verify language selection persists after page refresh             | Medium   |
| TS-067      | Verify product information is displayed in the selected language  | Medium   |
| TS-068      | Verify no mixed-language content appears after language selection | High     |

---

## 7. UI and Navigation

| Scenario ID | Test Scenario                                       | Priority |
| ----------- | --------------------------------------------------- | -------- |
| TS-069      | Verify navigation between main application pages    | Medium   |
| TS-070      | Verify visibility of major UI elements              | Medium   |
| TS-071      | Verify interactive UI elements are usable           | Medium   |
| TS-072      | Verify buttons provide appropriate visual feedback  | Low      |
| TS-073      | Verify broken or incorrect navigation links         | Medium   |
| TS-074      | Verify browser back and forward navigation behavior | Medium   |
| TS-075      | Verify application behavior after page refresh      | Medium   |

---

## 8. Responsive and Cross-Browser Testing

| Scenario ID | Test Scenario                                       | Priority |
| ----------- | --------------------------------------------------- | -------- |
| TS-076      | Verify main functionality on desktop resolution     | Medium   |
| TS-077      | Verify main functionality on mobile resolution      | High     |
| TS-078      | Verify responsive layout of product pages           | Medium   |
| TS-079      | Verify responsive layout of shopping cart           | High     |
| TS-080      | Verify responsive layout of checkout                | High     |
| TS-081      | Verify core functionality across supported browsers | Medium   |

---

## 9. Negative and Edge Case Testing

| Scenario ID | Test Scenario                                                    | Priority |
| ----------- | ---------------------------------------------------------------- | -------- |
| TS-082      | Verify behavior with empty required fields                       | High     |
| TS-083      | Verify behavior with invalid input formats                       | High     |
| TS-084      | Verify behavior with extremely long input values                 | Medium   |
| TS-085      | Verify behavior with special characters in input fields          | Medium   |
| TS-086      | Verify behavior when a product becomes unavailable               | High     |
| TS-087      | Verify behavior when a selected product size becomes unavailable | High     |
| TS-088      | Verify behavior when cart contents become outdated               | High     |
| TS-089      | Verify behavior when checkout is interrupted                     | Medium   |
| TS-090      | Verify behavior when the user refreshes during checkout          | Medium   |

---

## 10. Exploratory Testing

| Scenario ID | Test Scenario                                                   | Priority |
| ----------- | --------------------------------------------------------------- | -------- |
| TS-091      | Explore critical user journeys for unexpected functional issues | High     |
| TS-092      | Explore authentication and session behavior                     | High     |
| TS-093      | Explore product search and filtering behavior                   | Medium   |
| TS-094      | Explore shopping cart state changes                             | High     |
| TS-095      | Explore checkout flow for unexpected behavior                   | Critical |
| TS-096      | Explore localization for inconsistent or untranslated content   | Medium   |
| TS-097      | Explore responsive behavior across different screen sizes       | Medium   |

---

## Scenario Coverage Summary

| Area                          | Scenario Count |
| ----------------------------- | -------------: |
| Authentication and Login      |             12 |
| Product Search                |              9 |
| Product Details and Selection |              7 |
| Shopping Cart                 |             16 |
| Checkout                      |             16 |
| Localization                  |              8 |
| UI and Navigation             |              7 |
| Responsive and Cross-Browser  |              6 |
| Negative and Edge Cases       |              9 |
| Exploratory Testing           |              7 |
| **Total**                     |         **97** |

---

## Priority Definitions

**Critical** — Failure can prevent a core business transaction or significantly impact revenue, security, or data integrity.

**High** — Failure affects an important business function or major user journey.

**Medium** — Failure affects secondary functionality or usability but does not prevent the main user journey.

**Low** — Minor usability, visual, or non-critical functional issue.
