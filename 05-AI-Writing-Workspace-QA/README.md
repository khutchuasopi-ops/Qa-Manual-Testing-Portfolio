# AI Writing Workspace — Manual QA Testing

## Project Overview

This project documents **manual QA testing** performed on a staging/preview environment of an AI-powered writing and planning workspace.

The testing focused on core user workflows, data persistence, AI-assisted features, state management, and usability.

> **Note:** The product name has been anonymized for portfolio purposes.

---

## Testing Type

- Manual Functional Testing  
- Exploratory Testing  
- End-to-End User Flow Testing  
- Data Persistence & State Testing  
- AI Feature Testing  

**Environment:** Staging / Preview  

---

## Areas Tested

- Board (drag & drop, item management)
- Draft (editing, persistence, AI interaction)
- Plan
- AI Chat (context isolation, new conversations)
- Library / Project management
- Templates
- Split View
- Poster / Cover management
- Navigation & UI behavior

---

## Key Findings

During testing, several functional issues were identified:

- Deleted Board items remained visible after refresh
- Draft content was not preserved after page refresh
- Draft Editor converted lowercase text to uppercase
- AI Assistant could not reliably write content into an editable Draft
- New Draft retained context from a previous independent conversation
- AI-generated Plan content was not reflected on the Plan page
- Poster changes were not applied immediately after saving
- Poster upload dialog sometimes showed a previously uploaded image
- New Chat temporarily displayed the previous conversation
- Split View caused duplicated or reset pagination/page breaks

---

## Documentation

| Document | Description |
|----------|-------------|
| [Project Overview](./Project-Overview.md) | Full project details, scope and objectives |
| [Test Scenarios](./Test-Scenarios.md) | High-level test scenarios |
| [Test Cases](./Test-Cases.md) | Detailed test cases |
| [Checklists](./Checklists.md) | Testing checklists |
| [Bug Reports](./Bug-Reports) | Documented defects |
| [UX Recommendations](./UX-Recommendations) | Usability improvement suggestions |
| [Evidence](./Evidence) | Screenshots and supporting evidence |

---

## Skills Demonstrated

- Manual Functional Testing
- Exploratory Testing
- End-to-End Workflow Testing
- Data Persistence Testing
- State & Refresh Testing
- AI Feature Testing (context isolation, content generation)
- Rich-Text Editor Testing
- Drag & Drop Testing
- Split View Testing
- Bug Reproduction & Documentation
- Distinguishing Functional Bugs from UX Improvements

---

## Project Structure
