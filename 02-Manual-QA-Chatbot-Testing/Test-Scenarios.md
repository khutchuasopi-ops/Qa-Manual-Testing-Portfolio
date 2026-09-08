# Test Scenarios — AI-Powered E-commerce Chatbot

## 1. Document Information

| Field               | Details                                                       |
| ------------------- | ------------------------------------------------------------- |
| Project             | AI-Powered E-commerce Chatbot                                 |
| Testing Type        | Manual Testing                                                |
| QA Role             | Junior Manual QA Tester                                       |
| Scenario Level      | High-Level                                                    |
| Primary Coverage    | Functional, Negative, Exploratory, Usability                  |
| Additional Coverage | Context, State, Data Consistency, Compatibility, Localization |

---

## 2. Scenario Objective

The purpose of this document is to define the high-level test scenarios used to evaluate the main user-facing functionality and behavioral risks of the AI-powered e-commerce chatbot.

The scenarios cover product discovery, product information, conversation context, complex requirements, product comparison, purchase-related interactions, operator flow, conversation state, negative input, usability, and localization.

Detailed test steps and expected results are maintained separately in `Test-Cases.md`.

---

# 3. Product Search and Product Information

### TS-001 — Start a chatbot conversation

**Priority:** High
**Type:** Functional

Verify that the user can open and start interacting with the chatbot.

---

### TS-002 — Send a basic greeting

**Priority:** Medium
**Type:** Functional / Usability

Verify that the chatbot responds appropriately to a basic greeting.

---

### TS-003 — Search for a product category

**Priority:** High
**Type:** Functional

Verify that the chatbot can understand a general product category request and provide relevant results or information.

---

### TS-004 — Search for a specific product

**Priority:** High
**Type:** Functional

Verify that the chatbot can identify and respond to a request for a specific product.

---

### TS-005 — Request product information

**Priority:** High
**Type:** Functional

Verify that the chatbot provides relevant information about a requested product.

---

### TS-006 — Request product specifications

**Priority:** High
**Type:** Functional

Verify that the chatbot provides relevant technical or product attributes when requested.

---

### TS-007 — Request product price

**Priority:** Critical
**Type:** Functional / Data Consistency

Verify that the chatbot provides the correct price for the requested product.

---

### TS-008 — Request product availability information

**Priority:** Medium
**Type:** Functional

Verify how the chatbot handles questions related to product availability.

---

### TS-009 — Request a product link

**Priority:** High
**Type:** Functional / Data Consistency

Verify that the chatbot provides a relevant product link when one is available.

---

# 4. Product Recommendations

### TS-010 — Request product recommendations

**Priority:** Medium
**Type:** Functional

Verify that the chatbot can provide relevant product recommendations based on the user's request.

---

### TS-011 — Request recommendations within a budget

**Priority:** High
**Type:** Functional

Verify that the chatbot considers a specified budget when recommending products.

---

### TS-012 — Request recommendations using multiple attributes

**Priority:** High
**Type:** Functional / Context

Verify that the chatbot considers multiple product requirements in a single request.

Examples may include:

* Product type
* Budget
* Brand
* Technical specification
* Intended use

---

### TS-013 — Request the cheapest suitable product

**Priority:** Medium
**Type:** Functional

Verify that the chatbot correctly interprets a request for the lowest-priced suitable product.

---

### TS-014 — Request a product for a specific use case

**Priority:** Medium
**Type:** Functional

Verify that the chatbot considers the user's intended use when recommending a product.

---

# 5. Follow-Up Questions and Conversation Context

### TS-015 — Ask a follow-up question

**Priority:** High
**Type:** Context

Verify that the chatbot correctly understands a follow-up question based on the previous conversation.

---

### TS-016 — Ask for additional information about the previously discussed product

**Priority:** High
**Type:** Context

Verify that the chatbot maintains the relevant product context when the user asks another question.

---

### TS-017 — Continue a product conversation through multiple messages

**Priority:** High
**Type:** Context

Verify that product-related context is maintained across several consecutive messages.

---

### TS-018 — Change the conversation topic

**Priority:** Medium
**Type:** Context

Verify that the chatbot can switch to a new topic without incorrectly carrying unrelated information from the previous topic.

---

### TS-019 — Return to a previously discussed topic

**Priority:** Medium
**Type:** Context / State

Verify whether the chatbot can correctly handle returning to a previous topic during the same conversation.

---

### TS-020 — Handle multiple topics in one conversation

**Priority:** Medium
**Type:** Context / Exploratory

Verify that the chatbot maintains appropriate context when the conversation contains multiple topics.

---

# 6. Complex and Multiple Requirements

### TS-021 — Handle a request containing multiple product requirements

**Priority:** Critical
**Type:** Functional / Negative

Verify that the chatbot considers all relevant requirements included in a single user request.

---

### TS-022 — Handle a complex product request

**Priority:** High
**Type:** Functional / Exploratory

