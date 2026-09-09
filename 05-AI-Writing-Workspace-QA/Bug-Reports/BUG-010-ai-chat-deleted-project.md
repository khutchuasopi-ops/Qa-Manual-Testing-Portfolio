# BUG-010 — Deleted Project Conversation Remains in AI Chat

## Title
Deleted Project conversation remains visible in the AI Chat dropdown

## Preconditions
- User is logged in.
- A project/manuscript has an associated AI Chat conversation.
- The project/manuscript can be deleted.

## Steps to Reproduce
1. Open a project/manuscript.
2. Open the associated AI Chat conversation.
3. Note the conversation title.
4. Delete the related project/manuscript.
5. Open the AI Chat conversation dropdown.
6. Search for the conversation associated with the deleted project/manuscript.

## Expected Result
If AI Chat conversations are expected to be linked to their project/manuscript, deleting the project/manuscript should also remove the related conversation from the AI Chat dropdown.

## Actual Result
The conversation associated with the deleted project/manuscript remains visible in the AI Chat dropdown.

## Priority
Medium

## Severity
Major

## Note
This behavior should be confirmed with the product requirements because AI Chat history may be designed to remain independent from project/manuscript deletion.

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: AI Chat / Project Management

## Evidence
Screen recording showing the project deletion and the conversation still appearing in the AI Chat dropdown.

## Status
Requires Product Confirmation
