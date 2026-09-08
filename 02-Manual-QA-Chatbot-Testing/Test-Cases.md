# Test Cases — AI-Powered E-commerce Chatbot

## 1. Document Information

| Field               | Details                                                       |
| ------------------- | ------------------------------------------------------------- |
| Project             | AI-Powered E-commerce Chatbot                                 |
| Testing Type        | Manual Testing                                                |
| QA Role             | Junior Manual QA Tester                                       |
| Test Case Level     | Detailed                                                      |
| Primary Coverage    | Functional, Negative, Exploratory, Usability                  |
| Additional Coverage | Context, State, Data Consistency, Compatibility, Localization |
| Related Document    | `Test-Scenarios.md`                                           |

---

## 2. Test Case Purpose

This document contains detailed manual test cases for the AI-powered e-commerce chatbot.

The test cases are derived from the high-level scenarios defined in `Test-Scenarios.md`.

Each test case contains:

* Test Case ID
* Related Scenario ID
* Priority
* Preconditions
* Test Data
* Test Steps
* Expected Result

Execution results are documented separately in `Test-Execution.md`.

---

# 3. Test Case Format

Each test case follows the structure below:

**Test Case ID:** Unique identifier
**Scenario:** Related high-level scenario
**Priority:** Critical / High / Medium / Low
**Type:** Testing category
**Preconditions:** Required state before execution
**Test Data:** Input used during testing
**Steps:** Actions performed by the tester
**Expected Result:** Expected observable behavior

---

# 4. Basic Chatbot Functionality

## TC-001 — Open Chatbot

**Scenario:** TS-001
**Priority:** High
**Type:** Functional

### Preconditions

* Website is accessible.
* Chatbot functionality is available.

### Test Data

None.

### Steps

1. Open the website.
2. Locate the chatbot.
3. Open the chatbot.

### Expected Result

* Chatbot opens successfully.
* Initial chatbot interface is displayed.
* Message input is available.
* No visible UI error prevents interaction.

---

## TC-002 — Send Basic Greeting

**Scenario:** TS-002
**Priority:** Medium
**Type:** Functional / Usability

### Preconditions

* Chatbot is open.

### Test Data

`Hello`

### Steps

1. Enter `Hello`.
2. Send the message.
3. Review the chatbot response.

### Expected Result

* Chatbot responds to the greeting.
* Response is relevant to the greeting.
* No error is displayed.

---

## TC-003 — Search Product Category

**Scenario:** TS-003
**Priority:** High
**Type:** Functional

### Preconditions

* Chatbot is open.

### Test Data

`Tell me about laptops`

### Steps

1. Send the request.
2. Review the response.
3. Verify the product category identified by the chatbot.

### Expected Result

* Chatbot identifies laptops as the requested category.
* Response contains relevant information or product options.
* Response does not focus on an unrelated category.

---

## TC-004 — Search Specific Product

**Scenario:** TS-004
**Priority:** High
**Type:** Functional

### Test Data

`Tell me about iPhone 16`

### Steps

1. Send the request.
2. Review the response.
3. Verify the product name.

### Expected Result

* Chatbot identifies the requested product.
* Response is related to iPhone 16.
* No unrelated product is presented as the requested product.

---

## TC-005 — Request Product Information

**Scenario:** TS-005
**Priority:** High
**Type:** Functional

### Test Data

`What can you tell me about iPhone 16?`

### Steps

1. Send the request.
2. Review the response.
3. Check whether useful product information is provided.

### Expected Result

* Response contains relevant information about the requested product.
* Information is understandable.
* Response does not contain unrelated product information.

---

## TC-006 — Request Product Specifications

**Scenario:** TS-006
**Priority:** High
**Type:** Functional

### Test Data

`What are the specifications of iPhone 16?`

### Steps

1. Send the request.
2. Review the response.
3. Check the product attributes provided.

### Expected Result

* Relevant specifications are provided where available.
* Specifications correspond to the requested product.
* No unrelated model is substituted.

---

## TC-007 — Request Product Price

**Scenario:** TS-007
**Priority:** Critical
**Type:** Functional / Data Consistency

### Test Data

`What is the price of iPhone 16?`

### Steps

1. Send the request.
2. Record the price returned by the chatbot.
3. Open the relevant product page when a product link is available.
4. Compare the displayed prices.

### Expected Result

