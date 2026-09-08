# Exploratory Testing — AI E-commerce Chatbot

## 1. Overview

Exploratory testing was performed to evaluate the AI e-commerce chatbot in situations that are difficult to cover through predefined test cases alone.

The main goal was to simulate realistic customer behavior and investigate how the chatbot handles:

* changing requirements
* follow-up questions
* multiple requirements in one message
* conflicting requirements
* product comparisons
* product recommendations
* purchase intent
* operator handoff
* conversation state
* topic switching
* ambiguous input
* invalid input
* mixed-language conversations
* product information consistency
* unexpected user behavior

Exploratory testing was performed alongside structured functional testing and was used to identify additional risks, observations, and defects.

---

## 2. QA Role

**Role:** Junior Manual QA Tester

The exploratory testing was performed from a customer-focused manual QA perspective, with emphasis on:

* functional behavior
* conversation context
* state management
* product information accuracy
* requirement handling
* usability
* error handling
* data consistency
* realistic user behavior

---

## 3. Exploratory Testing Approach

The testing was based on short exploratory sessions rather than a fixed sequence of predefined test cases.

During each session, I:

1. Started with a realistic customer request.
2. Observed the chatbot response.
3. Changed or extended the requirement.
4. Introduced unexpected or ambiguous input where appropriate.
5. Checked whether previous conversation context was handled correctly.
6. Compared chatbot information with available product information when applicable.
7. Recorded observations and reproducible defects.
8. Created or linked defect reports when the behavior represented a confirmed issue.

### Exploratory Techniques Used

* Free-form exploration
* Scenario variation
* Follow-up questioning
* Boundary and negative exploration
* Context switching
* State transition testing
* Requirement combination
* Product comparison
* Data consistency checks
* Error handling exploration
* Usability observation

---

# 4. Exploratory Charters

## Charter 01 — Product Context and Follow-up Questions

### Mission

Investigate whether the chatbot maintains product context when the customer asks several follow-up questions.

### Starting Point

The conversation starts with a general laptop request.

### Actions

The conversation was extended with questions about:

* price
* RAM
* color
* design
* material
* warranty
* gaming performance
* battery
* office usage

### Expected Behavior

The chatbot should:

* maintain the relevant product context
* understand follow-up questions
* use previously provided information
* avoid losing important requirements
* ask for clarification when the request is unclear

### Findings

The chatbot generally maintained the conversation context, but complex requests could sometimes be simplified too much.

In some situations, the response focused on one attribute instead of considering all requested requirements.

### QA Assessment

**Risk:** Medium

This behavior can reduce recommendation quality when customers provide several important requirements at the same time.

### Related Coverage

* Test Scenarios: TS-005, TS-015–020, TS-021–025
* Test Cases: TC-005, TC-006, TC-015–019, TC-020–024
* Related defect: BUG-005

---

# 5. Exploratory Charter 02 — Complex and Multiple Requirements

## Mission

Investigate how the chatbot handles multiple product requirements provided in a single message.

### Example Request

```text
color RAM price design material battery warranty gaming office
```

### What Was Checked

The investigation focused on whether the chatbot could:

* identify all requested attributes
* preserve the complete requirement
* prioritize requirements appropriately
* ask clarification questions
* provide a useful recommendation
* avoid silently ignoring requirements

### Expected Behavior

The chatbot should consider the complete request or clearly communicate when some requirements cannot be satisfied.

### Finding

The chatbot sometimes focused on only one attribute, such as RAM, while giving less attention to the remaining requirements.

### Assessment

**Result:** Confirmed functional issue when important requirements were ignored.

**Related Defect:** BUG-005

---

# 6. Exploratory Charter 03 — Conflicting Requirements

## Mission

Investigate chatbot behavior when customer requirements are difficult or impossible to satisfy simultaneously.

### Example Requests

```text
I want a laptop under 1000 GEL and high performance
```

```text
cheap but gaming laptop
```

### Expected Behavior

The chatbot should:

* recognize conflicting or difficult requirements
* explain the limitation
* propose reasonable alternatives
* ask which requirement is more important when necessary

