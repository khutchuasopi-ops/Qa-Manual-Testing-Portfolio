# Test Plan — AI-Powered E-commerce Chatbot

## 1. Document Information

| Field              | Details                                                                                             |
| ------------------ | --------------------------------------------------------------------------------------------------- |
| Project            | AI-Powered E-commerce Chatbot                                                                       |
| Testing Type       | Manual Testing                                                                                      |
| QA Role            | Junior Manual QA Tester                                                                             |
| Application Type   | Web-based E-commerce Chatbot                                                                        |
| Primary Testing    | Functional, Negative, Exploratory, Usability                                                        |
| Additional Focus   | Context, State, Data Consistency, Compatibility                                                     |
| Test Environments  | Desktop / Notebook and Mobile Device                                                                |
| Test Documentation | Test Plan, Test Scenarios, Test Cases, Test Execution, Exploratory Testing, Bug Reports, Case Study |

---

## 2. Test Objective

The objective of this testing activity is to evaluate whether the AI-powered e-commerce chatbot provides a consistent, understandable, and usable experience when users search for products, ask product-related questions, compare products, continue conversations, and interact with purchase or operator-related flows.

The testing focuses on identifying functional issues, incorrect or inconsistent product information, context and state problems, incomplete handling of complex requests, usability concerns, and unexpected behavior during normal and negative user interactions.

---

## 3. Testing Scope

### 3.1 In Scope

The following areas are included in the manual testing scope.

### Product Functionality

* Product search
* Product categories
* Product information
* Product specifications
* Product prices
* Product recommendations
* Product availability-related responses where applicable
* Product links
* Product comparison
* Price comparison
* Follow-up questions about products
* Multiple product requirements

### Conversation and Context

* Initial conversation
* Greeting and basic interaction
* Follow-up questions
* Conversation context
* Product-related context
* Topic switching
* Multiple topics within a conversation
* Conversation memory
* Ambiguous questions
* Conflicting requirements
* Multiple requirements in one request
* Continuation of an existing conversation

### Purchase and Operator Flow

* Purchase intent
* Ordering-related questions
* Payment-related questions
* Pickup-related questions
* Operator handoff
* Operator state
* Returning from operator mode to the chatbot
* Minimize and reopen behavior
* Conversation state after reopening

### Negative and Exploratory Testing

* Invalid input
* Unexpected questions
* Random input
* Special characters
* Unknown or unavailable products
* Ambiguous requests
* Conflicting requirements
* Complex product requests
* Unexpected conversation sequences
* Mixed-language input
* Unexpected state changes

### Usability and Localization

* Response clarity
* Relevance of chatbot responses
* Conversation flow
* Ease of continuing a conversation
* Understandability of product information
* User experience during purchase-related interactions
* English-language interaction
* Georgian-language interaction
* Mixed-language interaction
* Consistency of product names and terminology

### Device Compatibility

* Desktop / notebook usage
* Mobile device usage
* Chat interaction on different screen sizes
* Basic usability across tested device types

---

## 4. Out of Scope

The following areas are outside the scope of this manual QA project:

* Source code testing
* Database testing
* API testing
* Performance testing
* Load testing
* Stress testing
* Security penetration testing
* Automated testing
* Backend infrastructure testing
* Internal AI model implementation
* Server-side implementation details

These areas were not directly accessible or evaluated as part of this manual testing activity.

---

## 5. Testing Approach

Testing is performed using a combination of structured and exploratory approaches.

### 5.1 Functional Testing

Verify that the chatbot performs expected user-facing functions, including:

* Product search
* Product information retrieval
* Product recommendations
* Product comparison
* Product links
* Purchase-related interaction
* Operator handoff
* Conversation continuation

### 5.2 Negative Testing

Provide invalid, unexpected, incomplete, ambiguous, or conflicting input to evaluate how the chatbot handles situations outside normal user flows.

Examples include:

* Unknown products
* Random text
* Special characters
* Conflicting product requirements
* Incomplete questions
* Unexpected topic changes
* Multiple requirements in one message

