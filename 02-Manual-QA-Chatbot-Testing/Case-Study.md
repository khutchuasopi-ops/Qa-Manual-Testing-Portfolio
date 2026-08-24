# Case Study — AI E-commerce Chatbot Testing

## Project Background

I performed manual and exploratory testing of an AI-powered e-commerce
chatbot designed to help customers find products, compare products, get
product information, and receive assistance during the purchase process.

The testing was based on realistic customer conversations.

## Testing Goal

The main goal was to evaluate whether the chatbot could:

- Understand customer requests.
- Provide relevant product information.
- Maintain conversation context.
- Handle multiple requirements.
- Compare the correct products.
- Support purchase-related questions.
- Correctly handle the transition between AI and human support.
- Provide consistent product information.

## Testing Approach

I started with simple questions and gradually increased the complexity of
the conversations.

I tested:

1. Basic product questions.
2. Product specifications.
3. Price and color questions.
4. Product recommendations.
5. Multiple requirements in one message.
6. Product comparisons.
7. Changes in user intent.
8. Purchase intent.
9. Payment and pickup questions.
10. Operator handoff.
11. Returning from operator mode.
12. Minimize and reopen behavior.
13. Mixed-language conversations.
14. Unexpected and ambiguous requests.

## Important Findings

During exploratory testing, I identified several important issues.

### 1. Product Price Inconsistency

The chatbot provided one price while the linked product page displayed a
different price.

This could directly affect a customer's purchasing decision.

### 2. Incorrect Product Comparison

When the user requested a comparison between iPhone 16 and Samsung S24,
the chatbot replaced Samsung S24 with Samsung S26.

The chatbot should not silently change the requested product.

### 3. Operator State Problem

After requesting an operator, the user could not clearly return to the AI
chatbot.

The operator state also remained after minimizing and reopening the chat.

### 4. Complex User Requirements

When the user provided several requirements such as price, RAM, design,
material, battery, warranty, gaming, and office use, the chatbot focused
mainly on one attribute.

This showed that complex user intent requires additional testing.

## QA Analysis

The testing showed that the chatbot generally handled simple questions well.

However, longer and more complex conversations exposed problems that were not
visible during basic testing.

The most important areas requiring attention were:

- Product data consistency
- Conversation state
- Product identity
- Complex intent handling
- Purchase flow
- Operator handoff

## Result

The testing produced five documented bugs and several additional UX and
requirement observations.

The findings were documented with clear reproduction steps, actual results,
expected results, severity, priority, and impact.

## What I Learned

This project helped me understand that testing an AI chatbot requires more
than checking whether an answer is returned.

A response can look reasonable while still being incorrect because the
chatbot may:

- Change the user's requested product.
- Lose part of the user's intent.
- Use outdated or inconsistent information.
- Maintain an incorrect conversation state.
- Fail when the conversation becomes more complex.

Exploratory testing was especially useful for discovering these issues.
