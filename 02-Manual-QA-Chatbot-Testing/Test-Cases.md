# Chatbot Testing — Test Cases

## Project

AI-powered e-commerce chatbot integrated into an online shopping website.

## Test Case Format

Each test case contains:

- Test Case ID
- Test Scenario
- Preconditions
- Test Data
- Steps
- Expected Result

---

## TC-001 — Start Chatbot

**Test Scenario:** Verify that the chatbot can be started successfully.

**Preconditions:**
- Website is accessible.
- Chatbot is available.

**Test Data:**
- None

**Steps:**
1. Open the website.
2. Open the chatbot.
3. Observe the initial message.

**Expected Result:**
- Chatbot opens successfully.
- Initial greeting is displayed.
- Message input is available.

---

## TC-002 — Send Simple Greeting

**Test Scenario:** Verify that the chatbot responds to a simple greeting.

**Preconditions:**
- Chatbot is open.

**Test Data:**
`Hello`

**Steps:**
1. Enter `Hello` in the chat input.
2. Send the message.
3. Observe the response.

**Expected Result:**
- Chatbot responds with a relevant greeting.
- No error is displayed.

---

## TC-003 — Search for Laptop Category

**Test Scenario:** Verify that the chatbot understands a product-category request.

**Preconditions:**
- Chatbot is open.

**Test Data:**
`Tell me about laptops`

**Steps:**
1. Send the message.
2. Review the chatbot response.

**Expected Result:**
- Chatbot identifies laptops as the requested category.
- Relevant laptop information or options are provided.
- The response is related to the user's request.

---

## TC-004 — Search for Specific Product

**Test Scenario:** Verify that the chatbot can provide information about a specific product.

**Test Data:**
`What is the price of iPhone 16?`

**Steps:**
1. Send the request.
2. Review the response.
3. Verify the product name and price.

**Expected Result:**
- Chatbot identifies iPhone 16.
- A price is provided if available.
- Product information is relevant to iPhone 16.

---

## TC-005 — Ask Product Follow-Up Question

**Test Scenario:** Verify that the chatbot maintains product context.

**Test Data:**

Message 1:
`Tell me about iPhone 16`

Message 2:
`What colors does it have?`

**Steps:**
1. Send the first message.
2. Wait for the response.
3. Send the follow-up question.
4. Review the response.

**Expected Result:**
- Chatbot understands that "it" refers to iPhone 16.
- Available colors are provided for the correct product.

---

## TC-006 — Ask Multiple Product Attributes

**Test Scenario:** Verify that the chatbot considers multiple product requirements.

**Test Data:**

`I want a Lenovo laptop, black color, 8GB RAM.`

**Steps:**
1. Send the request.
2. Review the chatbot response.
3. Check whether Lenovo, black color, and 8GB RAM are considered.

**Expected Result:**
- Chatbot considers all provided requirements.
- Recommended products match the requested attributes where possible.
- If more information is required, useful clarification questions are asked.

---

## TC-007 — Ask for Multiple Attributes in One Message

**Test Scenario:** Verify that the chatbot handles a complex product request.

**Test Data:**

`Color, RAM, price, design, material, battery, warranty and gaming performance.`

**Steps:**
1. Send the message.
2. Review the response.
3. Check which requirements are addressed.

**Expected Result:**
- Chatbot addresses the important requested attributes.
- The response does not unnecessarily reduce the request to one attribute.
- If the request is too broad, the chatbot asks useful clarification questions.

---

## TC-008 — Conflicting Requirements

**Test Scenario:** Verify how the chatbot handles conflicting product requirements.

**Test Data:**

`I want a laptop under 1000 GEL with high gaming performance.`

**Steps:**
1. Send the request.
2. Review the response.

**Expected Result:**
- Chatbot recognizes that the requirements may conflict.
- Chatbot explains available options or asks clarification questions.
- It does not recommend an unrelated product without explanation.

---

## TC-009 — Cheapest Laptop

**Test Scenario:** Verify that the chatbot identifies the cheapest available laptop.

**Test Data:**
`Which laptop is the cheapest?`

**Steps:**
1. Ask the chatbot which laptop is cheapest.
2. Record the product and price.
3. Compare the information with the available product data.

**Expected Result:**
- Chatbot identifies the correct cheapest available option.
- Price information is accurate.

---

## TC-010 — Budget Filtering

**Test Scenario:** Verify that the chatbot respects the user's budget.

**Test Data:**
`I want a laptop under 1200 GEL.`

**Steps:**
1. Send the request.
2. Review recommended products.
3. Check their prices.

**Expected Result:**
- Recommended products are within the requested budget.
- Products outside the budget are not presented as matching recommendations without explanation.

---

## TC-011 — Gaming Laptop Recommendation

**Test Scenario:** Verify that the chatbot considers intended usage when recommending a product.

