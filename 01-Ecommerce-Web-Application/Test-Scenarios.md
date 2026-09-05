# Test Scenarios

High-level test scenarios for the e-commerce web application.

Test scenarios define the main areas of the application to be tested and provide high-level coverage before detailed test cases are created.

## Login

| Scenario ID | Test Scenario                                   | Priority |
| ----------- | ----------------------------------------------- | -------- |
| TS-001      | Verify user login functionality                 | High     |
| TS-002      | Verify login with valid and invalid credentials | High     |
| TS-003      | Verify validation of required login fields      | High     |
| TS-004      | Verify logout functionality                     | Medium   |

## Product Search

| Scenario ID | Test Scenario                                                  | Priority |
| ----------- | -------------------------------------------------------------- | -------- |
| TS-005      | Verify product search functionality                            | High     |
| TS-006      | Verify search with valid and invalid keywords                  | High     |
| TS-007      | Verify search behavior with an empty search field              | Medium   |
| TS-008      | Verify that search results are relevant to the entered keyword | High     |

## Product Page and Size Selection

| Scenario ID | Test Scenario                                                              | Priority |
| ----------- | -------------------------------------------------------------------------- | -------- |
| TS-009      | Verify product information displayed on the product page                   | High     |
| TS-010      | Verify product size selection functionality                                | High     |
| TS-011      | Verify unavailable product sizes                                           | High     |
| TS-012      | Verify selected product size is retained when adding a product to the cart | High     |

## Shopping Cart

| Scenario ID | Test Scenario                                             | Priority |
| ----------- | --------------------------------------------------------- | -------- |
| TS-013      | Verify adding products to the shopping cart               | High     |
| TS-014      | Verify product information displayed in the shopping cart | High     |
| TS-015      | Verify changing product quantity in the shopping cart     | High     |
| TS-016      | Verify cart total calculation                             | High     |
| TS-017      | Verify removing products from the shopping cart           | High     |
| TS-018      | Verify behavior of an empty shopping cart                 | Medium   |

## Checkout

| Scenario ID | Test Scenario                                              | Priority |
| ----------- | ---------------------------------------------------------- | -------- |
| TS-019      | Verify navigation from the shopping cart to checkout       | High     |
| TS-020      | Verify checkout information and validation                 | High     |
| TS-021      | Verify delivery/shipping information                       | High     |
| TS-022      | Verify available payment methods                           | High     |
| TS-023      | Verify order summary and total amount                      | High     |
| TS-024      | Verify successful order placement                          | High     |
| TS-027      | Verify checkout behavior with missing required information | High     |
| TS-028      | Verify checkout behavior with invalid input data           | High     |

## Localization

| Scenario ID | Test Scenario                                                     | Priority |
| ----------- | ----------------------------------------------------------------- | -------- |
| TS-025      | Verify website language selection functionality                   | Medium   |
| TS-026      | Verify that website content is displayed in the selected language | High     |

## UI and Navigation

| Scenario ID | Test Scenario                                    | Priority |
| ----------- | ------------------------------------------------ | -------- |
| TS-029      | Verify navigation between main application pages | Medium   |
| TS-030      | Verify visibility of major UI elements           | Medium   |
| TS-031      | Verify that interactive UI elements are usable   | Medium   |

## Product Quantity

| Scenario ID | Test Scenario                                                   | Priority |
| ----------- | --------------------------------------------------------------- | -------- |
| TS-032      | Verify product quantity selection functionality                 | High     |
| TS-033      | Verify behavior when increasing and decreasing product quantity | High     |
| TS-034      | Verify quantity limits and invalid quantity values              | Medium   |