* Chatbot identifies the correct product.
* Price is displayed clearly.
* Chatbot price matches the corresponding product-page price where the values are expected to match.
* Any known price difference is clearly explained.

---

## TC-008 — Request Product Availability

**Scenario:** TS-008
**Priority:** Medium
**Type:** Functional

### Test Data

`Is this product available?`

### Preconditions

* A product has already been discussed.

### Steps

1. Send the availability question.
2. Review the response.

### Expected Result

* Chatbot provides an appropriate availability response when information is available.
* Response relates to the correct product.
* The chatbot does not present unsupported availability information as confirmed fact.

---

## TC-009 — Request Product Link

**Scenario:** TS-009
**Priority:** High
**Type:** Functional / Data Consistency

### Test Data

`Send me the link to this product.`

### Preconditions

* A specific product has already been discussed.

### Steps

1. Request the product link.
2. Open the returned link.
3. Review the destination page.
4. Compare the product identity with the conversation.

### Expected Result

* A relevant product link is provided when available.
* Link opens successfully.
* Destination corresponds to the product discussed.
* Product identity is consistent between chatbot and product page.

---

# 5. Product Recommendations

## TC-010 — Request Product Recommendation

**Scenario:** TS-010
**Priority:** Medium
**Type:** Functional

### Test Data

`Recommend a laptop for me.`

### Steps

1. Send the request.
2. Review the recommended products.
3. Check whether the recommendations are relevant to the requested category.

### Expected Result

* Relevant laptop recommendations are provided.
* Response explains or supports the recommendations where appropriate.

---

## TC-011 — Recommendation Within Budget

**Scenario:** TS-011
**Priority:** High
**Type:** Functional

### Test Data

`I want a laptop under 1200 GEL.`

### Steps

1. Send the request.
2. Review the recommendations.
3. Check the prices of recommended products.

### Expected Result

* Recommended products satisfy the stated budget where matching products are available.
* Products outside the budget are not presented as matching options without explanation.

---

## TC-012 — Recommendation Using Multiple Attributes

**Scenario:** TS-012
**Priority:** High
**Type:** Functional / Context

### Test Data

`I want a Lenovo laptop, black color, 8GB RAM.`

### Steps

1. Send the request.
2. Review the response.
3. Check whether each requirement is considered.

### Expected Result

* Lenovo requirement is considered.
* Color requirement is considered.
* RAM requirement is considered.
* If all requirements cannot be satisfied, the chatbot explains the limitation or asks an appropriate clarification question.

---

## TC-013 — Cheapest Suitable Product

**Scenario:** TS-013
**Priority:** Medium
**Type:** Functional / Data Consistency

### Test Data

`Which laptop is the cheapest?`

### Steps

1. Send the request.
2. Record the product and price returned.
3. Compare with available product information.

### Expected Result

* Chatbot identifies the appropriate cheapest available option based on the available data.
* Price information is consistent with the referenced product information.

---

## TC-014 — Recommendation for Specific Use Case

**Scenario:** TS-014
**Priority:** Medium
**Type:** Functional

### Test Data

`I need a laptop for gaming.`

### Steps

1. Send the request.
2. Review the recommendations.
3. Check whether the intended use is considered.

### Expected Result

* Recommendations are relevant to gaming use.
* Response provides useful reasoning or relevant performance considerations where available.

---

# 6. Conversation Context

## TC-015 — Product Follow-Up Question

**Scenario:** TS-015, TS-016
**Priority:** High
**Type:** Context

### Test Data

Message 1: `Tell me about iPhone 16.`
Message 2: `What colors does it have?`

### Steps

1. Send the first message.
2. Wait for the response.
3. Send the follow-up question.
4. Review the response.

### Expected Result

* Chatbot understands that `it` refers to iPhone 16.
* Response relates to the correct product.

---

## TC-016 — Continue Multi-Message Product Conversation

**Scenario:** TS-017
**Priority:** High
**Type:** Context

### Test Data

1. `Tell me about laptops.`
2. `Which one is cheaper?`
3. `What RAM does it have?`
4. `Does it come in black?`

### Steps

1. Send the messages sequentially.
2. Review each response.
3. Check whether the relevant product context is maintained.

### Expected Result

* Follow-up questions are interpreted using the relevant conversation context.
* Product information is not mixed between different products.
* Responses remain relevant to the active conversation.

---

## TC-017 — Topic Switching

