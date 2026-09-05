# Test Execution Report — AI-Powered E-commerce Chatbot

## 1. Overview

I performed manual and exploratory testing of an AI-powered e-commerce chatbot.

The testing focused on realistic customer conversations rather than only happy-path questions.

The main areas tested included:

* Product search
* Product information
* Product recommendations
* Product comparison
* Purchase intent
* Operator handoff
* Conversation state
* Language switching
* Complex and ambiguous user requests

> **Confidentiality Note:** Specific application, organization, website, product, and business information has been generalized or excluded from this portfolio.

---

## 2. Test Environment

* **Application:** Confidential AI-Powered E-commerce Chatbot
* **Testing Type:** Manual / Exploratory Testing
* **Platform:** Web
* **Languages Tested:** English and Georgian
* **Product Categories:** Laptops and Smartphones

---

## 3. Test Execution Summary

| Area                            | Result                        |
| ------------------------------- | ----------------------------- |
| Laptop product search           | Tested                        |
| Cheapest product search         | Tested                        |
| Price questions                 | Tested                        |
| RAM questions                   | Tested                        |
| Color questions                 | Tested                        |
| Gaming requirements             | Tested                        |
| Complex product requirements    | Defect found                  |
| Product comparison              | Defect found                  |
| Product price consistency       | Defect found                  |
| Product links                   | Tested                        |
| Purchase intent                 | Improvement / defect observed |
| Payment questions               | Tested                        |
| Pickup / availability questions | Tested                        |
| Operator handoff                | Tested                        |
| Returning from operator mode    | Defect found                  |
| Minimize and reopen chat        | Defect found                  |
| Conversation context            | Tested                        |
| Topic switching                 | Tested                        |
| Mixed-language input            | Tested                        |
| Store information               | Requirement concern found     |
| System maintenance behavior     | Observed                      |
| Product material questions      | Tested                        |
| Ambiguous questions             | Tested                        |

---

# 4. Detailed Execution Results

## 4.1 Laptop Search

**Test:**

`I want a laptop under 1200 GEL`

**Observed Result:**

The chatbot provided laptop recommendations and asked about preferred brand or screen size.

**Result:** Pass

No defect was observed during this test.

---

## 4.2 Cheapest Laptop

**Test:**

`Which one is the cheapest?`

**Observed Result:**

The chatbot provided a cheapest laptop recommendation and price.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.3 RAM Information

**Test:**

`How much RAM does it have?`

**Observed Result:**

The chatbot provided RAM information for the discussed laptops.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.4 Laptop Colors

**Test:**

`What colors does it come in?`

**Observed Result:**

The chatbot provided available color options.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.5 Gaming Requirement

**Test:**

`I need a laptop for gaming`

**Observed Result:**

The chatbot recognized the gaming requirement and suggested appropriate laptop options.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.6 Complex Product Requirements

**Test:**

`color RAM price design material battery warranty gaming office`

**Observed Result:**

The chatbot focused mainly on RAM and asked:

`Which RAM capacity would be your priority?`

The other requirements were not properly addressed.

**Result:** Fail

**Related Bug:** BUG-005

---

## 4.7 Conflicting Requirements

**Test:**

`want a laptop under 1000 GEL and high performance`

Then:

`cheap but gaming laptop`

**Observed Result:**

The chatbot could not provide a clear matching product and suggested operator assistance.

**Result:** Needs Improvement

This behavior was useful for exploratory testing, but it was not classified as a confirmed defect without a clearly defined product or business requirement.

---

## 4.8 Product Comparison

**Test:**

`Compare Product A and Product B`

**Observed Result:**

The chatbot compared the requested first product with a different second product instead of the product specified by the user.

**Result:** Fail

**Related Bug:** BUG-004

> Specific real product names have been generalized for portfolio confidentiality.

---

## 4.9 Follow-up Comparison Question

**Test:**

`Which one has a better camera?`

**Observed Result:**

The chatbot continued the comparison using the incorrect product context established during the previous response.

**Result:** Fail

**Related Bug:** BUG-004

---

## 4.10 Product Price

**Test:**

`What is the price?`

**Observed Result:**

The chatbot provided a product price that differed from the price displayed on the corresponding product page.

**Result:** Fail

**Related Bug:** BUG-001

---

## 4.11 Product Link

**Test:**

Asked the chatbot to provide a link for the selected product.

**Observed Result:**

The chatbot provided a product link that opened the corresponding product page.

However, the price displayed on the product page did not match the price provided by the chatbot.

**Result:** Partial / Fail

**Related Bug:** BUG-001

---

## 4.12 Purchase Intent

**Test:**

`Let's buy the laptop`

and:

`I want to buy it`

**Observed Result:**

The chatbot recognized the purchase intent and explained that the user could continue through the product page, cart, or available payment options.

However, it did not move into a structured checkout flow with a clear product summary and confirmation.

**Result:** Needs Improvement

This was documented as a UX / recommendation rather than a confirmed functional defect.

---

## 4.13 Payment Method

**Test:**

`Can I pay cash?`

