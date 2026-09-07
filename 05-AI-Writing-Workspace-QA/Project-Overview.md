# Project Overview

## Project Name

AI Writing Workspace — Manual QA Testing

## Project Description

This project documents manual QA testing performed on a staging/preview environment of an AI-powered writing and planning workspace.

The application provides tools for creating and managing writing projects, planning content, working with drafts, interacting with an AI Assistant, and organizing documents in different views.

The purpose of this QA project was to evaluate the application from an end-user perspective and identify functional issues, data persistence problems, state-related issues, AI workflow problems, and usability improvements.

> Note: The product name has been anonymized for portfolio purposes.

## Testing Purpose

The main purpose of the testing was to verify whether the application's main user workflows behaved as expected.

Testing focused on:

- Functional behavior
- User workflows
- Data persistence
- Page refresh behavior
- Navigation
- AI Assistant functionality
- Draft editing
- Board interactions
- Plan generation
- Project management
- Poster management
- Templates
- Split View
- Conversation and context handling
- UI/UX behavior

## Application Areas Tested

### Board

The Board was tested for:

- Drag and drop functionality
- Moving items between sections
- Position persistence
- Item deletion
- Deleted item behavior after page refresh

### Draft

The Draft area was tested for:

- Initial Draft loading
- AI Assistant interaction
- Draft Editor text entry
- Text formatting behavior
- Draft content persistence
- Page refresh behavior
- AI-generated content
- Creating and editing Draft content
- New Draft context

### Plan

The Plan area was tested for:

- Opening the Plan
- Assistant-based planning
- AI-generated planning options
- Plan content updates
- Plan behavior after page refresh

### AI Chat

AI Chat was tested for:

- Sending messages
- Starting new conversations
- Conversation state
- Context isolation
- Project-related conversations
- AI-generated content

### Library

The Library was tested for:

- Opening Projects / Manuscripts
- Viewing Project details
- Navigation between Library and Projects
- Project details panel behavior

### Templates

Templates were tested for:

- Template interaction
- Draggable elements
- Cursor behavior
- Horizontal content behavior

### Poster / Cover

Poster functionality was tested for:

- Uploading a new image
- Saving poster changes
- Poster update behavior
- Upload dialog behavior after changing the poster

### Split View

Split View was tested for:

- Opening the same Draft in multiple panes
- Pagination behavior
- Page break consistency
- Content positioning between panes

## Testing Environment

Environment: Staging / Preview

Testing Type: Manual QA

Testing Approach: Exploratory and Functional Testing

Production Environment: Not tested

## Testing Methodology

The application was tested using realistic end-user workflows.

Testing was not limited to individual UI elements. The focus was also placed on how the application behaved when moving between different states.

Examples included:

- Refreshing pages after entering data
- Reopening previously edited content
- Switching between Draft and Plan
- Deleting items and checking whether they remained visible
- Starting new conversations
- Checking whether previous conversation context was retained
- Opening the same Draft in Split View
- Uploading and saving poster images
- Repeating actions to verify whether behavior was consistent

## QA Focus

A major focus of the testing was identifying problems that may not be visible during a single interaction.

Additional checks included:

- Data persistence after refresh
- State consistency after navigation
- Deleted content behavior
- AI-generated content placement
- New conversation context
- Draft content persistence
- UI feedback after actions
- Consistency between different views
- Delayed or incomplete actions

## Expected Outcome

The expected outcome of the testing was to verify that users could successfully:

- Create and manage writing projects
- Navigate between application sections
- Create and edit Draft content
- Save and retain their work
- Use AI-assisted features
- Create planning content
- Manage Projects and Posters
- Use Templates
- Work with Split View
- Start new conversations without unrelated previous context
- Continue working after refreshing the page

## QA Deliverables

The project includes:

- Project documentation
- Test plan
- Test scenarios
- Test cases
- Testing checklists
- Bug reports
- UX recommendations
- Testing evidence

## Portfolio Purpose

This project demonstrates a practical manual QA workflow and shows how I approach testing real-world web application functionality.

The project focuses on identifying reproducible issues, documenting clear reproduction steps, validating expected versus actual behavior, and evaluating both functional quality and user experience.
