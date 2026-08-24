# Exploratory Testing — AI E-commerce Chatbot

## Overview

For exploratory testing, I tested the chatbot without following only predefined
test cases.

The main goal was to see how the chatbot behaves when a real user changes their
mind, asks several questions at once, switches between products, uses different
languages, gives unclear information, or tries to leave and return to the
conversation.

I focused mainly on user flow, conversation context, product information,
purchase intent, operator handoff, and unexpected input.

---

## 1. Product Context

I started by asking about a laptop and then asked follow-up questions about:

- price
- RAM
- color
- design
- material
- warranty
- gaming performance

### What I checked

I wanted to see whether the chatbot remembered the product and considered all
the information from the conversation.

### Observation

In some cases, the chatbot focused on only one attribute instead of considering
the complete request.

This can make the recommendation less useful because the user may have given
several important requirements.

---

## 2. Changing the Product Category

I started with laptops and then changed the topic to phones.

Example:

`Tell me about laptops`

Then:

`Actually show me phones`

### What I checked

I checked whether the chatbot would follow the latest request or continue
using the previous laptop context.

### Observation

The chatbot was able to switch topics, but this type of conversation can
easily cause context-mixing issues, so I included it as an important area for
further testing.

---

## 3. Complex User Requests

I sent several requirements in one message.

Example:

`color RAM price design material battery warranty gaming office`

### What I checked

I wanted to see whether the chatbot would:

- understand all the requested attributes
- organize the information
- ask clarification questions
- recommend a suitable product

### Observation

The response sometimes simplified the request and focused on one attribute,
such as RAM.

This can be a problem when the user expects the chatbot to consider all of
their requirements.

---

## 4. Conflicting Requirements

I tested requests such as:

`I want a laptop under 1000 GEL and high performance`

and:

`cheap but gaming laptop`

### What I checked

I wanted to see whether the chatbot would recognize that some requirements
may be difficult to satisfy at the same time.

### Expected behavior

The chatbot should explain the limitation or ask which requirement is more
important.

### Observation

The chatbot sometimes moved directly to another recommendation or suggested
contacting an operator without helping the user understand the available
options.

---

## 5. Purchase Intent

I tested different ways of saying that I wanted to buy a product.

Examples:

`I want to buy it`

`Let's buy the laptop`

`I decided to buy it`

### What I checked

I wanted to see whether the chatbot would guide the user through a clear
purchase process.

### Observation

The chatbot recognized the purchase intent, but the conversation did not
always move into a structured checkout flow.

For example, it could provide a general instruction to use the website cart,
but it did not always provide a clear summary of the selected product and
next steps.

---

## 6. Product Price Consistency

I asked the chatbot for the price of a specific product and then opened the
product link provided by the chatbot.

### What I checked

I compared the price shown in the chatbot with the price shown on the actual
product page.

### Observation

I found a case where the chatbot showed one price while the product page
showed a different price.

This is important because price information directly affects the user's
purchase decision.

---

## 7. Product Link Verification

I asked the chatbot to provide a link for the selected product.

### What I checked

After opening the link, I compared:

- product name
- model
- color
- RAM
- storage
- price

with the information previously provided by the chatbot.

### Observation

The link opened a product page, but the price did not match the price provided
in the chat.

This was treated as a potential product-information consistency defect.

---

## 8. Operator Handoff

I tested the operator flow using:

`Connect me to operator`

After the operator request was submitted, I tried:

`Never mind. Can you return to chatbot?`

### What I checked

I wanted to see whether the user could return to the AI chatbot after
requesting an operator.

### Observation

The chatbot remained in the operator state and responded that an operator
had already been requested.

This raised a question about whether the user can return to AI without
refreshing the page.

---

## 9. Minimize and Reopen

While the chat was in the operator state, I minimized the chat using the
available minimize button.

I then reopened the chat.

### What I checked

I wanted to see whether minimizing and reopening the chat would reset the
state or keep the previous state.

### Observation

The chat continued to show the previous operator state.

Refreshing the page changed the behavior, but simply minimizing and reopening
did not.

This should be reviewed from a user-experience perspective because the user
does not have a clear "close conversation" option.

---

## 10. Mixed Languages

I tested messages containing multiple languages.

Example:

`Hello გამარჯობა Hola Bonjour`

I also switched between English and Georgian during the same conversation.

### What I checked

I wanted to see whether the chatbot could understand the request and maintain
a consistent response.

### Observation

The chatbot was generally able to continue the conversation, but product
information and category names could still appear in Georgian even when the
conversation was being conducted in English.

This is an area that should be checked against the expected product
localization requirements.

---

## 11. Invalid and Random Input

I tested inputs such as:

`123456789`

`22@@@@@@@`

### What I checked

I wanted to see whether unexpected input could break the chatbot.

### Expected behavior

The chatbot should handle invalid or meaningless input gracefully without
crashing or entering an incorrect state.

---

## 12. Product Substitution

I asked for a specific product comparison.

Example:

`Compare iPhone 16 and Samsung S24`

### What I checked

I checked whether the chatbot compared exactly the products requested by the
user.

### Observation

The chatbot responded by comparing iPhone 16 with Samsung Galaxy S26 instead
of Samsung S24.

This is important because the chatbot should not silently replace a product
requested by the user.

---

## 13. Ambiguous Questions

I tested short follow-up questions such as:

`Which one?`

and:

`What about it?`

### What I checked

I wanted to see whether the chatbot would ask for clarification when the
conversation contained multiple possible products.

### Expected behavior

If the question is unclear, the chatbot should ask the user to clarify rather
than guessing.

---

## 14. Topic Switching

I tested several topic changes in one conversation.

Example:

`Tell me about laptops`

Then:

`Show me phones`

Then:

`Where is your store?`

Then:

`Let's buy the laptop`

### What I checked

I wanted to see whether the chatbot correctly handled the latest request
without mixing old context with the new request.

### Observation

Topic switching worked in some cases, but it is an important area for
continued testing because product context can easily become mixed after several
conversation changes.

---

## 15. What I Focused On

During exploratory testing, I mainly looked for:

- Wrong product recommendations
- Product information inconsistencies
- Incorrect prices
- Context loss
- Context mixing
- Product substitution
- Poor clarification
- Ignored user requirements
- Weak purchase flows
- Operator-state problems
- Conversation-state problems
- Language issues
- Unexpected input handling
- Broken links
- Inconsistent chatbot responses

---

## 16. Main Findings

The most interesting issues found during exploratory testing were:

1. The chatbot could simplify a complex request too much.
2. Product information could become inconsistent between the chatbot and the
   product page.
3. The chatbot could replace a requested product with another model.
4. Purchase intent did not always lead to a structured purchase flow.
5. The operator state could leave the user unable to return to the AI chatbot.
6. Conversation state could remain after minimizing and reopening the chat.
7. The chatbot sometimes needed better clarification when the user's request
   was ambiguous or contained conflicting requirements.

---

## 17. Why Exploratory Testing Was Useful

Predefined test cases are useful for checking known requirements, but
exploratory testing helped me find problems that were not obvious from a
simple happy-path flow.

By changing the user's language, requirements, product category, purchase
intent, and conversation direction, I was able to test the chatbot more like
a real customer would use it.

This helped identify issues related not only to individual responses, but also
to the overall conversation and user experience.