### Observation

The chatbot sometimes moved directly toward another recommendation or operator assistance instead of clearly explaining the trade-off.

### QA Assessment

**Risk:** Medium

The behavior may create confusion and reduce the usefulness of the recommendation process.

---

# 7. Exploratory Charter 04 — Product Comparison

## Mission

Verify whether the chatbot compares exactly the products requested by the customer.

### Example Request

```text
Compare iPhone 16 and Samsung S24
```

### Expected Behavior

The chatbot should compare:

* iPhone 16
* Samsung S24

The requested product models should not be silently replaced.

### Observation

The chatbot responded with a comparison involving:

* iPhone 16
* Samsung Galaxy S26

instead of the requested Samsung S24.

### Assessment

**Result:** Confirmed defect

### Related Defect

**BUG-004 — Requested product replaced during comparison**

### Risk

Incorrect product substitution can lead to misleading recommendations and incorrect purchase decisions.

### Related Coverage

* Test Scenarios: TS-026–030
* Test Cases: TC-025–028
* Test Execution: comparison-related failures

---

# 8. Exploratory Charter 05 — Product Information Consistency

## Mission

Investigate whether product information provided by the chatbot matches the information available on the linked product page.

### Actions

1. Ask the chatbot for a specific product.
2. Record the product name and price.
3. Request or open the product link.
4. Compare the chatbot information with the product page.

### Checked Information

* Product name
* Model
* Color
* RAM
* Storage
* Price

### Expected Behavior

Information presented by the chatbot should correspond to the selected product page.

### Finding

A price inconsistency was identified between the chatbot response and the product page.

### Assessment

**Result:** Confirmed defect

### Related Defect

**BUG-001 — Product price inconsistency**

### Risk

Price inconsistency is a high-value customer-facing issue because price directly influences purchase decisions.

---

# 9. Exploratory Charter 06 — Product Link Verification

## Mission

Investigate whether product links provided by the chatbot lead to the correct product and preserve the expected product information.

### Actions

The selected product was requested from the chatbot, followed by a request for its product link.

The linked page was then compared against the information previously provided by the chatbot.

### Expected Behavior

The link should open the correct product page.

The product details should be consistent with the chatbot response.

### Finding

The product page opened, but the displayed price did not match the price previously provided in the conversation.

### Assessment

**Result:** Related to confirmed product information consistency issue.

### Related Defect

**BUG-001**

---

# 10. Exploratory Charter 07 — Purchase Intent

## Mission

Investigate how the chatbot behaves when the customer clearly indicates an intention to purchase.

### Example Requests

```text
I want to buy it
```

```text
Let's buy the laptop
```

```text
I decided to buy it
```

### Expected Behavior

The chatbot should recognize purchase intent and provide clear next steps.

Where applicable, the response should help the customer understand:

* which product was selected
* what action should be taken next
* how to continue the purchase

### Observation

The chatbot generally recognized purchase intent.

However, the conversation did not always move into a clearly structured purchase flow.

For example, the chatbot could direct the customer toward the website cart without always providing a clear summary of the selected product and next step.

### QA Assessment

**Result:** Improvement opportunity

This observation was not automatically treated as a confirmed functional defect because the expected purchase flow may depend on the application's intended design.

---

# 11. Exploratory Charter 08 — Operator Handoff

## Mission

Investigate the transition from AI chatbot to human operator.

### Example Request

```text
Connect me to operator
```

### Expected Behavior

The chatbot should:

* recognize the operator request
* transition to the appropriate state
* communicate the transition clearly
* prevent contradictory chatbot behavior during operator interaction

### Observation

The operator handoff worked, but the transition created a state-management risk when the customer attempted to return to the AI chatbot.

---

# 12. Exploratory Charter 09 — Return from Operator State

## Mission

Investigate whether the user can return to the AI chatbot after requesting an operator.

### Actions

After requesting an operator, the following type of message was tested:

```text
Never mind. Can you return to chatbot?
```

### Expected Behavior

If the product supports returning to AI chat, the user should be able to return clearly and without restarting the entire experience.

### Finding