**Observed Result:**

The chatbot explained the available payment options.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.14 Pickup / Availability

**Test:**

`Can I pick it up tomorrow?`

**Observed Result:**

The chatbot indicated that pickup could depend on product availability and asked for additional information.

**Result:** Needs Verification

The chatbot did not verify real-time stock availability during this conversation.

---

## 4.15 Operator Handoff

**Test:**

`Connect me to operator`

**Observed Result:**

The system confirmed that the request had been sent to an operator.

**Result:** Pass

The operator request was successfully submitted.

---

## 4.16 Return to AI After Operator Request

**Test:**

After requesting an operator:

`Never mind. Can you return to chatbot?`

**Observed Result:**

The system indicated that an operator had already been requested.

The user could not return to the AI chatbot through the conversation.

**Result:** Fail

**Related Bug:** BUG-002

---

## 4.17 Minimize and Reopen Chat

**Test:**

1. Request an operator.
2. Minimize the chatbot.
3. Reopen the chatbot.
4. Continue the conversation.

**Observed Result:**

The chatbot remained in the previous operator state.

Refreshing the page changed the behavior, but minimizing and reopening the chat did not reset the conversation state.

**Result:** Fail

**Related Bug:** BUG-003

---

## 4.18 Topic Switching

**Test:**

`I want a laptop`

Then:

`Actually show me phones`

**Observed Result:**

The chatbot switched from laptops to phones.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.19 Multiple Topics in One Conversation

**Test:**

Laptop questions → phone comparison → laptop → phones → store information → purchase.

**Observed Result:**

The chatbot was able to continue the conversation, but longer conversations created situations where context and product selection required closer verification.

**Result:** Exploratory Observation

---

## 4.20 Store Information

**Test:**

`Where is your store?`

**Observed Result:**

The chatbot provided specific store information.

**Result:** Requirement Concern

The expected behavior for store information should be verified against the defined chatbot capabilities and available integrations.

This was treated as a requirement/business-rule concern rather than a confirmed technical defect.

---

## 4.21 Material Question

**Test:**

`silver material?`

**Observed Result:**

The chatbot distinguished between color and material and explained that laptops could use materials such as aluminum or plastic.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.22 Multiple Attribute Question

**Test:**

`silver material? design? color? RAM? price?`

**Observed Result:**

The chatbot provided information about several requested attributes and then asked which brand was preferred.

**Result:** No Confirmed Defect

---

## 4.23 Product Memory

**Test:**

After discussing a specific laptop:

`What I chose?`

**Observed Result:**

The chatbot identified the product configuration discussed earlier in the conversation.

**Result:** Pass

No defect was confirmed during this test.

---

## 4.24 Mixed Language

**Test:**

The conversation was switched between English and Georgian.

**Observed Result:**

The chatbot continued responding and understood the general conversation.

**Result:** Pass

No confirmed defect was observed.

---

## 4.25 System Maintenance

**Test:**

During some messages, the chatbot displayed a system maintenance message.

**Observed Result:**

The maintenance message appeared during testing and the chatbot became available again later.

**Result:** Observed

This was not automatically classified as a chatbot defect because the system may genuinely have been temporarily unavailable.

---

# 5. Confirmed / Documented Bugs

The following issues were documented as separate bug reports:

| Bug ID  | Issue                                                                    | Result |
| ------- | ------------------------------------------------------------------------ | ------ |
| BUG-001 | Chatbot price differs from product page                                  | Fail   |
| BUG-002 | User cannot clearly return from operator mode                            | Fail   |
| BUG-003 | Operator state remains after minimize/reopen                             | Fail   |
| BUG-004 | Requested product is replaced with a different product during comparison | Fail   |
| BUG-005 | Multiple product requirements are not properly handled                   | Fail   |

Detailed reproduction steps, expected results, actual results, and severity/priority information are available in the `Bug-Reports` folder.

---

# 6. Recommendations / Improvements

During testing, several areas were identified that may require product or UX improvements.

## Purchase Flow

The chatbot recognizes purchase intent but could provide a more structured path toward checkout.

## Complex Requests

The chatbot could improve how it processes multiple requirements within a single user message.

## Store Information

The expected behavior for store information should be confirmed based on available integrations and business requirements.

## Pickup Availability

The chatbot should provide availability information only when current stock data is available.

---

# 7. QA Conclusion

The chatbot successfully handled many basic product-related questions.

The most important issues identified during exploratory testing were related to:

* Data consistency
* Product identity
* Conversation state
* Operator handoff
* Complex user intent
* Product comparison
* Price consistency

The testing also demonstrated that AI-powered conversational systems require testing beyond simple question-and-answer scenarios.

Long conversations, changing requirements, product comparisons, purchase intent, and transitions between AI and human support can expose issues that may not be visible during basic functional testing.

This project demonstrates practical skills in:

* Manual Testing
* Exploratory Testing
* Functional Testing
* Negative Testing
* Conversational Testing
* Context and State Testing
* Defect Identification
* Bug Reporting
* Requirement-based thinking
* QA Documentation

