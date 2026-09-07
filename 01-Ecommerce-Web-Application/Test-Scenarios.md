# Test Scenarios — E-commerce Web Application

## Overview

This document contains high-level test scenarios for the confidential e-commerce web application.

Test scenarios define the main areas of the application to be tested before detailed test cases are created.

The scenarios focus on the main user journeys and core functional areas of the application.

---

# 1. Login and Authentication

| Scenario ID | Test Scenario                                   | Priority |
| ----------- | ----------------------------------------------- | -------- |
| TS-001      | Verify user login functionality                 | High     |
| TS-002      | Verify login with valid and invalid credentials | High     |
| TS-003      | Verify validation of required login fields      | High     |
| TS-004      | Verify logout functionality                     | Medium   |

---

# 2. Product Search

| Scenario ID | Test Scenario                                                  | Priority |
| ----------- | -------------------------------------------------------------- | -------- |
| TS-005      | Verify product search functionality                            | High     |
| TS-006      | Verify search with valid and invalid keywords                  | High     |
| TS-007      | Verify search behavior with an empty search field              | Medium   |
| TS-008      | Verify that search results are relevant to the entered keyword | High     |

---

# 3. Product Page and Size Selection

| Scenario ID | Test Scenario                                                                       | Priority |
| ----------- | ----------------------------------------------------------------------------------- | -------- |
| TS-009      | Verify product information displayed on the product page                            | High     |
| TS-010      | Verify product size selection functionality                                         | High     |
| TS-011      | Verify behavior when a product size is unavailable                                  | High     |
| TS-012      | Verify that the selected product size is retained when adding a product to the cart | High     |

---

# 4. Shopping Cart

| Scenario ID | Test Scenario                                             | Priority |
| ----------- | --------------------------------------------------------- | -------- |
| TS-013      | Verify adding products to the shopping cart               | High     |
| TS-014      | Verify product information displayed in the shopping cart | High     |
| TS-015      | Verify changing product quantity in the shopping cart     | High     |
| TS-016      | Verify cart total calculation                             | High     |
| TS-017      | Verify removing products from the shopping cart           | High     |
| TS-018      | Verify behavior of an empty shopping cart                 | Medium   |

---

# 5. Checkout

| Scenario ID | Test Scenario                                                 | Priority |
| ----------- | ------------------------------------------------------------- | -------- |
| TS-019      | Verify navigation from the shopping cart to checkout          | High     |
| TS-020      | Verify checkout information and validation                    | High     |
| TS-021      | Verify delivery and shipping information                      | High     |
| TS-022      | Verify available payment methods                              | High     |
| TS-023      | Verify order summary and total amount                         | High     |
| TS-024      | Verify successful order placement                             | High     |
| TS-025      | Verify checkout behavior when required information is missing | High     |
| TS-026      | Verify checkout behavior with invalid input data              | High     |

---

# 6. Localization

| Scenario ID | Test Scenario                                                     | Priority |
| ----------- | ----------------------------------------------------------------- | -------- |
| TS-027      | Verify website language selection functionality                   | Medium   |
| TS-028      | Verify that website content is displayed in the selected language | High     |

---

# 7. UI and Navigation

| Scenario ID | Test Scenario                                    | Priority |
| ----------- | ------------------------------------------------ | -------- |
| TS-029      | Verify navigation between main application pages | Medium   |
| TS-030      | Verify visibility of major UI elements           | Medium   |
| TS-031      | Verify that interactive UI elements are usable   | Medium   |

---

# 8. Product Quantity

| Scenario ID | Test Scenario                                                   | Priority |
| ----------- | --------------------------------------------------------------- | -------- |
| TS-032      | Verify product quantity selection functionality                 | High     |
| TS-033      | Verify behavior when increasing and decreasing product quantity | High     |
| TS-034      | Verify quantity limits and invalid quantity values              | Medium   |

---

## Scenario Coverage Summary

| Area                            | Scenario Range      |  Count |
| ------------------------------- | ------------------- | -----: |
| Login and Authentication        | TS-001 – TS-004     |      4 |
| Product Search                  | TS-005 – TS-008     |      4 |
| Product Page and Size Selection | TS-009 – TS-012     |      4 |
| Shopping Cart                   | TS-013 – TS-018     |      6 |
| Checkout                        | TS-019 – TS-026     |      8 |
| Localization                    | TS-027 – TS-028     |      2 |
| UI and Navigation               | TS-029 – TS-031     |      3 |
| Product Quantity                | TS-032 – TS-034     |      3 |
| **Total**                       | **TS-001 – TS-034** | **34** |

## Priority Definitions

* **High** — Important functionality that may directly affect the main user journey or core application behavior.
* **Medium** — Functionality that should be tested but has lower impact on the main user journey.

## Notes

* These are high-level test scenarios. Detailed test steps are documented separately in `Test-Cases.md`.
* Test execution results are documented separately in `Test-Execution/Test-Execution-Report.md`.
* The application and related test information are confidential.
* No confidential application, organization, user, credential, or business information is included in this portfolio.

