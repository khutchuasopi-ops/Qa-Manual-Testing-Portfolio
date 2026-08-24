# Project Overview

## Project Name

AI Chatbot — Manual & Exploratory QA Testing

## Project Type

E-commerce AI Chatbot

## Testing Type

Manual Testing

Exploratory Testing

## Project Description

The chatbot is designed to help customers find and learn about products in an e-commerce environment.

Users can ask questions about products, prices, colors, RAM, storage, warranty, product recommendations, comparisons, purchasing options, and other product-related information.

The chatbot can also transfer the user to a human operator.

## Testing Objective

The main objective was to verify whether the chatbot:

- Provides relevant responses
- Understands user intent
- Maintains conversation context
- Provides consistent product information
- Provides accurate prices
- Handles multiple requirements
- Handles changes of topic
- Supports a clear purchase journey
- Handles operator interaction correctly
- Recovers from errors
- Handles unexpected and invalid input

## Main Testing Areas

### Product Search

Testing searches based on:

- Product category
- Price
- Brand
- RAM
- Color
- Usage
- Gaming requirements

### Product Information

Testing questions about:

- Price
- RAM
- Storage
- Colors
- Materials
- Warranty
- Battery
- Design

### Conversation Context

Testing whether the chatbot remembers:

- Previously selected products
- Previous requirements
- Product attributes
- Previous questions
- Changes of topic

### Purchase Flow

Testing:

- Purchase intent
- Ordering questions
- Payment questions
- Delivery questions
- Pickup questions
- Return questions
- Product links

### Operator Flow

Testing:

- Requesting an operator
- Waiting for an operator
- Returning to the chatbot
- Minimizing the chat
- Reopening the chat
- Chat state persistence

### Error Handling

Testing:

- Maintenance messages
- Invalid input
- Random input
- Special characters
- Unknown products
- Recovery after errors

## Testing Devices

Testing was performed on:

- Desktop / notebook
- Mobile device

The exact device, OS, browser and browser version are recorded where relevant in test evidence and bug reports.

## Testing Result

Exploratory testing identified several issues involving:

- Operator state
- Product price consistency
- Business-rule compliance
- Handling of multiple product requirements
- Error handling