Verify that the chatbot can process a request containing several product attributes and provide a useful response.

---

### TS-023 — Handle conflicting requirements

**Priority:** High
**Type:** Negative / Exploratory

Verify how the chatbot responds when the user's requirements cannot reasonably be satisfied simultaneously.

---

### TS-024 — Handle incomplete product requirements

**Priority:** Medium
**Type:** Negative

Verify that the chatbot asks for clarification or provides an appropriate response when important information is missing.

---

### TS-025 — Handle ambiguous product requirements

**Priority:** Medium
**Type:** Negative / Exploratory

Verify that the chatbot can identify ambiguity and respond appropriately rather than making an unjustified assumption.

---

# 7. Product Comparison

### TS-026 — Compare two requested products

**Priority:** Critical
**Type:** Functional

Verify that the chatbot compares the products explicitly requested by the user.

---

### TS-027 — Compare product prices

**Priority:** High
**Type:** Functional / Data Consistency

Verify that prices are correctly represented when comparing products.

---

### TS-028 — Compare product specifications

**Priority:** High
**Type:** Functional

Verify that relevant product attributes are correctly compared.

---

### TS-029 — Ask a follow-up question about a comparison

**Priority:** High
**Type:** Context

Verify that the chatbot maintains the correct products and comparison context during follow-up questions.

---

### TS-030 — Verify product identity during comparison

**Priority:** Critical
**Type:** Data Consistency / Negative

Verify that the chatbot does not replace one of the products requested by the user with an unrelated product.

---

# 8. Purchase-Related Interaction

### TS-031 — Express purchase intent

**Priority:** High
**Type:** Functional / Usability

Verify that the chatbot correctly recognizes when the user wants to purchase a product.

---

### TS-032 — Ask about ordering

**Priority:** High
**Type:** Functional

Verify how the chatbot responds to questions about the ordering process.

---

### TS-033 — Ask about payment

**Priority:** High
**Type:** Functional

Verify that the chatbot provides appropriate payment-related information where available.

---

### TS-034 — Ask about pickup

**Priority:** Medium
**Type:** Functional

Verify how the chatbot handles questions about product pickup.

---

# 9. Operator Handoff and State

### TS-035 — Request operator assistance

**Priority:** High
**Type:** Functional

Verify that the user can request assistance from a human operator where the functionality is available.

---

### TS-036 — Transfer conversation to operator mode

**Priority:** High
**Type:** Functional / State

Verify that the chatbot correctly transitions from AI interaction to operator mode.

---

### TS-037 — Return from operator mode to chatbot

**Priority:** Critical
**Type:** Functional / State

Verify that the user can return from operator mode to the AI chatbot when the expected functionality is available.

---

### TS-038 — Minimize chatbot while in operator mode

**Priority:** High
**Type:** State / Usability

Verify that minimizing the chatbot does not produce an unexpected or confusing state.

---

### TS-039 — Reopen chatbot after minimizing

**Priority:** High
**Type:** State

Verify that reopening the chatbot results in the expected conversation state.

---

### TS-040 — Preserve or reset conversation state correctly

**Priority:** High
**Type:** State

Verify that conversation state after transitions, minimizing, reopening, or operator interaction matches the expected behavior.

---

# 10. Negative Input

### TS-041 — Submit invalid input

**Priority:** Medium
**Type:** Negative

Verify that the chatbot handles invalid or unsupported input appropriately.

---

### TS-042 — Submit random input

**Priority:** Low
**Type:** Negative / Exploratory

Verify how the chatbot responds to random or unrelated text.

---

### TS-043 — Submit special characters

**Priority:** Low
**Type:** Negative

Verify that special characters do not cause unexpected chatbot behavior.

---

### TS-044 — Ask about an unknown product

**Priority:** Medium
**Type:** Negative

Verify that the chatbot handles unknown or unavailable product requests appropriately.

---

### TS-045 — Submit an unexpected request

**Priority:** Medium
**Type:** Negative / Exploratory

Verify that the chatbot responds appropriately when the request is outside the expected e-commerce conversation flow.

---

# 11. Localization and Language Handling

### TS-046 — Interact in English

**Priority:** High
**Type:** Localization / Functional

Verify that the chatbot correctly handles English-language requests.

---

### TS-047 — Interact in Georgian

**Priority:** High
**Type:** Localization / Functional

Verify that the chatbot correctly handles Georgian-language requests.

---

### TS-048 — Use mixed English and Georgian

**Priority:** Medium
**Type:** Localization / Exploratory

Verify that the chatbot can understand and respond appropriately to mixed-language messages.

---

### TS-049 — Maintain product terminology consistently

**Priority:** Medium
**Type:** Localization / Data Consistency

Verify that product names, categories, and relevant terminology remain understandable and consistent across supported language interactions.

---

# 12. Usability

### TS-050 — Verify response clarity

**Priority:** High
**Type:** Usability