### 5.3 Exploratory Testing

Explore the chatbot beyond predefined test cases to identify unexpected behavior and risks that may not be covered by structured scenarios.

Exploratory testing focuses particularly on:

* Conversation context
* Product substitution
* State changes
* Complex requests
* Operator flow
* Minimize/reopen behavior
* Topic switching
* Mixed-language interaction

Detailed exploratory findings are documented separately in `Exploratory-Testing.md`.

### 5.4 Usability Testing

Evaluate whether users can understand and continue the conversation effectively.

Focus areas include:

* Response clarity
* Relevance
* Conversation flow
* Product information readability
* Purchase-flow clarity
* Operator-flow usability
* Mobile interaction

### 5.5 Context Testing

Verify that the chatbot correctly understands information from previous messages and uses relevant conversation context when responding to follow-up questions.

### 5.6 State Testing

Verify behavior when the chatbot changes or preserves its state, including:

* AI chatbot state
* Operator state
* Minimize/reopen behavior
* Conversation continuation
* Return from operator mode

### 5.7 Data Consistency Testing

Compare product-related information returned by the chatbot with the corresponding product information where available.

Primary focus:

* Product price
* Product identity
* Product comparison information
* Product links
* Product-related attributes

### 5.8 Compatibility Testing

Perform basic compatibility checks across the tested desktop/notebook and mobile environments.

The purpose is to identify user-facing differences in chatbot interaction and usability rather than perform exhaustive browser/device compatibility coverage.

---

## 6. Test Environment

Testing is performed using:

* Desktop / Notebook
* Mobile device
* Web browser
* Chatbot web interface

Where relevant, device, operating system, browser, and browser version should be recorded in the corresponding test evidence or defect report.

This portfolio documents the manual testing process and observed results rather than claiming exhaustive coverage of every browser, operating system, or device combination.

---

## 7. Test Data

Test data includes realistic user requests related to e-commerce product discovery and purchasing.

Examples of test data categories:

### Product Search

* General product categories
* Specific product names
* Product types
* Unknown products

### Product Requirements

* Price range
* Product category
* Brand
* Technical specifications
* Multiple attributes
* Conflicting requirements
* Multiple products in one request

### Product Comparison

* Two-product comparison
* Price comparison
* Specification comparison
* Follow-up comparison questions

### Conversation Data

* Follow-up questions
* Topic changes
* Multiple topics
* Ambiguous requests
* Mixed-language messages

### Purchase Data

* Purchase intent
* Payment questions
* Pickup questions
* Operator requests

No real customer personal information or sensitive user data is used in this portfolio testing activity.

---

## 8. Entry Criteria

Testing can begin when:

* The chatbot is accessible.
* The chatbot interface is available.
* The user can send messages.
* The chatbot can return responses.
* Product-related information is available.
* Relevant product links can be accessed where applicable.
* Purchase-related functionality can be explored where available.
* Operator functionality is available for testing where applicable.

---

## 9. Exit Criteria

Testing can be considered complete for the defined portfolio scope when:

* Planned test scenarios have been reviewed and executed where applicable.
* Core chatbot flows have been tested.
* Negative and exploratory areas have been investigated.
* Important observed defects have been documented.
* Relevant usability concerns have been recorded.
* Context and state behavior has been evaluated.
* Product information consistency has been checked where applicable.
* Major testing risks have been identified.
* Test execution results have been documented.
* The remaining limitations and out-of-scope areas are clearly stated.

---

## 10. Defect Management Approach

When an unexpected behavior is identified, it is evaluated before being documented as a confirmed defect.

The following factors are considered:

1. Expected behavior based on the available requirement or user flow.
2. Actual observed behavior.
3. Reproducibility.
4. User impact.
5. Severity.
6. Whether the behavior can be confirmed as a functional issue or should remain an observation/requirement concern.

Confirmed defects are documented separately in the `Bug-Reports` directory.

Current documented defects include:

* `BUG-001` — Product price inconsistency
* `BUG-002` — Unable to return from operator mode
* `BUG-003` — Operator state persists after minimize/reopen
* `BUG-004` — Requested product replaced during comparison
* `BUG-005` — Multiple product requirements are not properly handled

---

## 11. Test Deliverables

The following documentation is maintained as part of this project:

| Document                 | Purpose                                            |
| ------------------------ | -------------------------------------------------- |
| `README.md`              | Project-level QA portfolio overview                |
| `Project-Overview.md`    | Project context, objectives, scope and limitations |
| `Test-Plan.md`           | Testing strategy, scope, environments and risks    |
| `Test-Scenarios.md`      | High-level functional and behavioral scenarios     |
| `Test-Cases.md`          | Detailed test conditions and expected results      |
| `Test-Execution.md`      | Recorded execution results and observations        |
| `Exploratory-Testing.md` | Exploratory testing approach and findings          |
| `Bug-Reports/`           | Detailed defect documentation                      |
| `Case-Study.md`          | End-to-end QA case study and conclusions           |

---

## 12. Main Testing Risks

The main risks considered during testing are:

### Product Information Risks

* Incorrect product information
* Incorrect prices
* Inconsistent product data
* Incorrect product links
* Product substitution during comparison

### Conversation Risks

* Loss of context
* Incorrect interpretation of follow-up questions
* Context mixing after topic changes
* Incorrect handling of multiple topics
* Incorrect handling of ambiguous requests

### Complex Request Risks

* Ignoring one or more user requirements
* Focusing only on one product attribute
* Replacing the requested product with another product
* Inability to satisfy multiple requirements simultaneously

### State Risks

* Incorrect chatbot state
* Incorrect operator state
* Failure to return from operator mode
* State persistence after minimize/reopen
* Unexpected conversation continuation

### Purchase Flow Risks

* Unclear purchase-related responses
* Incomplete ordering flow
* Unclear payment or pickup information
* Inconsistent transition between chatbot and operator

### Usability Risks

* Unclear responses
* Irrelevant recommendations
* Difficult conversation flow
* Poor mobile usability
* Inconsistent terminology

---

## 13. Testing Priorities

Testing priority is based on user impact and the importance of the functionality.

### High Priority

* Product price accuracy
* Product identity
* Product comparison
* Product links
* Conversation context
* Operator handoff and return
* Chatbot state
* Multiple product requirements

### Medium Priority

* Product recommendations
* Follow-up questions
* Topic switching
* Purchase-related questions
* Payment and pickup information
* Mobile usability

### Lower Priority

* Unusual input combinations
* Random input
* Special-character input
* Less common conversation paths

Priority may change when a newly discovered issue affects a critical user flow.

---

## 14. Limitations

This is a practical manual QA portfolio project and does not represent a complete production-level quality assessment.

The testing is limited by:

* Available user-facing functionality
* Available product information
* Available chatbot behavior
* Available device coverage
* Limited visibility into backend systems
* No direct access to source code
* No direct database validation
* No API-level validation
* No automated test execution
* No dedicated performance or security testing

Where expected behavior cannot be confirmed from available requirements or observable application behavior, the result is documented as an observation or requirement concern rather than automatically classified as a defect.

---

## 15. QA Conclusion

The testing approach is designed to demonstrate a structured manual QA process for an AI-powered e-commerce chatbot.

The project covers both traditional functional testing and AI/chatbot-specific risks, including:

* Conversation context
* Follow-up interactions
* Multiple requirements
* Ambiguous and conflicting requests
* Product consistency
* Product comparison
* Conversation state
* Operator interaction
* Minimize/reopen behavior
* Negative and exploratory testing
* Usability and localization

The identified defects and observations are documented in the corresponding execution and bug-report documentation.

The main quality risks identified during testing relate to **data consistency, complex user requests, conversation state, product comparison, and operator-flow behavior**.

Further testing would be recommended if additional requirements, environments, browsers, API access, database access, performance requirements, or security requirements became available.
