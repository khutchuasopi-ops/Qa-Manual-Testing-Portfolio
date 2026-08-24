# Chatbot Testing — Test Scenarios

## Project

AI-powered e-commerce chatbot integrated into an online shopping website.

## Testing Objective

The goal of these scenarios is to verify that the chatbot understands user requests, provides relevant and accurate information, maintains conversation context, and handles different user flows correctly.

The scenarios also cover exploratory testing of unusual, incomplete, conflicting, and multi-attribute user requests.

---

## 1. Chat Initialization

### TS-001 — Start a new conversation

Verify that the chatbot opens correctly and displays an initial greeting.

### TS-002 — Send a simple greeting

Verify that the chatbot responds appropriately to messages such as:

- Hello
- Hi
- Hola
- გამარჯობა

### TS-003 — Start conversation with an immediate product request

Verify that the chatbot can handle a product request without requiring a greeting first.

---

## 2. Product Search

### TS-004 — Search for a product category

Verify that the chatbot can understand requests such as:

- Tell me about laptops
- Show me phones
- I need a TV

### TS-005 — Search for a specific product

Verify that the chatbot can identify a specific product or model.

Example:

> Tell me about iPhone 16.

### TS-006 — Search for a non-existing product

Verify that the chatbot clearly informs the user when a requested product cannot be found.

### TS-007 — Search using incorrect or incomplete product names

Verify that the chatbot can handle spelling mistakes, incomplete names, or informal product descriptions.

---

## 3. Product Information

### TS-008 — Ask for product price

Verify that the chatbot provides the correct product price.

### TS-009 — Ask for product colors

Verify that the chatbot provides available color options for the selected product.

### TS-010 — Ask for RAM

Verify that the chatbot provides the correct RAM information.

### TS-011 — Ask for storage

Verify that the chatbot provides the correct storage information.

### TS-012 — Ask about warranty

Verify that the chatbot provides correct warranty information or correctly redirects the user when the information is unavailable.

### TS-013 — Ask about product material

Verify that the chatbot distinguishes between a product's color and its physical material.

Example:

> Silver color

versus:

> Made from silver material.

---

## 4. Conversation Context

### TS-014 — Ask follow-up questions about the previously mentioned product

Example:

> Tell me about laptops.

Followed by:

> Which one is the cheapest?

Verify that the chatbot understands that "which one" refers to the previously discussed laptops.

### TS-015 — Continue asking questions about the selected product

Example:

> How much RAM does it have?

Followed by:

> What colors does it come in?

Verify that the chatbot maintains the correct product context.

### TS-016 — Ask what product was previously selected

Verify that the chatbot can correctly identify the product and attributes discussed earlier in the conversation.

### TS-017 — Change product category during the conversation

Example:

> I want a laptop.

Followed by:

> Actually show me phones.

Verify that the chatbot correctly changes the conversation context.

---

## 5. Multi-Attribute Requests

### TS-018 — Provide multiple product requirements in one message

Example:

> I want a laptop under 1200 GEL, 8GB RAM, black, for office work.

Verify that the chatbot considers all important attributes.

### TS-019 — Provide many attributes in one message

Example:

> Color, RAM, price, design, material, battery, warranty, gaming and office use.

Verify that the chatbot does not ignore most of the requested attributes.

### TS-020 — Ask for a product with conflicting requirements

Example:

> I want a very cheap laptop with high gaming performance.

Verify that the chatbot identifies the conflict and asks useful clarification questions or explains the available options.

### TS-021 — Ask for a product using natural language

Example:

> I need something cheap but powerful.

Verify that the chatbot can understand the general intent and ask relevant follow-up questions.

---

## 6. Product Recommendations

### TS-022 — Ask for the cheapest product

Verify that the chatbot identifies the correct cheapest available option.

### TS-023 — Ask for a product within a specific budget

Example:

> I want a laptop under 1000 GEL.

Verify that recommendations stay within the requested budget.

### TS-024 — Ask for a gaming laptop

Verify that the chatbot recommends products suitable for gaming rather than general office laptops.

### TS-025 — Ask for a product for office use

Verify that the chatbot recommends appropriate products for office work.

### TS-026 — Ask for a premium product with a limited budget

Verify that the chatbot handles competing requirements appropriately instead of selecting a product without explaining the trade-off.

---