Verify that chatbot responses are understandable and provide useful information to the user.

---

### TS-051 — Verify response relevance

**Priority:** High
**Type:** Usability

Verify that responses address the user's actual request rather than unrelated information.

---

### TS-052 — Verify conversation flow

**Priority:** High
**Type:** Usability

Verify that the user can naturally continue the conversation without unnecessary confusion.

---

### TS-053 — Verify product information readability

**Priority:** Medium
**Type:** Usability

Verify that product information is presented in a clear and understandable manner.

---

### TS-054 — Verify purchase-flow clarity

**Priority:** High
**Type:** Usability

Verify that purchase-related responses provide a clear understanding of the next available action.

---

# 13. Mobile and Device Compatibility

### TS-055 — Use chatbot on desktop/notebook

**Priority:** High
**Type:** Compatibility

Verify the basic chatbot experience in the desktop/notebook environment.

---

### TS-056 — Use chatbot on mobile device

**Priority:** High
**Type:** Compatibility / Usability

Verify the basic chatbot experience on a mobile device.

---

### TS-057 — Verify chat interaction on different screen sizes

**Priority:** Medium
**Type:** Compatibility / Usability

Verify that the chatbot remains usable when accessed from different screen sizes represented by the tested environments.

---

# 14. Exploratory Risk Scenarios

### TS-058 — Rapidly change conversation topics

**Priority:** Medium
**Type:** Exploratory / Context

Explore whether rapid topic changes cause context mixing or incorrect responses.

---

### TS-059 — Combine multiple requirements with follow-up questions

**Priority:** High
**Type:** Exploratory / Context

Explore whether the chatbot maintains all relevant requirements when the user continues with follow-up questions.

---

### TS-060 — Compare products after changing context

**Priority:** High
**Type:** Exploratory / Context

Explore whether previous conversation context affects a new product comparison.

---

### TS-061 — Change state during an active conversation

**Priority:** High
**Type:** Exploratory / State

Explore behavior when minimizing, reopening, or switching between chatbot and operator interactions during an active conversation.

---

### TS-062 — Use unexpected conversation sequences

**Priority:** Medium
**Type:** Exploratory

Explore chatbot behavior when the user does not follow the expected conversation sequence.

---

# 15. Scenario Coverage Summary

| Area                         | Scenario IDs    | Coverage                                     |
| ---------------------------- | --------------- | -------------------------------------------- |
| Product Search & Information | TS-001 – TS-009 | Product discovery and information            |
| Recommendations              | TS-010 – TS-014 | Recommendation logic                         |
| Context & Follow-Up          | TS-015 – TS-020 | Conversation context                         |
| Complex Requirements         | TS-021 – TS-025 | Multiple, conflicting and ambiguous requests |
| Product Comparison           | TS-026 – TS-030 | Comparison and product identity              |
| Purchase Flow                | TS-031 – TS-034 | Purchase-related interaction                 |
| Operator & State             | TS-035 – TS-040 | Operator and conversation state              |
| Negative Testing             | TS-041 – TS-045 | Invalid and unexpected input                 |
| Localization                 | TS-046 – TS-049 | Language handling                            |
| Usability                    | TS-050 – TS-054 | User-facing experience                       |
| Compatibility                | TS-055 – TS-057 | Desktop/mobile                               |
| Exploratory Risks            | TS-058 – TS-062 | Advanced exploratory coverage                |

**Total High-Level Test Scenarios: 62**

---

# 16. Traceability

The scenarios are mapped to the detailed test cases in `Test-Cases.md`.

The execution results are documented in `Test-Execution.md`.

Confirmed defects are documented in:

* `Bug-Reports/BUG-001.md`
* `Bug-Reports/BUG-002.md`
* `Bug-Reports/BUG-003.md`
* `Bug-Reports/BUG-004.md`
* `Bug-Reports/BUG-005.md`

Exploratory findings are documented in `Exploratory-Testing.md`.

---

# 17. Testing Notes

Not every scenario necessarily results in a confirmed defect.

During manual testing, an observed behavior may be classified as:

* Pass
* Fail
* Partial / Needs Improvement
* Observation
* Requirement Concern
* Needs Verification

A behavior is documented as a confirmed defect only when there is sufficient evidence that the observed result does not meet the expected behavior.

This distinction is especially important for AI-powered applications because some responses may depend on available product data, business rules, conversation context, or expected chatbot behavior.

---

## 18. QA Perspective

These scenarios are designed to demonstrate a structured manual QA approach rather than exhaustive production test coverage.

The main focus is on identifying risks that can directly affect the user's ability to:

1. Find products.
2. Understand product information.
3. Compare the correct products.
4. Continue a conversation.
5. Provide multiple requirements.
6. Complete or continue purchase-related interactions.
7. Transition between AI and operator interaction.
8. Maintain the expected conversation state.
9. Use the chatbot in supported languages.
10. Interact with the chatbot comfortably across tested devices.