The chatbot remained in the operator-related state and indicated that an operator had already been requested.

### Assessment

**Result:** Confirmed defect

### Related Defect

**BUG-002 — Unable to return from operator mode**

### Risk

The user may become trapped in a state that does not provide a clear recovery path.

---

# 13. Exploratory Charter 10 — Minimize and Reopen

## Mission

Investigate whether minimizing and reopening the chatbot changes or preserves the current conversation state.

### Actions

1. Move the conversation into the operator state.
2. Minimize the chat.
3. Reopen the chat.
4. Observe the resulting state.

### Expected Behavior

The behavior should be consistent with the intended chat-state design.

The user should have a clear understanding of whether the conversation is:

* active
* paused
* closed
* waiting for an operator
* available for AI interaction

### Finding

After minimizing and reopening the chatbot, the previous operator state remained.

Refreshing the page produced different behavior.

### Assessment

**Result:** Confirmed state-management issue

### Related Defect

**BUG-003 — Operator state persists after minimize/reopen**

---

# 14. Exploratory Charter 11 — Topic Switching

## Mission

Investigate whether the chatbot correctly handles changes in topic during a single conversation.

### Example Flow

```text
Tell me about laptops
```

Then:

```text
Show me phones
```

Then:

```text
Where is your store?
```

Then:

```text
Let's buy the laptop
```

### Expected Behavior

The chatbot should:

* understand the latest request
* preserve only relevant context
* avoid mixing unrelated topics
* correctly handle a return to a previous topic

### Observation

Topic switching generally worked, but long conversations created a potential risk of context mixing.

### QA Assessment

**Risk:** Medium

This area should remain part of regression and exploratory testing because AI conversation state can change depending on the sequence and wording of requests.

---

# 15. Exploratory Charter 12 — Ambiguous Follow-up Questions

## Mission

Investigate whether the chatbot asks for clarification when a short follow-up can refer to multiple possible products or topics.

### Example Inputs

```text
Which one?
```

```text
What about it?
```

### Expected Behavior

If multiple possible references exist, the chatbot should ask the user to clarify instead of making an unsupported assumption.

### Observation

Ambiguous follow-up questions were treated as an area requiring continued observation.

### QA Assessment

**Risk:** Medium

Ambiguous context is particularly important in conversational applications because an incorrect assumption may lead to an incorrect recommendation.

---

# 16. Exploratory Charter 13 — Mixed-Language Conversation

## Mission

Investigate whether the chatbot can maintain a conversation when the user switches between languages.

### Example

```text
Hello გამარჯობა Hola Bonjour
```

Additional exploration included switching between English and Georgian during the same conversation.

### Expected Behavior

The chatbot should:

* understand the user's request
* maintain the conversation context
* respond consistently
* preserve expected product terminology

### Observation

The chatbot generally continued the conversation successfully.

However, product or category names could appear in Georgian while the conversation was otherwise being conducted in English.

### QA Assessment

**Risk:** Low to Medium

The behavior should be evaluated against the application's intended localization requirements.

---

# 17. Exploratory Charter 14 — Invalid and Random Input

## Mission

Investigate how the chatbot handles unexpected or meaningless input.

### Example Inputs

```text
123456789
```

```text
22@@@@@@@
```

### Expected Behavior

The chatbot should:

* handle invalid input gracefully
* provide a useful fallback response
* avoid crashing
* avoid entering an invalid state
* allow the user to continue the conversation

### Observation

Invalid and random inputs were included as part of negative exploratory coverage.

No automatic defect was assigned without a reproducible functional failure.

---

# 18. Exploratory Charter 15 — Product Substitution

## Mission

Investigate whether the chatbot silently changes the product requested by the customer.

### Example

```text
Compare iPhone 16 and Samsung S24
```

### Expected Behavior

The exact requested models should be used.

If a requested product cannot be found, the chatbot should clearly communicate the limitation or ask whether the user wants an alternative.

### Finding

The chatbot substituted Samsung S24 with Samsung Galaxy S26.

### Assessment

**Result:** Confirmed defect

### Related Defect

**BUG-004**

### QA Importance

