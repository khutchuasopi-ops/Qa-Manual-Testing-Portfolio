# BUG-005 — AI Assistant Fails to Write Content into an Editable Draft

## Title
AI Assistant fails to create or write content into an editable Draft

## Preconditions
- User is logged in.
- A project/manuscript with an available Draft exists.
- AI Assistant is available in the Draft flow.

## Steps to Reproduce
1. Open a project/manuscript.
2. Navigate to the Draft section.
3. Start a conversation with the AI Assistant.
4. Provide a writing request, for example:
   `Write about fairies and elves.`
5. Provide the requested additional information when prompted.
6. Observe the AI Assistant response and the Draft.

## Expected Result
The AI Assistant should create or update the Draft with the requested content.

The generated content should be available in an editable Draft.

## Actual Result
The AI Assistant indicates that it is writing or editing the Draft, but the requested content is not correctly created in an editable Draft.

In some cases, the Assistant displays an error such as:

`No fs_entries mirror found for draft; AI webhooks require the archive-node id.`

In other cases, the Assistant reports that it could not reach or edit the Draft.

## Priority
High

## Severity
Critical

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Draft / AI Assistant

## Evidence
Screen recording showing the AI writing request, Assistant response, and the resulting Draft state or error message.

## Status
Open