**Scenario:** TS-018
**Priority:** Medium
**Type:** Context

### Test Data

1. `Tell me about laptops.`
2. `Actually show me phones.`
3. `Where is your store?`

### Steps

1. Send the first message.
2. Send the second message.
3. Send the third message.
4. Review each response.

### Expected Result

* Laptop request is handled correctly.
* Phone request becomes the active product topic.
* Store-related question is handled independently.
* Previous topic does not incorrectly affect the new request.

---

## TC-018 — Return to Previous Topic

**Scenario:** TS-019
**Priority:** Medium
**Type:** Context / State

### Test Data

1. `Tell me about laptops.`
2. `Show me phones.`
3. `Go back to the laptop we discussed.`

### Steps

1. Start the laptop conversation.
2. Change the topic to phones.
3. Return to the laptop topic.
4. Review the response.

### Expected Result

* Chatbot handles the topic return appropriately.
* Previously discussed information is not incorrectly mixed with phone information.
* If clarification is required, the chatbot asks an appropriate question.

---

## TC-019 — Multiple Topics in One Conversation

**Scenario:** TS-020
**Priority:** Medium
**Type:** Context / Exploratory

### Test Data

A conversation containing product, store, payment, and delivery-related questions.

### Steps

1. Start a product conversation.
2. Ask a store-related question.
3. Ask a payment-related question.
4. Return to the product topic.
5. Review each response.

### Expected Result

* Each topic receives a relevant response.
* Context from unrelated topics is not incorrectly applied.
* Product information remains consistent when returning to the product topic.

---

# 7. Complex and Negative Requirements

## TC-020 — Multiple Product Requirements

**Scenario:** TS-021
**Priority:** Critical
**Type:** Functional / Negative

### Test Data

`I want a Lenovo laptop, black, 8GB RAM, under 1200 GEL for gaming.`

### Steps

1. Send the complete request.
2. Review the response.
3. Identify which requirements were considered.
4. Check whether any requirement was ignored.

### Expected Result

* All major requirements are considered.
* If no exact match exists, the chatbot explains the limitation or offers reasonable alternatives.
* The chatbot does not silently ignore major requirements.

---

## TC-021 — Complex Product Request

**Scenario:** TS-022
**Priority:** High
**Type:** Functional / Exploratory

### Test Data

`I need a laptop with good battery life, gaming performance, black design, enough RAM, reasonable price and warranty.`

### Steps

1. Send the request.
2. Review the response.
3. Identify which requirements are addressed.
4. Check whether the chatbot asks for clarification when necessary.

### Expected Result

* The chatbot attempts to address the major requirements.
* The response does not unnecessarily reduce the request to a single attribute.
* Clarification is requested when required.

---

## TC-022 — Conflicting Requirements

**Scenario:** TS-023
**Priority:** High
**Type:** Negative / Exploratory

### Test Data

`I want a laptop under 1000 GEL with high gaming performance.`

### Steps

1. Send the request.
2. Review the response.
3. Evaluate whether the chatbot recognizes the potential conflict.

### Expected Result

* Chatbot recognizes the trade-off where applicable.
* It provides realistic options or asks a useful clarification question.
* It does not silently present an unrelated product as a match.

---

## TC-023 — Incomplete Product Request

**Scenario:** TS-024
**Priority:** Medium
**Type:** Negative

### Test Data

`I need a good laptop.`

### Steps

1. Send the request.
2. Review the response.

### Expected Result

* Chatbot provides useful general guidance or asks clarification questions.
* It does not make unjustified assumptions about important requirements.

---

## TC-024 — Ambiguous Product Request

**Scenario:** TS-025
**Priority:** Medium
**Type:** Negative / Exploratory

### Test Data

`Which one?`

### Preconditions

* More than one product has been discussed.

### Steps

1. Discuss multiple products.
2. Send `Which one?`
3. Review the response.

### Expected Result

* Chatbot asks for clarification when the reference is ambiguous.
* It does not randomly select a product without sufficient context.

---

# 8. Product Comparison

## TC-025 — Compare Requested Products

**Scenario:** TS-026, TS-030
**Priority:** Critical
**Type:** Functional / Data Consistency

### Test Data

`Compare iPhone 16 and Samsung S24.`

### Steps

1. Send the comparison request.
2. Review the product names in the response.
3. Check the compared products.
4. Review the comparison criteria.

### Expected Result

