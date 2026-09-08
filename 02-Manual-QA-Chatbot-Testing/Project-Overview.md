# Project Overview — AI Chatbot Manual QA Testing

## Project Information

| Field             | Details                                      |
| ----------------- | -------------------------------------------- |
| Project Type      | AI-powered E-commerce Chatbot                |
| Testing Type      | Manual Testing                               |
| QA Role           | Junior Manual QA Tester                      |
| Testing Approach  | Functional, Exploratory, Negative, Usability |
| Platform          | Web-based Chatbot                            |
| Test Environments | Desktop / Notebook and Mobile Device         |

---

## Project Description

This project focuses on the manual testing of an AI-powered chatbot used in an e-commerce environment.

The chatbot allows users to search for products, request product information, compare products, receive recommendations, ask purchase-related questions, and interact with a human operator.

The purpose of testing was to evaluate whether the chatbot responds appropriately to different user requests and maintains correct conversation behavior throughout the interaction.

---

## Testing Objectives

The main testing objectives were to:

* Verify core chatbot functionality
* Validate product-related responses
* Check product information and price consistency
* Verify conversation context
* Test follow-up questions
* Test multiple requirements in a single request
* Check topic switching
* Verify conversation state
* Test operator handoff and return behavior
* Test invalid and unexpected input
* Evaluate usability and response clarity
* Identify and document defects

---

## Testing Scope

### In Scope

The following areas were included in testing:

#### Product Functionality

* Product Search
* Product Information
* Product Prices
* Product Specifications
* Product Recommendations
* Product Comparison
* Product Links

#### Conversation Behavior

* Conversation Context
* Follow-up Questions
* Product Memory
* Topic Switching
* Multiple Requirements
* Ambiguous Requests
* Conflicting Requirements
* Conversation State

#### Purchase and Operator Flow

* Purchase Intent
* Ordering Questions
* Payment-related Questions
* Pickup / Availability Questions
* Operator Handoff
* Returning from Operator Mode
* Minimize and Reopen Chat

#### Negative and Exploratory Testing

* Invalid Input
* Random Input
* Special Characters
* Unknown Products
* Unexpected Requests
* Mixed-Language Input
* Error Handling

#### Usability and Localization

* Response Clarity
* Conversation Flow
* User Experience
* English Input
* Georgian Input
* Language Consistency

---

## Testing Approach

Testing was performed using both predefined test cases and exploratory testing.

### Functional Testing

Predefined test cases were used to verify expected chatbot behavior and important user flows.

### Negative Testing

Invalid, incomplete, ambiguous, and unexpected inputs were used to evaluate how the chatbot handles situations outside normal user behavior.

### Exploratory Testing

Exploratory sessions were used to investigate chatbot behavior beyond predefined test cases.

Testing focused on changing requirements, topic switching, complex requests, product substitution, conversation state, and unexpected responses.

### Usability Testing

The chatbot was evaluated from a user perspective, with attention to response clarity, conversation flow, and ease of interaction.

### Context and State Testing

Conversation history and chatbot state were tested to determine whether the chatbot maintained relevant information during an interaction and after state changes.

---

## Test Environments

Testing covered:

* Desktop / Notebook
* Mobile Device

The environments were used to evaluate chatbot behavior and interaction across different device contexts.

---

## Defects Identified

Five defects were documented during testing.

| Bug ID  | Area                | Summary                                                        |
| ------- | ------------------- | -------------------------------------------------------------- |
| BUG-001 | Product Information | Product price inconsistency                                    |
| BUG-002 | Operator Flow       | User cannot clearly return from operator mode                  |
| BUG-003 | Conversation State  | Operator state remains after minimizing and reopening the chat |
| BUG-004 | Product Comparison  | Requested product is replaced during comparison                |
| BUG-005 | User Requirements   | Multiple product requirements are not properly handled         |

Detailed information is available in the [Bug Reports](Bug-Reports/) folder.

---

## Test Documentation

The project includes:

* Test Plan
* Test Scenarios
* Test Cases
* Test Execution
* Exploratory Testing
* Bug Reports
* Case Study

---

## Out of Scope

The following areas were not included in this manual testing project:

* Source Code Testing
* Database Testing
* API Testing
* Performance / Load Testing
* Security Penetration Testing
* Automated Testing

---

## Project Limitations

This is a practical QA portfolio project and does not represent production-level testing experience.

Some chatbot behavior may depend on business rules, available product data, integrations, or requirements that are not publicly documented.

Where expected behavior could not be confirmed, the behavior was treated as an observation or requirement concern rather than automatically classified as a defect.

---

## Confidentiality

The original application name, company information, private test data, credentials, screenshots, and other confidential project materials are intentionally excluded from this public portfolio.

Only non-sensitive testing documentation and generalized examples are included.

---

## Junior QA Perspective

This project demonstrates my current practical experience as a **Junior Manual QA Tester**.

It focuses on manual test design, functional testing, exploratory testing, negative testing, conversation and state validation, defect reporting, and clear QA documentation.

The project also provided practical experience in testing an AI-powered user interface from a manual QA perspective.
