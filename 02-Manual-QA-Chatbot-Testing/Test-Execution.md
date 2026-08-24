# Test Execution Report — AI E-commerce Chatbot

## Overview

I performed manual and exploratory testing of an AI-powered e-commerce
chatbot.

The testing was based on realistic customer conversations rather than only
happy-path questions.

I tested product search, product information, recommendations, product
comparison, purchase intent, operator handoff, conversation state, language
switching, and more complex user requests.

---

## Test Environment

- Application: AI E-commerce Chatbot
- Testing type: Manual / Exploratory Testing
- Platform: Web
- Main languages tested: English and Georgian
- Product categories tested: Laptops and Smartphones

---

## What I Tested

| Area | Result |
|---|---|
| Laptop product search | Tested |
| Cheapest product search | Tested |
| Price questions | Tested |
| RAM questions | Tested |
| Color questions | Tested |
| Gaming requirements | Tested |
| Complex product requirements | Defect found |
| Product comparison | Defect found |
| Product price consistency | Defect found |
| Product links | Tested |
| Purchase intent | Improvement / defect observed |
| Payment questions | Tested |
| Pickup / availability questions | Tested |
| Operator handoff | Tested |
| Returning from operator mode | Defect found |
| Minimize and reopen chat | Defect found |
| Conversation context | Tested |
| Topic switching | Tested |
| Mixed-language input | Tested |
| Store information | Requirement concern found |
| System maintenance behavior | Observed |
| Product material questions | Tested |
| Ambiguous questions | Tested |

---

# Detailed Execution Results

## 1. Laptop Search

**Test:**  
`I want a laptop under 1200 GEL`

**Observed result:**  
The chatbot provided laptop brands and asked about preferred brand or screen
size.

**Result:** Pass / No defect observed during this test.

---

## 2. Cheapest Laptop

**Test:**  
`Which one is the cheapest?`

**Observed result:**  
The chatbot provided a cheapest laptop recommendation and price.

**Result:** Pass / No defect confirmed during this test.

---

## 3. RAM Information

**Test:**  
`How much RAM does it have?`

**Observed result:**  
The chatbot provided RAM information for the discussed laptops.

**Result:** Pass / No defect confirmed during this test.

---

## 4. Laptop Colors

**Test:**  
`What colors does it come in?`

**Observed result:**  
The chatbot provided available color options.

**Result:** Pass / No defect confirmed during this test.

---

## 5. Gaming Requirement

**Test:**  
`I need a laptop for gaming`

**Observed result:**  
The chatbot recognized the gaming requirement and suggested gaming laptop
brands.

**Result:** Pass / No defect confirmed during this test.

---

## 6. Complex Product Requirements

**Test:**

`color RAM price design material battery warranty gaming office`

**Observed result:**

The chatbot focused mainly on RAM and asked:

`Which RAM capacity would be your priority?`

The other requirements were not properly addressed.

**Result:** Fail

**Related bug:** BUG-005

---

## 7. Conflicting Requirements

**Test:**

`want a laptop under 1000 GEL and high performance`

Then:

`cheap but gaming laptop`

**Observed result:**

The chatbot could not provide a clear matching product and suggested
operator assistance.

**Result:** Needs improvement

This behavior was useful for exploratory testing, but I did not classify it
as a confirmed defect without a clear product/business requirement.

---

## 8. Product Comparison

**Test:**

`Compare iPhone 16 and Samsung S24`

**Observed result:**

The chatbot compared iPhone 16 with Samsung Galaxy S26 instead of the
requested Samsung S24.

**Result:** Fail

**Related bug:** BUG-004

---

## 9. Camera Comparison

**Test:**

`Which one has a better camera?`

**Observed result:**

The chatbot continued the comparison using iPhone 16 and Samsung Galaxy S26.

Because the previous comparison had already replaced S24 with S26, the
response continued with the incorrect product context.

**Result:** Fail

**Related bug:** BUG-004

---

## 10. Product Price

**Test:**

`What is the price?`

**Observed result:**

The chatbot stated that the selected Asus Vivobook model cost 1999 GEL.

The provided product link was opened and the product page showed 2099 GEL.

**Result:** Fail

**Related bug:** BUG-001

---

## 11. Product Link

**Test:**

Asked the chatbot to provide a link for the selected product.

**Observed result:**

The chatbot provided a product link that opened the product page.

However, the price on the page did not match the price provided by the
chatbot.

**Result:** Partial / Fail

**Related bug:** BUG-001

---

## 12. Purchase Intent

**Test:**

`Let's buy the laptop`

and:

`I want to buy it`

**Observed result:**

The chatbot recognized the purchase intent and explained that the user could
use the product page, cart, or online installment options.

However, it did not move into a structured checkout flow with a clear product
summary and confirmation.

**Result:** Needs improvement

This was documented as a UX / recommendation rather than a confirmed
functional defect.

---

## 13. Payment Method