* The requested products are compared.
* Product identity is preserved.
* The chatbot does not silently replace a requested product with another model.
* Relevant comparison information is provided.

---

## TC-026 — Compare Product Prices

**Scenario:** TS-027
**Priority:** High
**Type:** Functional / Data Consistency

### Test Data

`Which one is cheaper?`

### Preconditions

* Two products have already been discussed.

### Steps

1. Ask which product is cheaper.
2. Review the prices used in the response.
3. Compare the prices.
4. Verify the conclusion.

### Expected Result

* Correct products are used for the comparison.
* Prices are consistent with the available product information.
* The cheaper product is correctly identified.

---

## TC-027 — Compare Product Specifications

**Scenario:** TS-028
**Priority:** High
**Type:** Functional

### Test Data

`Compare the RAM, storage and camera of these two phones.`

### Preconditions

* Two products have already been identified.

### Steps

1. Send the comparison request.
2. Review the specifications.
3. Check whether the values belong to the correct products.

### Expected Result

* Requested attributes are compared.
* Product specifications are associated with the correct products.
* No product information is incorrectly mixed.

---

## TC-028 — Follow-Up Comparison Question

**Scenario:** TS-029
**Priority:** High
**Type:** Context

### Test Data

Message 1: `Compare iPhone 16 and Samsung S24.`
Message 2: `Which one has better battery life?`

### Steps

1. Send the comparison request.
2. Wait for the response.
3. Send the follow-up question.
4. Review the response.

### Expected Result

* Chatbot understands which two products are being compared.
* Follow-up response remains within the correct comparison context.
* The response addresses battery life rather than restarting the comparison with unrelated products.

---

# 9. Purchase Flow

## TC-029 — Express Purchase Intent

**Scenario:** TS-031
**Priority:** High
**Type:** Functional / Usability

### Test Data

`I want to buy it.`

### Preconditions

* A specific product has already been discussed.

### Steps

1. Send the purchase request.
2. Review the response.
3. Check whether the previously discussed product is retained.

### Expected Result

* Purchase intent is recognized.
* The correct product remains associated with the request.
* Clear next steps are provided where supported.

---

## TC-030 — Ask How to Order

**Scenario:** TS-032
**Priority:** High
**Type:** Functional

### Test Data

`How can I order this laptop?`

### Steps

1. Send the question.
2. Review the response.

### Expected Result

* Chatbot explains the available ordering process where information is available.
* Response provides understandable next steps.

---

## TC-031 — Ask About Payment

**Scenario:** TS-033
**Priority:** High
**Type:** Functional

### Test Data

`Can I pay cash?`

### Steps

1. Send the payment question.
2. Review the response.

### Expected Result

* Chatbot provides the available payment information.
* Payment options are clearly distinguished where applicable.
* Response does not invent unsupported payment methods.

---

## TC-032 — Ask About Pickup

**Scenario:** TS-034
**Priority:** Medium
**Type:** Functional

### Test Data

`Can I pick it up from the store?`

### Steps

1. Send the question.
2. Review the response.

### Expected Result

* Chatbot provides appropriate pickup information where available.
* Response clearly communicates what the user can do next.

---

# 10. Operator and Conversation State

## TC-033 — Request Operator Assistance

**Scenario:** TS-035, TS-036
**Priority:** High
**Type:** Functional / State

### Test Data

`Connect me to an operator.`

### Steps

1. Send the operator request.
2. Observe the chatbot state.
3. Review any status or confirmation message.

### Expected Result

* Operator request is accepted where functionality is available.
* User receives a clear confirmation.
* Chat enters the expected operator/waiting state.

---

## TC-034 — Return From Operator Mode

**Scenario:** TS-037
**Priority:** Critical
**Type:** Functional / State

### Test Data

Message 1: `Connect me to operator.`
Message 2: `Never mind. Can you return me to the chatbot?`

### Steps

1. Request an operator.
2. Wait for the operator state to appear.
3. Request a return to the AI chatbot.
4. Observe the result.

### Expected Result

* Current state is communicated clearly.
* If returning to AI is supported, the user can return successfully.
* If it is not supported, the limitation is clearly communicated.
* User is not left in an unclear state.

---

## TC-035 — Minimize and Reopen During Operator State

**Scenario:** TS-038, TS-039, TS-040
**Priority:** High
**Type:** State / Usability

### Preconditions

* Operator request has been submitted.