**Test Data:**
`I need a laptop for gaming.`

**Steps:**
1. Send the request.
2. Review the recommendations.
3. Check whether the suggested products are appropriate for gaming.

**Expected Result:**
- Chatbot recommends gaming-capable laptops.
- The response explains relevant performance considerations where appropriate.

---

## TC-012 — Product Comparison

**Test Scenario:** Verify that the chatbot compares the requested products.

**Test Data:**
`Compare iPhone 16 and Samsung S24.`

**Steps:**
1. Send the comparison request.
2. Review the response.
3. Check the product names in the response.

**Expected Result:**
- The chatbot compares iPhone 16 and Samsung S24.
- It does not silently replace one requested model with another model.
- Relevant comparison criteria are provided.

---

## TC-013 — Price Comparison

**Test Scenario:** Verify that the chatbot compares product prices correctly.

**Test Data:**
`Which one is cheaper?`

**Preconditions:**
- Two products have already been discussed.

**Steps:**
1. Ask which product is cheaper.
2. Review the response.
3. Compare the prices provided.

**Expected Result:**
- Chatbot understands which two products are being compared.
- Correct prices are used.
- The cheaper product is correctly identified.

---

## TC-014 — Verify Price Against Product Page

**Test Scenario:** Verify consistency between chatbot price and website product-page price.

**Test Data:**
A specific product discussed by the chatbot.

**Steps:**
1. Ask the chatbot for the product price.
2. Record the price provided.
3. Open the product link provided by the chatbot.
4. Compare the chatbot price with the product-page price.

**Expected Result:**
- Chatbot price matches the current product-page price.
- If prices differ, the chatbot clearly explains the difference.

---

## TC-015 — Verify Product Link

**Test Scenario:** Verify that a product link opens the correct product.

**Steps:**
1. Ask the chatbot for a product link.
2. Click the provided link.
3. Check the opened product page.
4. Compare the product name and attributes with the chatbot response.

**Expected Result:**
- Link opens successfully.
- Correct product page is displayed.
- Product information matches the product discussed in the conversation.

---

## TC-016 — Purchase Intent

**Test Scenario:** Verify that the chatbot recognizes clear purchase intent.

**Test Data:**
`I want to buy it.`

**Preconditions:**
- A product has already been discussed.

**Steps:**
1. Send the purchase request.
2. Review the chatbot response.

**Expected Result:**
- Chatbot recognizes the user's purchase intent.
- Clear next steps are provided.
- Previously discussed product information is retained.

---

## TC-017 — Ask How to Order

**Test Scenario:** Verify that the chatbot explains the ordering process.

**Test Data:**
`How can I order this laptop?`

**Steps:**
1. Send the question.
2. Review the response.

**Expected Result:**
- Chatbot explains the available purchase process.
- The response provides clear and useful next steps.

---

## TC-018 — Ask About Payment Methods

**Test Scenario:** Verify that the chatbot provides correct payment information.

**Test Data:**
`Can I pay cash?`

**Steps:**
1. Send the question.
2. Review the response.

**Expected Result:**
- Chatbot explains whether cash payment is available.
- Online and physical-store payment methods are clearly distinguished if applicable.

---

## TC-019 — Operator Handoff

**Test Scenario:** Verify that the chatbot can transfer the user to a human operator.

**Test Data:**
`Connect me to an operator.`

**Steps:**
1. Send the request.
2. Observe the chatbot state.
3. Check the displayed status message.

**Expected Result:**
- Operator request is accepted.
- User receives a clear confirmation.
- Chat enters the correct operator/waiting state.

---

## TC-020 — Attempt to Return to AI After Operator Request

**Test Scenario:** Verify chatbot behavior after an operator request has been submitted.

**Test Data:**

Message 1:
`Connect me to operator.`

Message 2:
`Never mind. Can you return to chatbot?`

**Steps:**
1. Request an operator.
2. Wait for the operator request confirmation.
3. Send a request to return to the chatbot.
4. Observe the response.

**Expected Result:**
- System clearly explains the current state.
- If returning to AI is supported, the user can return.
- If it is not supported, the limitation is clearly communicated.
- User should not be left in an unclear or stuck state.

---

## TC-021 — Minimize Chat While Waiting for Operator

**Test Scenario:** Verify chat behavior when minimized during an operator request.

**Preconditions:**
- Operator request has been submitted.

**Steps:**
1. Request an operator.
2. Minimize the chat using the available minimize control.
3. Reopen the chat.
4. Observe the conversation and current state.

**Expected Result:**
- Chat opens successfully.
- Conversation history is preserved.
- Current operator state is displayed correctly.
- User is not left confused about the next step.

---

## TC-022 — Refresh Page During Operator State

**Test Scenario:** Verify operator state after page refresh.

**Preconditions:**
- Operator request has been submitted.

