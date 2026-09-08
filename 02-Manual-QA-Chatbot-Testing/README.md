# AI Chatbot — Manual QA Testing

## Project Overview

This project demonstrates practical **Manual and Exploratory QA Testing** of an AI-powered chatbot used in an e-commerce environment.

The chatbot is designed to help users search for products, ask about product information and prices, compare products, receive recommendations, ask about purchasing options, and interact with a human operator.

The main focus of testing was the chatbot's functionality, conversation context, product information, price consistency, error handling, state management, and overall user experience.

---

## QA Role

**Junior Manual QA Tester**

**Testing Type:** Manual Testing

**Application Type:** AI-powered E-commerce Chatbot

---

## Testing Approach

The project combines structured test case execution with exploratory testing.

Testing was performed from a real-user perspective using:

* Normal user questions
* Follow-up questions
* Multiple requirements in one request
* Invalid and unexpected input
* Mixed-language messages
* Topic changes
* Product comparisons
* Purchase-related questions
* Operator interaction
* Conversation state changes

---

## Main Testing Areas

### Product Testing

* Product Search
* Product Information
* Product Prices
* Product Specifications
* Product Recommendations
* Product Comparison
* Product Links
* Product Information Consistency

### Conversation Testing

* Conversation Context
* Follow-up Questions
* Topic Switching
* Multiple Requirements
* Ambiguous Questions
* Conflicting Requirements
* Product Memory
* Conversation State

### Purchase and Operator Flow

* Purchase Intent
* Ordering Questions
* Payment Questions
* Pickup / Availability Questions
* Operator Handoff
* Returning from Operator Mode
* Minimize and Reopen Chat

### Negative and Exploratory Testing

* Invalid Input
* Random Input
* Special Characters
* Unknown Products
* Unexpected User Requests
* Mixed-Language Input
* Error Handling

### Usability and Localization

* User Experience
* Response Clarity
* Conversation Flow
* English and Georgian Input
* Language Consistency

---

## QA Activities

The project includes:

* Test Planning
* Test Scenario Design
* Test Case Design
* Manual Functional Testing
* Exploratory Testing
* Negative Testing
* Context Testing
* State Testing
* Data Consistency Testing
* Usability Testing
* Defect Identification
* Bug Reporting
* Test Execution Reporting

---

## Test Documentation

The project contains:

* [Project Overview](Project-Overview.md)
* [Test Plan](Test-Plan.md)
* [Test Scenarios](Test-Scenarios.md)
* [Test Cases](Test-Cases.md)
* [Test Execution](Test-Execution.md)
* [Exploratory Testing](Exploratory-Testing.md)
* [Bug Reports](Bug-Reports/)
* [Case Study](Case-Study.md)

---

## Defects Identified

The testing documentation contains five documented defects:

* BUG-001 — Product price inconsistency
* BUG-002 — User cannot clearly return from operator mode
* BUG-003 — Operator state remains after minimizing and reopening the chat
* BUG-004 — Requested product is replaced during comparison
* BUG-005 — Multiple product requirements are not properly handled

The detailed reproduction steps, expected results, actual results, severity, priority, and related testing information are available in the [Bug Reports](Bug-Reports/) folder.

---

## Test Execution

The execution report documents manual and exploratory testing results across areas including:

* Product Search
* Product Information
* Product Recommendations
* Product Comparison
* Price Consistency
* Purchase Intent
* Operator Handoff
* Conversation State
* Topic Switching
* Mixed-Language Input
* Error Handling

The execution report distinguishes between confirmed defects, observations, and areas that require further verification.

---

## Exploratory Testing

Exploratory testing was used to test the chatbot beyond predefined test cases.

The exploratory sessions focused on:

* Changing product requirements
* Switching product categories
* Complex requests
* Conflicting requirements
* Purchase intent
* Product price consistency
* Product links
* Operator handoff
* Conversation state
* Mixed-language input
* Product substitution
* Ambiguous questions
* Topic switching

This approach helped identify issues that could be difficult to discover through predefined test cases alone.

---

## Testing Environment

Testing covered web-based chatbot behavior on:

* Desktop / Notebook
* Mobile Device

The execution documentation records the relevant environment information where applicable.

Specific confidential application details and private test data are intentionally excluded from this public portfolio.

---

## Out of Scope

The following areas were outside the scope of this manual testing project:

* Source Code Testing
* Database Testing
* API Testing
* Performance / Load Testing
* Security Penetration Testing
* Automated Testing

---

## Tools

Tools used for this project include:

* GitHub
* Markdown
* Web Browser
* Chrome DevTools

---

## Skills Demonstrated

### Manual Testing

* Functional Testing
* Exploratory Testing
* Negative Testing
* Usability Testing
* Context Testing
* State Testing
* Data Consistency Testing

### Test Design

* Test Scenario Design
* Test Case Design
* Test Data Preparation
* User Flow Analysis

### Defect Management

* Defect Identification
* Bug Reporting
* Severity and Priority Assignment
* Defect Traceability

### Documentation

* Test Plan
* Test Scenarios
* Test Cases
* Exploratory Testing Sessions
* Test Execution Report
* Bug Reports
* Case Study

---

## Project Limitations

This project is a practical QA portfolio project and does not represent production-level testing experience.

Some chatbot behaviors depend on application requirements, available product data, integrations, and business rules.

Where expected behavior could not be confirmed from a defined requirement, the behavior was documented as an observation or requirement concern rather than automatically classified as a defect.

---

## Confidentiality

The original application name, company information, screenshots, private test data, and other confidential project materials are intentionally excluded from this public portfolio.

Only non-sensitive testing documentation and generalized examples are included.

---

## Junior QA Perspective

This project reflects my current level as a **Junior Manual QA Tester**.

It demonstrates my ability to:

* Analyze user flows
* Design manual test scenarios and test cases
* Perform functional and exploratory testing
* Investigate chatbot behavior
* Identify unexpected behavior
* Document defects clearly
* Distinguish confirmed defects from observations
* Communicate testing findings in a structured way

The project also demonstrates my interest in testing modern AI-powered user experiences from a manual QA perspective.