### Steps

1. Request an operator.
2. Minimize the chatbot.
3. Reopen the chatbot.
4. Review the displayed conversation and state.

### Expected Result

* Chatbot reopens successfully.
* Conversation history is displayed as expected.
* Current state is clearly communicated.
* User understands the available next action.

---

## TC-036 — Verify State After Page Refresh

**Scenario:** TS-040
**Priority:** High
**Type:** State

### Preconditions

* Operator state or active conversation exists.

### Steps

1. Start the relevant conversation.
2. Refresh the browser page.
3. Open the chatbot again.
4. Review the conversation state.

### Expected Result

* State after refresh matches the expected application behavior.
* Conversation history is preserved where supported.
* User is not left with a misleading or contradictory state.

---

# 11. Negative Input

## TC-037 — Random Numeric Input

**Scenario:** TS-042
**Priority:** Low
**Type:** Negative

### Test Data

`123456789`

### Steps

1. Send the numeric input.
2. Review the response.
3. Observe the interface.

### Expected Result

* Chatbot handles the input gracefully.
* No crash occurs.
* Chat interface remains usable.
* Response is appropriate for unsupported or unclear input.

---

## TC-038 — Special Characters

**Scenario:** TS-043
**Priority:** Low
**Type:** Negative

### Test Data

`22@@@@@@@`

### Steps

1. Send the message.
2. Review the response.
3. Observe the chatbot interface.

### Expected Result

* Chatbot does not crash.
* Input is handled gracefully.
* No unexpected UI behavior occurs.

---

## TC-039 — Unknown Product

**Scenario:** TS-044
**Priority:** Medium
**Type:** Negative

### Test Data

`Tell me about a product that is not available in the store.`

### Steps

1. Send the request.
2. Review the response.

### Expected Result

* Chatbot does not present an unavailable product as confirmed store inventory.
* User receives an appropriate explanation or alternative where supported.

---

## TC-040 — Unexpected Request

**Scenario:** TS-045
**Priority:** Medium
**Type:** Negative / Exploratory

### Test Data

An unrelated request outside the normal e-commerce flow.

### Steps

1. Send the unexpected request.
2. Review the response.

### Expected Result

* Chatbot responds gracefully.
* Response does not cause a broken conversation state.
* User is redirected toward supported functionality where appropriate.

---

# 12. Localization

## TC-041 — English Interaction

**Scenario:** TS-046
**Priority:** High
**Type:** Localization / Functional

### Test Data

`I need a laptop for work.`

### Steps

1. Send the English request.
2. Review the response.

### Expected Result

* Chatbot understands the request.
* Response is relevant and understandable.
* Product terminology remains clear.

---

## TC-042 — Georgian Interaction

**Scenario:** TS-047
**Priority:** High
**Type:** Localization / Functional

### Test Data

A Georgian product-related request.

### Steps

1. Send the Georgian request.
2. Review the response.
3. Check product names and terminology.

### Expected Result

* Chatbot understands the request.
* Response is relevant to the user's request.
* Product information remains understandable.

---

## TC-043 — Mixed-Language Interaction

**Scenario:** TS-048
**Priority:** Medium
**Type:** Localization / Exploratory

### Test Data

`Hello გამარჯობა Hola Bonjour`

### Steps

1. Send the mixed-language message.
2. Review the response.
3. Continue with a product-related question if appropriate.

### Expected Result

* Chatbot handles mixed-language input without breaking the conversation.
* Response remains relevant.
* Product context remains understandable.

---

## TC-044 — Product Terminology Consistency

**Scenario:** TS-049
**Priority:** Medium
**Type:** Localization / Data Consistency

### Steps

1. Discuss a product in English.
2. Continue the conversation in Georgian.
3. Refer to the same product again.
4. Compare the product identity and terminology.

### Expected Result

* The same product remains identifiable across language changes.
* Product names are not incorrectly changed to unrelated products.
* Important product information remains consistent.

---

# 13. Usability

## TC-045 — Response Clarity

**Scenario:** TS-050
**Priority:** High
**Type:** Usability

### Steps

1. Send a normal product request.
2. Review the chatbot response.
3. Evaluate whether the response is understandable.

### Expected Result

* Response is clear.
* Information is structured sufficiently for the user to understand.
* Important information is not unnecessarily obscured.

---

## TC-046 — Response Relevance

