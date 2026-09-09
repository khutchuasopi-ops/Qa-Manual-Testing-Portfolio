# BUG-006 — New Draft Retains Context from a Previous Conversation

## Title
New Draft retains context from a previous independent conversation

## Preconditions
- User is logged in.
- A previous independent document/conversation contains different writing content.
- A new Draft can be opened.

## Steps to Reproduce
1. Open a new Draft.
2. Start a new conversation with the AI Assistant.
3. Enter a completely unrelated new topic.
4. Continue the conversation.
5. Observe the Assistant responses.

## Expected Result
The new Draft should start with a clean context.

The AI Assistant should only use information related to the current Draft and current conversation.

## Actual Result
The new Draft retains or references content from a previous independent document/conversation.

The Assistant may mention unrelated previous topics even though the user is working on a new Draft.

## Priority
Medium

## Severity
Major

## Environment
- Environment: Staging / Preview
- Testing type: Manual QA
- Area: Draft / AI Assistant

## Evidence
Screen recording showing the new Draft, the new topic entered by the user, and the Assistant referencing unrelated previous content.

## Status
Open