## 7. Product Comparison

### TS-027 — Compare two specific products

Example:

> Compare iPhone 16 and Samsung S24.

Verify that the chatbot compares the requested models.

### TS-028 — Compare products when one requested product is unavailable

Verify that the chatbot clearly explains the availability issue instead of silently replacing the requested product.

### TS-029 — Ask which product is cheaper

Verify that the chatbot compares the correct products and provides accurate prices.

### TS-030 — Ask which product has a better camera

Verify that the chatbot provides a relevant comparison based on camera specifications.

---

## 8. Price Accuracy

### TS-031 — Compare chatbot price with product page price

Verify that the price provided by the chatbot matches the current product page.

### TS-032 — Check discounted prices

Verify that the chatbot clearly distinguishes between the original price and the discounted price.

### TS-033 — Ask for the price after selecting product attributes

Verify that the chatbot returns the price for the exact selected configuration.

### TS-034 — Recheck the same product price

Ask for the price multiple times during the conversation and verify consistency.

---

## 9. Purchase Intent

### TS-035 — Express purchase intent

Example:

> I want to buy it.

Verify that the chatbot recognizes that the user wants to purchase the product.

### TS-036 — Ask how to order

Verify that the chatbot explains the purchase process clearly.

### TS-037 — Ask for a product link

Verify that the chatbot provides a valid product link when appropriate.

### TS-038 — Ask about payment methods

Verify that the chatbot provides correct information about available payment methods.

### TS-039 — Ask about cash payment

Verify that the chatbot distinguishes between physical-store payment and online payment.

### TS-040 — Ask about pickup

Verify that the chatbot does not guarantee store pickup without confirming product availability.

### TS-041 — Continue purchase conversation after selecting a product

Verify that the chatbot maintains the selected product and its attributes throughout the purchase flow.

---

## 10. Operator Handoff

### TS-042 — Request a human operator

Verify that the chatbot correctly transfers the conversation to an operator.

### TS-043 — Continue sending messages after requesting an operator

Verify that the system clearly indicates the current operator state.

### TS-044 — Try to return to the chatbot after requesting an operator

Verify that the user can understand how to return to AI chatbot mode, if this functionality is supported.

### TS-045 — Close the chat while waiting for an operator

Verify that reopening the chat preserves the correct state.

### TS-046 — Refresh the page while waiting for an operator

Verify that the operator/chat state remains consistent after refresh.

---

## 11. Chat State and Reopening

### TS-047 — Minimize the chat

Verify that minimizing the chat does not unexpectedly change the conversation state.

### TS-048 — Reopen the minimized chat

Verify that the conversation and current state are displayed correctly.

### TS-049 — Reopen the chat without refreshing the page

Verify that the system does not remain stuck in an incorrect state.

### TS-050 — Start a new conversation after an old conversation

Verify that the user can start a fresh conversation when appropriate.

---

## 12. Error Handling

### TS-051 — Send random numbers

Example:

> 123456789

Verify that the chatbot handles irrelevant input gracefully.

### TS-052 — Send special characters

Example:

> 22@@@@@@@

Verify that the chatbot does not crash or produce unexpected behavior.

### TS-053 — Send emojis

Verify that the chatbot handles emoji-only messages.

### TS-054 — Send meaningless text

Verify that the chatbot responds appropriately to unclear input.

### TS-055 — Send a request while the system is unavailable

Verify that the maintenance/error message is displayed correctly and that the user can continue once the service becomes available.

---

## 13. Language and Mixed-Language Input

### TS-056 — Ask questions in English

Verify that English queries are understood correctly.

### TS-057 — Ask questions in Georgian

Verify that Georgian queries are understood correctly.

### TS-058 — Mix languages in one message

Example:

> Hello გამარჯობა Hola Bonjour

Verify that the chatbot handles mixed-language input without losing the user's intent.

### TS-059 — Switch language during an existing conversation

Verify that changing language does not incorrectly reset or change product context.

### TS-060 — Check language consistency in responses

Verify that the chatbot responds in the expected language according to the conversation or selected UI language.

---

## 14. Branch and Store Information

### TS-061 — Ask where stores are located

Verify that the chatbot handles store-location requests according to the available system information and integration limitations.

### TS-062 — Ask for a specific store location

Example:

> Is there a store in Vake?

Verify that the chatbot does not provide unsupported or unverified branch information.