**Scenario:** TS-051
**Priority:** High
**Type:** Usability

### Test Data

A specific product question.

### Steps

1. Send the question.
2. Review the response.
3. Compare the response with the requested information.

### Expected Result

* Response directly addresses the user's question.
* Unrelated information does not replace the requested information.

---

## TC-047 — Conversation Flow

**Scenario:** TS-052
**Priority:** High
**Type:** Usability

### Steps

1. Start a product conversation.
2. Ask follow-up questions.
3. Change the topic.
4. Continue the conversation.
5. Observe the interaction flow.

### Expected Result

* User can continue the conversation naturally.
* Chatbot responses provide enough context for the next action.
* No unnecessary dead-end is introduced.

---

## TC-048 — Product Information Readability

**Scenario:** TS-053
**Priority:** Medium
**Type:** Usability

### Steps

1. Request product information.
2. Review the returned content.
3. Check readability and organization.

### Expected Result

* Product information is understandable.
* Important attributes can be identified without unnecessary confusion.

---

## TC-049 — Purchase Flow Clarity

**Scenario:** TS-054
**Priority:** High
**Type:** Usability

### Steps

1. Discuss a product.
2. Express purchase intent.
3. Review the chatbot response.
4. Identify the next available action.

### Expected Result

* Purchase intent is recognized.
* User receives understandable next steps where supported.
* The flow does not leave the user without direction.

---

# 14. Mobile and Compatibility

## TC-050 — Desktop/Notebook Chatbot Usage

**Scenario:** TS-055
**Priority:** High
**Type:** Compatibility

### Steps

1. Open the website on the tested desktop/notebook environment.
2. Open the chatbot.
3. Send several messages.
4. Review the interface.

### Expected Result

* Chatbot opens successfully.
* Messages can be sent and received.
* Chat interface remains usable.
* No major UI issue prevents normal interaction.

---

## TC-051 — Mobile Chatbot Usage

**Scenario:** TS-056
**Priority:** High
**Type:** Compatibility / Usability

### Preconditions

* Tested mobile device and browser are available.

### Steps

1. Open the website on the mobile device.
2. Open the chatbot.
3. Send several messages.
4. Scroll through the conversation.
5. Minimize and reopen the chatbot.
6. Send another message.

### Expected Result

* Chatbot is usable on mobile.
* Input field works correctly.
* Messages are displayed correctly.
* Conversation can be scrolled.
* Minimize/reopen behavior remains usable.
* No major UI element prevents interaction.

---

## TC-052 — Different Screen Sizes

**Scenario:** TS-057
**Priority:** Medium
**Type:** Compatibility / Usability

### Steps

1. Use the chatbot in the tested desktop/notebook environment.
2. Use the chatbot on the tested mobile environment.
3. Compare the basic interaction experience.

### Expected Result

* Core chatbot interaction remains available.
* Important controls remain accessible.
* No major layout issue prevents the user from sending or reading messages.

---

# 15. Exploratory Test Cases

## TC-053 — Rapid Topic Switching

**Scenario:** TS-058
**Priority:** Medium
**Type:** Exploratory / Context

### Steps

1. Ask about laptops.
2. Switch to phones.
3. Ask about a store.
4. Switch back to laptops.
5. Ask a product-specific follow-up.

### Expected Result

* Chatbot follows the active topic.
* Previous topics do not incorrectly override the current request.
* Relevant context is retained where expected.

---

## TC-054 — Multiple Requirements With Follow-Up

**Scenario:** TS-059
**Priority:** High
**Type:** Exploratory / Context

### Steps

1. Send a request containing several product requirements.
2. Ask a follow-up question about one requirement.
3. Ask another follow-up about a different requirement.
4. Review the responses.

### Expected Result

* Chatbot maintains the original product context.
* Follow-up questions are connected to the correct request.
* Requirements are not unnecessarily lost between messages.

---

## TC-055 — Comparison After Context Change

**Scenario:** TS-060
**Priority:** High
**Type:** Exploratory / Context

### Steps

1. Discuss one product.
2. Change to another product category.
3. Introduce two products for comparison.
4. Request a comparison.

### Expected Result

* Comparison uses the products explicitly requested for comparison.
* Previous conversation context does not cause unrelated product substitution.

---

## TC-056 — State Change During Active Conversation

**Scenario:** TS-061
**Priority:** High
**Type:** Exploratory / State

### Steps