Silent product substitution is particularly important because the customer may believe the comparison represents the products they originally requested.

---

# 19. Exploratory Charter 16 — Long Conversation and Context Stability

## Mission

Investigate whether conversation quality remains stable after multiple requests and topic changes.

### Exploration Areas

The conversation was extended through combinations of:

* product search
* follow-up questions
* comparisons
* purchase intent
* topic changes
* store information
* operator request
* return attempts

### Expected Behavior

The chatbot should maintain a predictable conversation state and avoid mixing information from unrelated earlier requests.

### Observation

The chatbot generally continued the conversation, but long conversations increased the risk of:

* context mixing
* incorrect product references
* unclear follow-up interpretation
* state-related inconsistencies

### QA Assessment

**Risk:** Medium

Long-context behavior should remain part of regression and exploratory testing.

---

# 20. Exploratory Charter 17 — Requirement Changes During Conversation

## Mission

Investigate how the chatbot reacts when the customer changes one or more requirements after receiving a recommendation.

### Example Flow

```text
I need a laptop under 1000 GEL
```

Then:

```text
Actually, I can spend up to 1500 GEL
```

Then:

```text
Gaming performance is more important than price
```

### Expected Behavior

The chatbot should:

* recognize the updated requirement
* stop relying on outdated constraints where appropriate
* provide a new recommendation
* preserve still-valid requirements

### QA Assessment

**Risk:** Medium

Changing requirements is a realistic user behavior and should be covered during future regression cycles.

---

# 21. Exploratory Charter 18 — State Recovery

## Mission

Investigate whether the chatbot provides a clear recovery path after unusual conversation states.

### Areas Explored

* operator state
* minimized chat
* reopened chat
* topic changes
* ambiguous questions
* invalid input
* changed product requirements

### Expected Behavior

The user should always have a clear way to continue or recover the conversation.

### Finding

Operator-related state handling showed the strongest recovery risk.

### Related Defects

* BUG-002
* BUG-003

---

# 22. Exploratory Findings Classification

Exploratory findings were classified into three categories.

## Confirmed Defect

A reproducible behavior that does not meet the expected functional behavior.

Examples:

* Product price inconsistency — BUG-001
* Unable to return from operator mode — BUG-002
* Operator state after minimize/reopen — BUG-003
* Incorrect product substitution — BUG-004
* Multiple requirements not properly handled — BUG-005

## Observation

A behavior that may represent a risk or usability concern but does not have enough evidence to classify it as a confirmed defect.

Examples:

* Ambiguous question handling
* Long conversation context stability
* Purchase-flow structure
* Mixed-language terminology
* Conflicting requirements

## Improvement Opportunity

A behavior that may be acceptable from a functional perspective but could provide a better user experience.

Examples:

* clearer purchase next steps
* clearer explanation of conflicting requirements
* clearer recovery from certain conversation states

---

# 23. Confirmed Defects Identified Through Exploration

| Bug ID  | Area                 | Finding                                            | Severity | Priority |
| ------- | -------------------- | -------------------------------------------------- | -------- | -------- |
| BUG-001 | Product Information  | Chatbot price differs from product page            | Medium   | High     |
| BUG-002 | Operator State       | User cannot clearly return from operator mode      | High     | High     |
| BUG-003 | Conversation State   | Operator state remains after minimize/reopen       | Medium   | High     |
| BUG-004 | Product Comparison   | Requested product is replaced by another model     | High     | High     |
| BUG-005 | Complex Requirements | Multiple requirements are not consistently handled | High     | High     |

---

# 24. Exploratory Testing Risk Areas

The following areas were considered the highest-risk areas during exploration:

### 1. Conversation Context

The chatbot must correctly maintain and update context as the conversation changes.

### 2. Product Accuracy

Product name, model, price, and other attributes should remain consistent.

### 3. Requirement Handling

Multiple customer requirements should not be silently ignored.

### 4. Product Comparison

The chatbot should compare the exact products requested.

### 5. State Management

Operator, minimized, reopened, and active conversation states should behave predictably.

### 6. Purchase Flow

Purchase intent should lead to clear and useful next steps.