### TS-063 — Ask for store phone numbers

Verify that the chatbot does not provide unsupported contact information when the required integration/data source is unavailable.

---

## 15. Conversation Robustness

### TS-064 — Change topic several times

Example:

> Laptop → phone → laptop → store → purchase.

Verify that the chatbot correctly handles topic changes.

### TS-065 — Return to a previous topic

Verify that the chatbot can return to an earlier product discussion when context is still available.

### TS-066 — Ask many questions in one message

Verify that the chatbot addresses all important questions or clearly separates them.

### TS-067 — Continue a long conversation

Verify that the chatbot maintains relevant context during a long conversation.

### TS-068 — Repeat the same question

Verify that repeated questions receive consistent and relevant answers.

### TS-069 — Ask an ambiguous question

Example:

> Which one?

Verify that the chatbot asks for clarification instead of guessing.

### TS-070 — Provide contradictory information

Example:

> I want black. Actually I want silver.

Verify that the chatbot uses the latest requirement correctly.

---

## 16. Accuracy and Consistency

### TS-071 — Compare chatbot information with the website

Verify important product information against the available product page.

Check:

- Product name
- Price
- Color
- RAM
- Storage
- Warranty
- Availability
- Product link

### TS-072 — Ask the same question at different points in the conversation

Verify that the chatbot does not provide conflicting information.

### TS-073 — Verify selected product attributes

Verify that the chatbot does not mix attributes from different products.

### TS-074 — Verify product link accuracy

Verify that links provided by the chatbot open the correct product page.

---

## 17. Exploratory Testing

### TS-075 — Explore unexpected user behavior

Use natural, incomplete, informal, misspelled, or unusual messages to identify unexpected chatbot behavior.

Examples:

- Very short messages
- Long messages
- Multiple questions
- Mixed languages
- Emojis
- Numbers
- Special characters
- Contradictory requirements
- Sudden topic changes

### TS-076 — Stress the conversation with many follow-up questions

Continue asking related and unrelated questions to determine whether the chatbot loses context.

### TS-077 — Try to break the conversation flow

Rapidly switch between:

- AI chatbot
- Operator
- Product search
- Purchase intent
- Store questions
- New product requests

Verify that the chatbot remains in a valid state.

---

## 18. Mobile and Desktop Testing

### TS-078 — Test chatbot on desktop

Verify the chatbot UI, conversation flow, input field, messages, links, and operator state on a desktop browser.

### TS-079 — Test chatbot on mobile

Verify the same functionality on a mobile device.

### TS-080 — Minimize and reopen chatbot on mobile

Verify that conversation state and UI behave correctly.

### TS-081 — Test long conversations on mobile

Verify that scrolling, message display, input field, and conversation history remain usable.

### TS-082 — Test chatbot during orientation changes

Verify behavior when switching between portrait and landscape mode, if supported.

---

## 19. Usability

### TS-083 — Verify clarity of chatbot responses

Responses should be understandable and relevant to the user's question.

### TS-084 — Verify useful clarification questions

When the request is unclear or contains conflicting requirements, the chatbot should ask useful clarification questions.

### TS-085 — Verify purchase flow guidance

When the user clearly wants to purchase a product, the chatbot should provide clear next steps.

### TS-086 — Verify error messages

Error and maintenance messages should be understandable and should not leave the user confused about what to do next.

---

## 20. Regression Testing

### TS-087 — Retest fixed chatbot defects

Verify that previously reported defects are resolved without introducing new problems.

### TS-088 — Retest related functionality after a fix

After a chatbot defect is fixed, test related conversation flows to check for regression.

### TS-089 — Verify behavior across desktop and mobile after fixes

Verify that fixes work consistently on both supported device types.

---

# Exploratory Testing Focus

During exploratory testing, special attention should be given to:

- Context loss
- Wrong product selection
- Incorrect prices
- Product attribute mixing
- Unsupported store information
- Incorrect product recommendations
- Purchase-flow problems
- Operator handoff problems
- Chat state problems
- Language switching
- Mixed-language input
- Long conversations
- Conflicting requirements
- Multiple questions in one message
- Error and maintenance states
- Mobile-specific behavior

The main goal is not only to verify predefined requirements, but also to discover unexpected behavior that may affect the user experience, product accuracy, or purchase journey.