1. Start an active product conversation.
2. Request operator assistance.
3. Minimize the chatbot.
4. Reopen it.
5. Continue the conversation where possible.

### Expected Result

* State transitions are understandable.
* Relevant conversation history is preserved where supported.
* User is not left in an unexplained or contradictory state.

---

## TC-057 — Unexpected Conversation Sequence

**Scenario:** TS-062
**Priority:** Medium
**Type:** Exploratory

### Steps

1. Start with a product request.
2. Ask an unrelated question.
3. Return to the product.
4. Request an operator.
5. Continue with another product-related question.

### Expected Result

* Chatbot handles the sequence without breaking.
* Responses remain relevant to the current interaction.
* Unexpected state changes are documented as observations or defects when appropriate.

---

# 16. Test Data Reference

| Category              | Example                             |
| --------------------- | ----------------------------------- |
| Product               | iPhone 16                           |
| Product Category      | Laptop                              |
| Brand                 | Lenovo                              |
| Budget                | Under 1000 GEL                      |
| RAM                   | 8GB                                 |
| Color                 | Black                               |
| Usage                 | Gaming                              |
| Language              | English                             |
| Language              | Georgian                            |
| Mixed Language        | `Hello გამარჯობა Hola Bonjour`      |
| Invalid Input         | `123456789`                         |
| Special Characters    | `22@@@@@@@`                         |
| Purchase Intent       | `I want to buy it`                  |
| Operator Request      | `Connect me to operator`            |
| Ambiguous Input       | `Which one?`                        |
| Multiple Requirements | Brand + price + RAM + color + usage |

---

# 17. Execution Status

Test execution results are intentionally maintained separately from this document.

Possible execution statuses include:

* **PASS** — Expected behavior observed.
* **FAIL** — Observed behavior does not meet the expected result.
* **PARTIAL** — Some expected behavior works, but one or more aspects require improvement.
* **BLOCKED** — Test cannot be completed because a required condition is unavailable.
* **NOT EXECUTED** — Test case has not yet been executed.
* **OBSERVATION** — Behavior was observed but cannot be confirmed as a defect.
* **NEEDS VERIFICATION** — Additional information or confirmation is required.

The execution status should not be permanently embedded into the test-case definition because the same test case may be executed again during retesting or regression testing.

---

# 18. Defect Traceability

Confirmed defects identified during testing are documented separately.

| Bug ID  | Related Test Case      | Area                                     |
| ------- | ---------------------- | ---------------------------------------- |
| BUG-001 | TC-007, TC-009         | Product price / data consistency         |
| BUG-002 | TC-034                 | Return from operator mode                |
| BUG-003 | TC-035, TC-036         | Operator state / minimize-reopen         |
| BUG-004 | TC-025, TC-028         | Product comparison / product identity    |
| BUG-005 | TC-020, TC-021, TC-054 | Multiple requirements / complex requests |

A test case may identify an observation or requirement concern without resulting in a confirmed defect.

---

# 19. Test Case Coverage

The test cases cover the following major areas:

| Area                            | Test Cases      |
| ------------------------------- | --------------- |
| Basic Chatbot Functionality     | TC-001 – TC-009 |
| Product Recommendations         | TC-010 – TC-014 |
| Conversation Context            | TC-015 – TC-019 |
| Complex / Negative Requirements | TC-020 – TC-024 |
| Product Comparison              | TC-025 – TC-028 |
| Purchase Flow                   | TC-029 – TC-032 |
| Operator / State                | TC-033 – TC-036 |
| Negative Input                  | TC-037 – TC-040 |
| Localization                    | TC-041 – TC-044 |
| Usability                       | TC-045 – TC-049 |
| Mobile / Compatibility          | TC-050 – TC-052 |
| Exploratory                     | TC-053 – TC-057 |

**Total Detailed Test Cases: 57**

---

# 20. QA Notes

These test cases are designed for a practical manual QA portfolio and demonstrate the relationship between high-level scenarios and detailed test execution.

They are not intended to represent exhaustive production coverage.

For AI-powered applications, expected behavior may depend on:

* Available product data
* Business rules
* Conversation context
* Supported functionality
* Product availability
* Operator workflow
* Application state

When expected behavior cannot be confirmed, the result should be documented objectively as an observation or requirement concern rather than automatically reported as a defect.

The test cases should be reused during retesting and regression testing after relevant fixes or application changes.