**Test:**

`Can I pay cash?`

**Observed result:**

The chatbot explained that cash payment was available in physical stores and
described online payment options.

**Result:** Pass / No defect confirmed.

---

## 14. Pickup

**Test:**

`Can I pick it up tomorrow?`

**Observed result:**

The chatbot said pickup could be possible if the product was in stock and
asked which branch the user preferred.

**Result:** Needs verification

The chatbot did not actually verify a specific product's real-time stock
during this conversation.

---

## 15. Operator Handoff

**Test:**

`Connect me to operator`

**Observed result:**

The system confirmed:

`Your request has been sent to an operator.`

**Result:** Pass for operator request submission.

---

## 16. Return to AI After Operator Request

**Test:**

After requesting an operator:

`Never mind. Can you return to chatbot?`

**Observed result:**

The system responded that an operator had already been requested.

The user could not return to the AI chatbot through the conversation.

**Result:** Fail

**Related bug:** BUG-002

---

## 17. Minimize and Reopen Chat

**Test:**

1. Request an operator.
2. Minimize the chatbot.
3. Reopen it.
4. Continue the conversation.

**Observed result:**

The chatbot remained in the previous operator state.

Refreshing the page changed the behavior, but simply minimizing and reopening
the chat did not.

**Result:** Fail

**Related bug:** BUG-003

---

## 18. Topic Switching

**Test:**

`I want a laptop`

Then:

`Actually show me phones`

**Observed result:**

The chatbot switched from laptops to phones.

**Result:** Pass / No defect confirmed.

---

## 19. Multiple Topics in One Conversation

**Test:**

Laptop questions → phone comparison → laptop → phones → store information →
purchase.

**Observed result:**

The chatbot was able to continue the conversation, but longer conversations
created situations where context and product selection needed closer
verification.

**Result:** Exploratory observation

---

## 20. Store Information

**Test:**

`Where is your store?`

**Observed result:**

The chatbot provided specific store addresses and locations.

**Result:** Requirement concern

Based on the project requirement that the chatbot does not have an official
Alta website integration, providing specific branch addresses should be
reviewed.

This was treated as a requirement/business-rule issue rather than a confirmed
technical defect until the expected behavior is confirmed.

---

## 21. Material Question

**Test:**

`silver material?`

**Observed result:**

The chatbot correctly distinguished between a silver color and actual silver
material and explained that laptops were made from materials such as aluminum
or plastic.

**Result:** Pass / No defect confirmed.

---

## 22. Multiple Attribute Question

**Test:**

`silver material? design? color? RAM? price?`

**Observed result:**

The chatbot provided information about silver laptops, aluminum bodies,
RAM, design, and price range, then asked which brand was preferred.

**Result:** No confirmed defect from this specific test.

---

## 23. Product Memory

**Test:**

After discussing an Asus Vivobook:

`What I chose?`

**Observed result:**

The chatbot identified the Asus Vivobook configuration discussed earlier.

**Result:** Pass / No defect confirmed.

---

## 24. Mixed Language

**Test:**

The conversation was switched between English and Georgian.

**Observed result:**

The chatbot continued responding and understood the general conversation.

**Result:** Pass / No confirmed defect.

---

## 25. System Maintenance

**Test:**

During some messages, the chatbot displayed:

`System is under maintenance, please try again in a few minutes.`

**Observed result:**

The message appeared during testing and later the chatbot became available
again.

**Result:** Observed

This should not automatically be reported as a chatbot defect because the
system may genuinely have been unavailable at that moment.

---

# Confirmed / Documented Bugs

The following issues were strong enough to document as separate bugs:

| Bug ID | Issue | Result |
|---|---|---|
| BUG-001 | Chatbot price differs from product page | Fail |
| BUG-002 | User cannot clearly return from operator mode | Fail |
| BUG-003 | Operator state remains after minimize/reopen | Fail |
| BUG-004 | Requested Samsung S24 is replaced with S26 | Fail |
| BUG-005 | Multiple product requirements are not properly handled | Fail |

---

# Recommendations / Improvements

During testing, I also identified areas that may require product or UX
improvements but were not necessarily confirmed defects.

### Purchase flow

The chatbot recognizes purchase intent but could provide a more structured
path to checkout.

### Complex requests

The chatbot could improve how it handles several requirements in one message.

### Store information

The expected behavior for store addresses should be confirmed based on the
available integrations and business requirements.

### Pickup availability

The chatbot should only provide availability information if it has access to
current stock data.

---

# QA Conclusion

The chatbot handled many basic product questions successfully.

The most important issues found during exploratory testing were related to
data consistency, product identity, conversation state, operator handoff, and
complex user intent.

The testing also showed that an AI chatbot needs to be tested beyond simple
question-and-answer scenarios.

Long conversations, changing requirements, product comparisons, purchase
intent, and transitions between AI and human support can expose problems that
are not visible during basic functional testing.