**Steps:**
1. Request an operator.
2. Refresh the browser page.
3. Open the chatbot.
4. Check the current state.

**Expected Result:**
- Chat state is consistent after refresh.
- Conversation history is preserved where expected.
- User can understand the current state.

---

## TC-023 — Random Numeric Input

**Test Scenario:** Verify chatbot handling of irrelevant numeric input.

**Test Data:**
`123456789`

**Steps:**
1. Send the message.
2. Review the response.

**Expected Result:**
- Chatbot handles the input gracefully.
- No crash or broken UI occurs.
- Response remains appropriate.

---

## TC-024 — Special Characters

**Test Scenario:** Verify chatbot handling of special characters.

**Test Data:**
`22@@@@@@@`

**Steps:**
1. Send the message.
2. Review the response.

**Expected Result:**
- Chatbot does not crash.
- Message is handled gracefully.
- No unexpected UI behavior occurs.

---

## TC-025 — Mixed Language Input

**Test Scenario:** Verify chatbot handling of multiple languages in one message.

**Test Data:**
`Hello გამარჯობა Hola Bonjour`

**Steps:**
1. Send the message.
2. Review the response.

**Expected Result:**
- Chatbot handles the mixed-language input.
- Conversation does not break.
- Response remains relevant.

---

## TC-026 — Topic Switching

**Test Scenario:** Verify that the chatbot handles changes in product category.

**Test Data:**

Message 1:
`Tell me about laptops.`

Message 2:
`Actually show me phones.`

Message 3:
`Where is your store?`

**Steps:**
1. Send each message sequentially.
2. Review each response.
3. Check whether the chatbot updates the conversation context correctly.

**Expected Result:**
- Laptop request is handled correctly.
- Phone request becomes the new topic.
- Store question is handled independently.
- Previous context does not incorrectly affect the new request.

---

## TC-027 — Long Conversation Context

**Test Scenario:** Verify that relevant context is maintained during a long conversation.

**Steps:**
1. Start a conversation about laptops.
2. Ask about price.
3. Ask about RAM.
4. Ask about colors.
5. Ask about warranty.
6. Change to another product.
7. Return to the original topic.
8. Ask what product was previously selected.

**Expected Result:**
- Chatbot maintains relevant context.
- Product information is not mixed between products.
- Previously discussed information is recalled correctly where supported.
- No unrelated product is selected.

---

## TC-028 — Ambiguous Follow-Up Question

**Test Scenario:** Verify that the chatbot asks for clarification when the user's question is ambiguous.

**Preconditions:**
- Multiple products have been discussed.

**Test Data:**
`Which one?`

**Steps:**
1. Discuss multiple products.
2. Send `Which one?`
3. Review the response.

**Expected Result:**
- Chatbot asks a clarification question.
- It does not randomly select a product.

---

## TC-029 — Contradictory Requirements

**Test Scenario:** Verify that the chatbot handles changing requirements.

**Test Data:**

Message 1:
`I want a black laptop.`

Message 2:
`Actually, I want silver.`

**Steps:**
1. Send the first requirement.
2. Send the second requirement.
3. Review the next recommendation.

**Expected Result:**
- Latest requirement is considered.
- The chatbot does not continue recommending black products without explanation.

---

## TC-030 — Mobile Chatbot Testing

**Test Scenario:** Verify the chatbot on a mobile device.

**Preconditions:**
- Supported mobile device and browser are available.

**Steps:**
1. Open the website on the mobile device.
2. Open the chatbot.
3. Send several messages.
4. Scroll through the conversation.
5. Minimize and reopen the chatbot.
6. Send another message.

**Expected Result:**
- Chatbot is usable on mobile.
- Messages are displayed correctly.
- Input field works correctly.
- Conversation can be scrolled.
- Minimize/reopen works correctly.
- No major UI elements overlap or disappear.

---

# Test Data Examples

The following test data can be used during exploratory and functional testing:

| Category | Example |
|---|---|
| Product | iPhone 16 |
| Product category | Laptop |
| Brand | Lenovo |
| Price | Under 1000 GEL |
| RAM | 8GB |
| Color | Black |
| Usage | Gaming |
| Language | English |
| Language | Georgian |
| Mixed language | Hello გამარჯობა Hola |
| Invalid input | 123456789 |
| Special characters | 22@@@@@@@ |
| Purchase intent | I want to buy it |
| Operator request | Connect me to operator |
| Ambiguous input | Which one? |

---

# Test Case Execution Notes

During execution, the following should be recorded where relevant:

- Test case result: Pass / Fail / Blocked
- Device
- Operating system and version
- Browser and version
- Date of execution
- Relevant screenshot or screen recording
- Bug ID if a defect is found

For failed tests, a separate bug report should be created with clear reproduction steps, actual result, expected result, and supporting evidence.
