# AI Writing Workspace QA

## Project Overview

This project focuses on manual QA testing of an AI-powered writing workspace in a staging / preview environment.

The goal was to verify core user workflows, identify functional issues, check data persistence and AI-related behavior, and document usability observations.

Production was not tested as part of this project.

---

## Testing Scope

The testing covered the following areas:

* Board
* Draft Editor
* Draft creation and editing
* Draft persistence
* Plan
* AI Assistant
* AI Chat
* Library
* Templates
* Poster / Cover
* Split View
* Project / Manuscript details
* Navigation
* UI / UX
* Data persistence
* AI workflows
* AI context and conversation state

---

## Testing Approach

The following manual testing approaches were used:

* Functional testing
* Exploratory testing
* Smoke testing
* Regression testing
* Negative testing
* User-flow testing
* UI / UX testing
* Persistence testing
* AI workflow testing
* Context and state testing

---

## Test Results

A total of **28 test cases** were documented.

| Result                        |  Count |
| ----------------------------- | -----: |
| PASS                          |     12 |
| FAIL                          |     11 |
| Requires Product Confirmation |      4 |
| UX Recommendation Only        |      1 |
| **Total**                     | **28** |

The testing identified:

* **9 confirmed bugs**
* **4 behaviors requiring product confirmation**
* **2 UX recommendations**

---

## Confirmed Bugs

### BUG-001 — Draft Content Lost After Refresh

Draft content was lost after refreshing the page.

### BUG-002 — Draft Editor Lowercase Automatically Uppercase

Lowercase text entered in the Draft Editor was automatically converted to uppercase.

### BUG-003 — AI Assistant Fails to Write Into Editable Draft

The AI Assistant failed to insert generated content into the editable Draft.

### BUG-004 — New Draft Retains Previous Independent Conversation Context

A newly created Draft retained conversation context from a previous independent conversation.

### BUG-005 — AI-Generated Plan Content Not Reflected on Plan Page

AI-generated Plan content was not correctly reflected on the Plan page.

### BUG-006 — Save Poster Action Delayed / Unresponsive

The Save Poster action was delayed or appeared unresponsive.

### BUG-007 — Upload Dialog Shows Previous Image

The image upload dialog displayed an image from a previous operation.

### BUG-008 — New Chat Temporarily Shows Previous Conversation

Starting a new Chat temporarily displayed the previous conversation until new text was entered.

### BUG-009 — Split View Pagination / Page State Breaks

Split View pagination became inconsistent, with pages being duplicated or reset during navigation.

---

## Product Confirmation Items

The following observations were not classified as confirmed bugs because the intended product behavior requires clarification:

* **TC-004** — Board item deletion behavior
* **TC-005** — Draft initial loading behavior
* **TC-023** — Conversation availability after Project deletion
* **TC-025** — Horizontal Template content behavior

---

## UX Recommendations

Two UX recommendations were identified:

### UX-001 — Grab Cursor for Draggable Template Elements

A grab cursor would make it clearer that Template elements can be dragged.

### UX-002 — Close Button for Project / Manuscript Details

A visible Close (X) button would make the details panel easier to close and improve interaction clarity.

---

## Test Documentation

The project contains the following QA documentation:

* [Project Overview](./Project-Overview.md)
* [Test Plan](./Test-Plan.md)
* [Test Scenarios](./Test-Scenarios.md)
* [Test Cases](./Test-Cases.md)
* [Checklists](./Checklists.md)
* [Bug Reports](./Bug-Reports)

UX recommendations are documented within the relevant testing documentation.

---

## Environment

**Environment:** Staging / Preview

**Production:** Not tested

---

## Testing Status

**Completed**

The project documents the manual testing performed on the staging / preview environment, including test coverage, observed failures, confirmed defects, product-confirmation items, and UX recommendations.