### 7. Error Handling

Unexpected input should not cause broken or confusing conversation states.

---

# 25. Exploratory Testing Coverage

| Area                      | Explored | Result                      |
| ------------------------- | -------- | --------------------------- |
| Product Search            | Yes      | Generally functional        |
| Product Context           | Yes      | Risk identified             |
| Follow-up Questions       | Yes      | Generally functional        |
| Multiple Requirements     | Yes      | Defect identified           |
| Conflicting Requirements  | Yes      | Observation                 |
| Product Comparison        | Yes      | Defect identified           |
| Product Price Consistency | Yes      | Defect identified           |
| Product Links             | Yes      | Related consistency issue   |
| Purchase Intent           | Yes      | Improvement opportunity     |
| Operator Handoff          | Yes      | Functional with state risks |
| Return from Operator      | Yes      | Defect identified           |
| Minimize/Reopen           | Yes      | Defect identified           |
| Topic Switching           | Yes      | Observation                 |
| Ambiguous Input           | Yes      | Risk identified             |
| Mixed Languages           | Yes      | Observation                 |
| Invalid Input             | Yes      | Explored                    |
| Long Conversations        | Yes      | Risk identified             |
| Requirement Changes       | Yes      | Risk identified             |

---

# 26. Relationship to Structured Testing

Exploratory testing complemented the predefined test cases.

The structured test cases were used to verify known expected behavior consistently, while exploratory testing was used to investigate:

* unexpected combinations
* alternative user wording
* context changes
* state transitions
* realistic customer behavior
* edge cases
* potential usability problems

Findings from exploratory testing were then connected to the formal defect documentation where appropriate.

---

# 27. Traceability

| Exploratory Area          | Related Test Coverage     | Related Defect          |
| ------------------------- | ------------------------- | ----------------------- |
| Complex requirements      | TS-021–025 / TC-020–024   | BUG-005                 |
| Product comparison        | TS-026–030 / TC-025–028   | BUG-004                 |
| Product price consistency | Product information tests | BUG-001                 |
| Operator return           | TS-035–040 / TC-033–036   | BUG-002                 |
| Minimize/reopen           | TS-035–040 / TC-033–036   | BUG-003                 |
| Topic switching           | TS-015–020 / TC-015–019   | Observation             |
| Purchase intent           | TS-031–034 / TC-029–032   | Improvement opportunity |
| Mixed language            | TS-046–049 / TC-041–044   | Observation             |
| Invalid input             | TS-041–045 / TC-037–040   | Exploratory coverage    |

---

# 28. Limitations

The exploratory testing was performed as manual black-box testing.

The following areas were outside the scope of this exploration:

* source code review
* database validation
* API testing
* automated testing
* performance/load testing
* security penetration testing
* internal AI model evaluation
* backend architecture validation

The exact behavior of AI-generated responses can vary depending on wording and conversation context. Therefore, exploratory findings should be reproduced before being treated as confirmed defects.

---

# 29. Key QA Findings

The exploratory sessions demonstrated that the chatbot can support common product-search and conversation flows, but several areas require additional attention.

The most important findings were:

1. Complex requirements are not always handled completely.
2. Product information can become inconsistent between chatbot responses and product pages.
3. The chatbot can substitute a requested product with another model.
4. Purchase intent is recognized, but the next-step flow could be clearer.
5. Operator state handling can prevent a clear return to the AI chatbot.
6. Conversation state can remain after minimizing and reopening the chatbot.
7. Long and changing conversations create additional context-management risks.

---

# 30. QA Conclusion

Exploratory testing provided additional coverage beyond predefined functional test cases and helped identify defects related to:

* product information accuracy
* product comparison
* complex requirements
* conversation state
* operator state

The most significant risks are related to **conversation context, product accuracy, and state management**.

Further regression testing should focus on the confirmed defects after fixes are implemented, especially:

* BUG-001
* BUG-002
* BUG-003
* BUG-004
* BUG-005

Exploratory testing should also remain part of future QA cycles because conversational AI behavior can vary significantly depending on user wording, context, and sequence of interactions.
